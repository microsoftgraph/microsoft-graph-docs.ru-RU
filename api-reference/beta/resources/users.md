---
title: Работа с пользователями в Microsoft Graph
description: Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a5e1ed5a2403def740d92b9f77d57a58f6d1a3e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912017"
---
# <a name="working-with-users-in-microsoft-graph"></a>Работа с пользователями в Microsoft Graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.

Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.

- По идентификатору пользователя (`/users/{id}`). 
- С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.

## <a name="authorization"></a>Authorization
Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Общие свойства

| Свойство | Описание |
|----------|-------------|
| displayName | Имя, отображаемое в адресной книге, для пользователя.|
|givenName| Имя пользователя. |
|surname| Фамилия пользователя. |
|mail| Электронный адрес пользователя. |
|photo;| Фотографий профиля пользователя. |

Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).

## <a name="common-operations"></a>Стандартные действия
>**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.

| Путь    | Описание |
|---------|-------------|
|[`/users`](../api/user-list.md) | Вывод списка пользователей в организации. |
|[`/users/{id}`](../api/user-get.md) | Получение определенного пользователя по идентификатору. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Получение фотографии профиля пользователя. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Получение сведений о руководителе пользователя. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Вывод списка электронных писем пользователя в его основном почтовом ящике. |
|[`/users/{id}/events`](../api/user-list-events.md) | Вывод списка предстоящих событий пользователя из его календаря. |
|[`/users/{id}/drive`](../api/drive-get.md)| Получение хранилища файлов OneDrive пользователя. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Вывод списка групп, участником которых является пользователь. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Список групп Майкрософт, который входит пользователь. |
