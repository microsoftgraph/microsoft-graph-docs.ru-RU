---
title: Диспетчер приглашений
description: 'С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 524e97befcdc08fcf216255ee37f981a5f2b54ac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341381"
---
# <a name="invitation-manager"></a>Диспетчер приглашений

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|invitedUserType|String|Элемент userType, связанный с приглашаемым пользователем. Значение по умолчанию: Guest. Вы можете пригласить как участник, если вы являетесь администратором компании. |
|status|String|Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|invitedUser|[user](user.md)|Пользователь, создаваемый при создании приглашения. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "string",
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
