---
title: Тип ресурса plannerPlanContextDetailsCollection
description: " значение — это объект plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 0020ff8e8fd0d2e8dfd783e282e2bd648c16ec6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828240"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>Тип ресурса plannerPlanContextDetailsCollection

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.


Ресурс **plannerPlanContextDetailsCollection** представляет коллекцию внешних контекстах, с которыми связан плана. Этот ресурс является открытым и является частью объекта [plannerPlanDetails](plannerplandetails.md) . Имя свойства в паре значение свойства — это идентификатор приложения определенного контекста; значение — это объект [plannerPlanContextDetails](plannerplancontextdetails.md) .


## <a name="properties"></a>Свойства
Свойства открытого типа может быть определен клиентом. В этом случае клиент должен использовать особый идентификатор, представляющий внешнего контекста как имя свойства. Значения свойства должны быть [plannerPlanContextDetails](plannerplancontextdetails.md) объектов. На основании OData, имена свойств в открытые типы не может содержать следующие символы: `.`, `:`, `@`, `%`. Эти символы должны кодируются с помощью кодировки формат URL-адреса. Удаление элемента из списка "Избранное", значение должно быть удален из коллекции [plannerPlanContextCollection](plannerplancontextcollection.md) вместо этого которого будет автоматически удалять запись в этот объект.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
