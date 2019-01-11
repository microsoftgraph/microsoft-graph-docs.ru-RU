---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807513"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="3c24d-102">Тип ресурса incompleteData</span><span class="sxs-lookup"><span data-stu-id="3c24d-102">incompleteData resource type</span></span>

 > <span data-ttu-id="3c24d-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c24d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c24d-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c24d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c24d-105">Аспекта **incompleteData** указывает, что ресурс был создан с помощью неполные данные.</span><span class="sxs-lookup"><span data-stu-id="3c24d-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="3c24d-106">Свойства в можно указать сведения о, поэтому неполные данные.</span><span class="sxs-lookup"><span data-stu-id="3c24d-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c24d-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c24d-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="3c24d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c24d-108">Properties</span></span>

| <span data-ttu-id="3c24d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c24d-109">Property</span></span>                  | <span data-ttu-id="3c24d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3c24d-110">Type</span></span>           | <span data-ttu-id="3c24d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c24d-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="3c24d-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="3c24d-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="3c24d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c24d-113">DateTimeOffset</span></span> | <span data-ttu-id="3c24d-114">Служба не имеет источника данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="3c24d-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="3c24d-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="3c24d-115">wasThrottled</span></span>              | <span data-ttu-id="3c24d-116">Логический</span><span class="sxs-lookup"><span data-stu-id="3c24d-116">Boolean</span></span>        | <span data-ttu-id="3c24d-117">Не удалось записать часть данных из-за высокой активности.</span><span class="sxs-lookup"><span data-stu-id="3c24d-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
