---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 036b2e2d4081160680b7f5471bd2707ee503bc4a
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366543"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="45853-103">тип ресурса externalItemContent</span><span class="sxs-lookup"><span data-stu-id="45853-103">externalItemContent resource type</span></span>

<span data-ttu-id="45853-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45853-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45853-105">Содержимое [externalItem,](externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="45853-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45853-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="45853-106">Properties</span></span>

| <span data-ttu-id="45853-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="45853-107">Property</span></span> | <span data-ttu-id="45853-108">Тип</span><span class="sxs-lookup"><span data-stu-id="45853-108">Type</span></span>   | <span data-ttu-id="45853-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45853-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="45853-110">значение</span><span class="sxs-lookup"><span data-stu-id="45853-110">value</span></span>    | <span data-ttu-id="45853-111">String</span><span class="sxs-lookup"><span data-stu-id="45853-111">String</span></span> | <span data-ttu-id="45853-112">Содержимое для externalItem.</span><span class="sxs-lookup"><span data-stu-id="45853-112">The content for the externalItem.</span></span> <span data-ttu-id="45853-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="45853-113">Required.</span></span>                                                 |
| <span data-ttu-id="45853-114">type</span><span class="sxs-lookup"><span data-stu-id="45853-114">type</span></span>     | <span data-ttu-id="45853-115">String</span><span class="sxs-lookup"><span data-stu-id="45853-115">String</span></span> | <span data-ttu-id="45853-116">Тип контента в свойстве значения.</span><span class="sxs-lookup"><span data-stu-id="45853-116">The type of content in the value property.</span></span> <span data-ttu-id="45853-117">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="45853-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="45853-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45853-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="45853-119">Связи</span><span class="sxs-lookup"><span data-stu-id="45853-119">Relationships</span></span>

<span data-ttu-id="45853-120">Нет</span><span class="sxs-lookup"><span data-stu-id="45853-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45853-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45853-121">JSON representation</span></span>

<span data-ttu-id="45853-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45853-122">The following is a JSON representation of the resource.</span></span>

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


