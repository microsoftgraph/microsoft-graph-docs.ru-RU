---
title: Тип ресурса Екстерналитемконтент
description: Содержимое элемента, индексируемого с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a9121648f35dd09d8fb87d4738bb2bf6e9b3960b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998812"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="311cf-103">Тип ресурса Екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="311cf-103">externalItemContent resource type</span></span>

<span data-ttu-id="311cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="311cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="311cf-105">Содержимое объекта [екстерналитем](externalitem.md) , индексируемого с помощью [подключения](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="311cf-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="311cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="311cf-106">Properties</span></span>

| <span data-ttu-id="311cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="311cf-107">Property</span></span> | <span data-ttu-id="311cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="311cf-108">Type</span></span>   | <span data-ttu-id="311cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="311cf-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="311cf-110">значение</span><span class="sxs-lookup"><span data-stu-id="311cf-110">value</span></span>    | <span data-ttu-id="311cf-111">String</span><span class="sxs-lookup"><span data-stu-id="311cf-111">String</span></span> | <span data-ttu-id="311cf-112">Содержимое для Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="311cf-112">The content for the externalItem.</span></span> <span data-ttu-id="311cf-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="311cf-113">Required.</span></span>                                                 |
| <span data-ttu-id="311cf-114">type</span><span class="sxs-lookup"><span data-stu-id="311cf-114">type</span></span>     | <span data-ttu-id="311cf-115">String</span><span class="sxs-lookup"><span data-stu-id="311cf-115">String</span></span> | <span data-ttu-id="311cf-116">Тип контента в свойстве Value.</span><span class="sxs-lookup"><span data-stu-id="311cf-116">The type of content in the value property.</span></span> <span data-ttu-id="311cf-117">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="311cf-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="311cf-118">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="311cf-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="311cf-119">Связи</span><span class="sxs-lookup"><span data-stu-id="311cf-119">Relationships</span></span>

<span data-ttu-id="311cf-120">Нет</span><span class="sxs-lookup"><span data-stu-id="311cf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="311cf-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="311cf-121">JSON representation</span></span>

<span data-ttu-id="311cf-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="311cf-122">The following is a JSON representation of the resource.</span></span>

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


