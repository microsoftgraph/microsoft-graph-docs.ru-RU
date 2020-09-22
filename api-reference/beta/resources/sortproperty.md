---
title: Тип ресурса Сортпроперти
description: Предоставляет возможность сортировки результатов поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f1288b2dc9ec05fe8aaedb5871c3bda68714f90
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193972"
---
# <a name="sortproperty-resource-type"></a><span data-ttu-id="cb726-103">Тип ресурса Сортпроперти</span><span class="sxs-lookup"><span data-stu-id="cb726-103">sortProperty resource type</span></span>

<span data-ttu-id="cb726-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb726-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb726-105">Представляет параметры сортировки для упорядочивания результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="cb726-105">Represents the sort options to order search results.</span></span>

## <a name="properties"></a><span data-ttu-id="cb726-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb726-106">Properties</span></span>

| <span data-ttu-id="cb726-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb726-107">Property</span></span>     | <span data-ttu-id="cb726-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb726-108">Type</span></span>        | <span data-ttu-id="cb726-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb726-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb726-110">name</span><span class="sxs-lookup"><span data-stu-id="cb726-110">name</span></span>|<span data-ttu-id="cb726-111">String</span><span class="sxs-lookup"><span data-stu-id="cb726-111">String</span></span>|<span data-ttu-id="cb726-112">Имя свойства, по которому выполняется сортировка.</span><span class="sxs-lookup"><span data-stu-id="cb726-112">The name of the property to sort on.</span></span> <span data-ttu-id="cb726-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cb726-113">Required.</span></span>|
|<span data-ttu-id="cb726-114">по убыванию</span><span class="sxs-lookup"><span data-stu-id="cb726-114">isDescending</span></span>|<span data-ttu-id="cb726-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="cb726-115">Boolean</span></span>|<span data-ttu-id="cb726-116">`True` Если порядок сортировки — по убыванию.</span><span class="sxs-lookup"><span data-stu-id="cb726-116">`True` if the sort order is descending.</span></span> <span data-ttu-id="cb726-117">По умолчанию используется `false` порядок сортировки по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="cb726-117">Default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="cb726-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cb726-118">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb726-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb726-119">JSON representation</span></span>

<span data-ttu-id="cb726-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb726-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortProperty",
  "baseType": null
}-->

```json
{
  "name": "String",
  "isDescending": "true"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->