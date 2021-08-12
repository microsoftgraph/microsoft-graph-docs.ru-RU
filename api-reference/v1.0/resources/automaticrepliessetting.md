---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации, чтобы автоматически уведомить отправитель входящего сообщения электронной почты с сообщением из '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7e92dca6390e539a73d42bf27d248d5e9c90d38b281246278714246679584071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147037"
---
# <a name="automaticrepliessetting-resource-type"></a>Тип ресурса automaticRepliesSetting

Пространство имен: microsoft.graph

Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|externalAudience|externalAudienceScope| Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. Допустимые значения: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|string|Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.|
|internalReplyMessage|string|Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.|
|status|automaticRepliesStatus|Состояние настройки автоматических ответов. Допустимые значения: `disabled`, `alwaysEnabled`, `scheduled`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

