---
title: Тип ресурса externalItemContent
description: Содержимое элемента, индексироваться через подключение Поиска (Майкрософт).
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 66e3fccc8c072d06d2328301100d6bf3a0d50806
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777633"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="7d364-103">Тип ресурса externalItemContent</span><span class="sxs-lookup"><span data-stu-id="7d364-103">externalItemContent resource type</span></span>

<span data-ttu-id="7d364-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d364-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d364-105">Содержимое [externalItem, индексироваться](externalitem.md) через подключение Поиска (Майкрософт). [](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7d364-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="7d364-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d364-106">Properties</span></span>

| <span data-ttu-id="7d364-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d364-107">Property</span></span> | <span data-ttu-id="7d364-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d364-108">Type</span></span>   | <span data-ttu-id="7d364-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d364-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="7d364-110">значение</span><span class="sxs-lookup"><span data-stu-id="7d364-110">value</span></span>    | <span data-ttu-id="7d364-111">String</span><span class="sxs-lookup"><span data-stu-id="7d364-111">String</span></span> | <span data-ttu-id="7d364-112">Содержимое для externalItem.</span><span class="sxs-lookup"><span data-stu-id="7d364-112">The content for the externalItem.</span></span> <span data-ttu-id="7d364-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="7d364-113">Required.</span></span>                                                 |
| <span data-ttu-id="7d364-114">type</span><span class="sxs-lookup"><span data-stu-id="7d364-114">type</span></span>     | <span data-ttu-id="7d364-115">String</span><span class="sxs-lookup"><span data-stu-id="7d364-115">String</span></span> | <span data-ttu-id="7d364-116">Тип контента в свойстве value.</span><span class="sxs-lookup"><span data-stu-id="7d364-116">The type of content in the value property.</span></span> <span data-ttu-id="7d364-117">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="7d364-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="7d364-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d364-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7d364-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7d364-119">Relationships</span></span>

<span data-ttu-id="7d364-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7d364-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d364-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d364-121">JSON representation</span></span>

<span data-ttu-id="7d364-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d364-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
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


