---
title: Диспетчер приглашений
description: 'С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72ff2ca13a0de314697961504da9a4203afdb2b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981051"
---
# <a name="invitation-manager"></a>Диспетчер приглашений

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию. 

Процесс приглашения:

* Создается приглашение.
* Приглашение с соответствующей ссылкой отправляется пользователю.
* Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.
* После активации пользователь перенаправляется на определенную страницу.

При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.


## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание приглашений](../api/invitation-post.md) | invitation | Запись свойств и отношений объекта приглашения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|Отображаемое имя приглашаемого пользователя.|
|invitedUserEmailAddress|String|Адрес электронной почты приглашаемого пользователя. Указывать обязательно.|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.|
|sendInvitationMessage|Boolean|Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.|
|inviteRedirectUrl|String|URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.|
|inviteRedeemUrl|String|URL-адрес для активации приглашения. Только для чтения.|
|invitedUserType|String|Элемент userType, связанный с приглашаемым пользователем. Значение по умолчанию: Guest. Администратор компании может заменить его на Member. |
|status|String|Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|invitedUser|[User](user.md)|Пользователь, создаваемый при создании приглашения. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
