---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
ms.localizationpriority: high
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: fcf43ab888318ce0769db04d5b83994cb6762c58
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695584"
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