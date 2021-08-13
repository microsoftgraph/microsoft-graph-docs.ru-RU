---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f35cd50c66d6d34b2837911514a9ac53387915bb19cbb46c0a0b36cb708ebe4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218459"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения приглашения

Пространство имен: microsoft.graph

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|Коллекция объектов [Recipient](recipient.md)|Дополнительные получатели, в которые должно быть отправлено приглашение. В настоящее время поддерживается только один дополнительный получатель.|
|customizedMessageBody|String|Настраиваемый текст сообщения, который необходимо отправить, если не нужно сообщение по умолчанию.|
|messageLanguage|String|Язык, на который нужно отправить сообщение по умолчанию. Если задан настраиваемыйMessageBody, это свойство игнорируется, и сообщение отправляется с помощью настраиваемогоMessageBody. Формат языка должен быть в ISO 639. По умолчанию — en-US.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

