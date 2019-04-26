---
title: Тип ресурса Планнерпланконтекстдетаилсколлектион
description: " значение — объект Планнерпланконтекстдетаилс."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571859"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>Тип ресурса Планнерпланконтекстдетаилсколлектион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Ресурс **планнерпланконтекстдетаилсколлектион** представляет коллекцию внешних контекстов, с которыми связан план. Этот ресурс является открытым типом и является частью объекта [plannerPlanDetails](plannerplandetails.md) . Имя свойства в аргументе "свойство-значение" — это идентификатор контекста, зависящий от приложения; значение — объект [планнерпланконтекстдетаилс](plannerplancontextdetails.md) .


## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен использовать отличительный идентификатор, представляющий внешний контекст в качестве имени свойства. Значения свойств должны быть [планнерпланконтекстдетаилс](plannerplancontextdetails.md) объектами. На основе OData имена свойств в открытых типах не могут содержать следующие символы `.`:, `:`, `@`,. `%` Эти символы необходимо закодировать с помощью формата кодирования URL-адресов. Чтобы удалить элемент из списка "Избранное", необходимо удалить его из коллекции [планнерпланконтекстколлектион](plannerplancontextcollection.md) , что приведет к автоматическому удалению записи в этом объекте.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
