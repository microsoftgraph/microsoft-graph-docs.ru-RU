---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
ms.localizationpriority: medium
author: jconley76
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6a321eeb77b011730ec99b76112bd441862e72d2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900403"
---
# <a name="licenseunitsdetail-resource-type"></a>Тип ресурса licenseUnitsDetail

Пространство имен: microsoft.graph

Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**. Дополнительные сведения о состоянии хода выполнения подписки см. в разделе "Что делать, [если срок действия подписки истекает?".](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide&preserve-view=true)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-------------|:-----|:----------|
|enabled|Int32| Количество единиц, включенных для активной подписки SKU службы.  |
|suspended|Int32| Количество единиц, приостановленных из-за отмены подписки на номер SKU службы. Единицы не могут быть назначены, но по-прежнему могут быть повторно активированы до их удаления. |
|warning|Int32| Количество единиц, которые находятся в состоянии предупреждения. По истечении срока действия подписки на номер SKU службы у клиента есть льготный период для продления подписки до ее отмены (перемещены в **приостановленное** состояние).  |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

