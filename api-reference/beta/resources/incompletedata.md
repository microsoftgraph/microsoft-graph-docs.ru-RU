---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075852"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="90462-102">Тип ресурса incompleteData</span><span class="sxs-lookup"><span data-stu-id="90462-102">incompleteData resource type</span></span>

 > <span data-ttu-id="90462-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90462-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90462-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90462-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90462-105">Аспекта **incompleteData** указывает, что ресурс был создан с помощью неполные данные.</span><span class="sxs-lookup"><span data-stu-id="90462-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="90462-106">Свойства в можно указать сведения о, поэтому неполные данные.</span><span class="sxs-lookup"><span data-stu-id="90462-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90462-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90462-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="90462-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="90462-108">Properties</span></span>

| <span data-ttu-id="90462-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="90462-109">Property</span></span>                  | <span data-ttu-id="90462-110">Тип</span><span class="sxs-lookup"><span data-stu-id="90462-110">Type</span></span>           | <span data-ttu-id="90462-111">Описание</span><span class="sxs-lookup"><span data-stu-id="90462-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="90462-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="90462-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="90462-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90462-113">DateTimeOffset</span></span> | <span data-ttu-id="90462-114">Служба не имеет источника данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="90462-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="90462-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="90462-115">wasThrottled</span></span>              | <span data-ttu-id="90462-116">Логический</span><span class="sxs-lookup"><span data-stu-id="90462-116">Boolean</span></span>        | <span data-ttu-id="90462-117">Не удалось записать часть данных из-за высокой активности.</span><span class="sxs-lookup"><span data-stu-id="90462-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
