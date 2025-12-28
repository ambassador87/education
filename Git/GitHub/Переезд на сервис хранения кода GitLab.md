```bash
# Изменяет адрес удаленного репозитория origin
git remote set-url origin <новый_URL>
# git remote -- команда для работы с удаленными репозиториями
# set-url -- подкоманда для изменения URL репозитория
# origin -- имя удаленного репозитория

# Если бы origin не существоввал, нжно было бы создать его
git remote add origin <URL>

# Проверить адрес удаленного репозитория, к которому привязан локальный
git remote -v
# origin  git@gitlab.com:username/repo.git (fetch)
# origin  git@gitlab.com:username/repo.git (push)
```
### Когда это нужно

- Репозиторий переехал на другой сервер (например, GitHub → GitLab)    
- Хочешь сменить способ доступа (HTTPS → SSH)    
- Исправляешь неправильный URL

После привязки нового origin к local можно запушить историю локального репозитория
```bash
git push -u origin --all

# --all -- отправляет все локальные ветки в удаленный репозиторий
# -u -- устанавливает upstream (связь local_branch ↔ origin/local_branch) 
# для каждой отправленной ветки

```