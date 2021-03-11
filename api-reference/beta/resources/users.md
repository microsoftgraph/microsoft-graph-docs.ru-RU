---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c18731042d9d86479c5658f0a0f38a38d23bdb0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719824"
---
# <a name="working-with-users-in-microsoft-graph"></a>Работа с пользователями в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.

Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.

- По идентификатору пользователя (`/users/{id}`).
- С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.

## <a name="authorization"></a>Авторизация

Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](/graph/permissions-reference). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- User.ManageIdentities.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Общие свойства

| Свойство | Описание |
|----------|-------------|
| displayName | Имя, отображаемое в адресной книге, для пользователя.|
|givenName| Имя пользователя. |
|surname| Фамилия пользователя. |
|mail| Адрес электронной почты пользователя. |
|photo| Фотография профиля пользователя. |

Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).

## <a name="common-operations"></a>Стандартные действия

>**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.

| Path    | Описание |
|---------|-------------|
|[`/users`](../api/user-list.md) | Вывод списка пользователей в организации. |
|[`/users/{id}`](../api/user-get.md) | Получение определенного пользователя по идентификатору. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Получение фотографии профиля пользователя. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Получение сведений о руководителе пользователя. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Вывод списка электронных писем пользователя в его основном почтовом ящике. |
|[`/users/{id}/events`](../api/user-list-events.md) | Вывод списка предстоящих событий пользователя из его календаря. |
|[`/users/{id}/drive`](../api/drive-get.md)| Получение хранилища файлов OneDrive пользователя. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Вывод списка групп, участником которых является пользователь. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Вывод списка команд Microsoft Teams, участником которых является пользователь. |

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.