---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 0d0e4742b3d41ba5f8dd1da49b234005aa2e766f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442345"
---
# <a name="working-with-users-in-microsoft-graph"></a>Работа с пользователями в Microsoft Graph

Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.

Вы можете получить доступ к [пользователям](user.md) через Microsoft Graph двумя указанными ниже способами.

- По идентификатору пользователя (`/users/{id | userPrincipalName}`).
- С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.

## <a name="authorization"></a>Авторизация

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

Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей. Это подмножество всех доступных свойств. Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.

|Свойство |Описание |
|:----------|:-------------|
|id | Уникальный идентификатор для пользователя.|
|businessPhones | Номера телефонов пользователя.|
|displayName | Имя, отображаемое в адресной книге, для пользователя.|
|givenName| Имя пользователя. |
|jobTitle | Должность пользователя.|
|mail| Электронный адрес пользователя. |
|mobilePhone | Номер мобильного телефона пользователя.|
|officeLocation | Физическое расположение офиса пользователя.|
|preferredLanguage | Предпочитаемый язык пользователя.|
|surname| Фамилия пользователя. |
|userPrincipalName| Имя участника-пользователя для пользователя. |

Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).

## <a name="common-operations"></a>Стандартные действия

> **Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.

| Path    | Описание |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | Вывод списка пользователей в организации. |
|[`/users/{id}`](../api/user-get.md) | Получение определенного пользователя по идентификатору. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Получение фотографии профиля пользователя. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Получение сведений о руководителе пользователя. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Вывод списка электронных писем пользователя в его основном почтовом ящике. |
|[`/users/{id}/events`](../api/user-list-events.md) | Вывод списка предстоящих событий пользователя из его календаря. |
|[`/users/{id}/drive`](../api/drive-get.md)| Получение хранилища файлов OneDrive пользователя. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Вывод списка групп, участником которых является пользователь. |
