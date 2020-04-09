---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
author: elisolMS
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5bdcc08721a56d379790b83d70aae216d169c6af
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200294"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения с приглашением

Пространство имен: microsoft.graph

Объект invitedUserMessageInfo позволяет настроить сообщение с [приглашением](invitation.md) .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|Коллекция объектов [Recipient](recipient.md)|Дополнительные получатели сообщение о приглашении должно быть отправлено. В настоящее время поддерживается только один дополнительный получатель.|
|кустомизедмессажебоди|String|Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.|
|мессажелангуаже|String|Язык, по которому необходимо отправить сообщение по умолчанию. Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди. Языковой формат должен быть в стандарте ISO 639. Значение по умолчанию — en-US.|

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
