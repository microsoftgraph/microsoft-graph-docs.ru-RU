---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
ms.localizationpriority: medium
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 473e043da7669cc07e79fdf3a06edb0d36f657ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084421"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения приглашения

Пространство имен: microsoft.graph

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|Коллекция объектов [Recipient](recipient.md)|Дополнительные получатели, в которые должно быть отправлено приглашение. В настоящее время поддерживается только один дополнительный получатель.|
|customizedMessageBody|Строка|Настраиваемый текст сообщения, который необходимо отправить, если не нужно сообщение по умолчанию.|
|messageLanguage|Строка|Язык, на который нужно отправить сообщение по умолчанию. Если задан настраиваемыйMessageBody, это свойство игнорируется, и сообщение отправляется с помощью настраиваемогоMessageBody. Формат языка должен быть в ISO 639. По умолчанию — en-US.|

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

