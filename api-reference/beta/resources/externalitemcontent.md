---
title: Тип ресурса Екстерналитемконтент
description: Содержимое элемента, индексируемого с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db0276307e824faa0c5606a8fb1212a0ad25e654
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805662"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="1868b-103">Тип ресурса Екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="1868b-103">externalItemContent resource type</span></span>

<span data-ttu-id="1868b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1868b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1868b-105">Содержимое объекта [екстерналитем](externalitem.md) , индексируемого с помощью [подключения](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="1868b-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="1868b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1868b-106">Properties</span></span>

| <span data-ttu-id="1868b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1868b-107">Property</span></span> | <span data-ttu-id="1868b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1868b-108">Type</span></span>   | <span data-ttu-id="1868b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1868b-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="1868b-110">значение</span><span class="sxs-lookup"><span data-stu-id="1868b-110">value</span></span>    | <span data-ttu-id="1868b-111">String</span><span class="sxs-lookup"><span data-stu-id="1868b-111">String</span></span> | <span data-ttu-id="1868b-112">Содержимое для Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="1868b-112">The content for the externalItem.</span></span> <span data-ttu-id="1868b-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="1868b-113">Required.</span></span>                                                 |
| <span data-ttu-id="1868b-114">type</span><span class="sxs-lookup"><span data-stu-id="1868b-114">type</span></span>     | <span data-ttu-id="1868b-115">String</span><span class="sxs-lookup"><span data-stu-id="1868b-115">String</span></span> | <span data-ttu-id="1868b-116">Тип контента в свойстве Value.</span><span class="sxs-lookup"><span data-stu-id="1868b-116">The type of content in the value property.</span></span> <span data-ttu-id="1868b-117">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="1868b-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="1868b-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1868b-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1868b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="1868b-119">Relationships</span></span>

<span data-ttu-id="1868b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1868b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1868b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1868b-121">JSON representation</span></span>

<span data-ttu-id="1868b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1868b-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent",
  "baseType": ""
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
