---
title: Тип ресурса Планнерпланконтекстдетаилсколлектион
description: " значение — объект Планнерпланконтекстдетаилс."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 2e2f292de763674510f6da5a8aad90fe8e17ab7f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344402"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>Тип ресурса Планнерпланконтекстдетаилсколлектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Ресурс **планнерпланконтекстдетаилсколлектион** представляет коллекцию внешних контекстов, с которыми связан план. Этот ресурс является открытым типом и является частью объекта [plannerPlanDetails](plannerplandetails.md) . Имя свойства в аргументе "свойство-значение" — это идентификатор контекста, зависящий от приложения; значение — объект [планнерпланконтекстдетаилс](plannerplancontextdetails.md) .


## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен использовать отличительный идентификатор, представляющий внешний контекст в качестве имени свойства. Значения свойств должны быть [планнерпланконтекстдетаилс](plannerplancontextdetails.md) объектами. На основе OData имена свойств в открытых типах не могут содержать следующие символы `.`:, `:`, `@`,. `%` Эти символы необходимо закодировать с помощью формата кодирования URL-адресов. Чтобы удалить элемент из списка "Избранное", необходимо удалить его из коллекции [планнерпланконтекстколлектион](plannerplancontextcollection.md) , что приведет к автоматическому удалению записи в этом объекте.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
