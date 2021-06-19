---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: michaelcurnutt
ms.openlocfilehash: 0f2f069cbbff191cefcdc8b735b2847b48a8f2ed
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030784"
---
# <a name="licenseunitsdetail-resource-type"></a>Тип ресурса licenseUnitsDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**. Дополнительные сведения о состояниях прогрессии подписки см. в журнале [What if my subscription expires?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-------------|:-----|:----------|
|enabled|Int32| Количество единиц, включенных для активной подписки службы SKU. |
|suspended|Int32| Количество единиц, которые приостановлены из-за отмены подписки на службу SKU. Эти блоки не могут быть назначены, но могут быть повторно активированы перед удалением. |
|warning|Int32| Количество единиц, которые находятся в состоянии предупреждения. По истечении срока действия подписки на службу SKU у клиента есть льготный период для продления подписки до ее отмены (перенесенной в **приостановленное** состояние). |

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


