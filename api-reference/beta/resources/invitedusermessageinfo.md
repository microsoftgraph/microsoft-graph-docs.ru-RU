---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: Sammak
ms.openlocfilehash: 610a82646b87775e4f50651a2fc8f617f1782108
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952797"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения приглашения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|Коллекция [recipient](recipient.md)|Дополнительные получатели, в которые должно быть отправлено приглашение. В настоящее время поддерживается только один дополнительный получатель.|
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
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


