---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: elisolMS
ms.openlocfilehash: 6092a5bd493377480c0a835b28982aec2d95c522
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131501"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения приглашения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|Коллекция [recipient](recipient.md)|Дополнительные получатели, на которые должно быть отправлено приглашение. В настоящее время поддерживается только один дополнительный получатель.|
|customizedMessageBody|Строка|Настраиваемый текст сообщения, который необходимо отправить, если сообщение по умолчанию не нужно.|
|messageLanguage|Строка|Язык, на который вы хотите отправить сообщение по умолчанию. Если задан параметр customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью параметра customizedMessageBody. Формат языка должен быть в формате ISO 639. Значение по умолчанию : en-US.|

## <a name="json-representation"></a>Представление в формате JSON
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


