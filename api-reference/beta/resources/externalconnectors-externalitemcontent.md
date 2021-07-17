---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d895d0056da71ea065dbc62d08c9deda054a6f29
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467855"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="40ee8-103">тип ресурса externalItemContent</span><span class="sxs-lookup"><span data-stu-id="40ee8-103">externalItemContent resource type</span></span>

<span data-ttu-id="40ee8-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="40ee8-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ee8-105">Содержимое [externalItem,](externalconnectors-externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="40ee8-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="40ee8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="40ee8-106">Properties</span></span>

| <span data-ttu-id="40ee8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="40ee8-107">Property</span></span> | <span data-ttu-id="40ee8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="40ee8-108">Type</span></span>   | <span data-ttu-id="40ee8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40ee8-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="40ee8-110">значение</span><span class="sxs-lookup"><span data-stu-id="40ee8-110">value</span></span>    | <span data-ttu-id="40ee8-111">String</span><span class="sxs-lookup"><span data-stu-id="40ee8-111">String</span></span> | <span data-ttu-id="40ee8-112">Содержимое для externalItem.</span><span class="sxs-lookup"><span data-stu-id="40ee8-112">The content for the externalItem.</span></span> <span data-ttu-id="40ee8-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="40ee8-113">Required.</span></span>                                                 |
| <span data-ttu-id="40ee8-114">type</span><span class="sxs-lookup"><span data-stu-id="40ee8-114">type</span></span>     | <span data-ttu-id="40ee8-115">String</span><span class="sxs-lookup"><span data-stu-id="40ee8-115">String</span></span> | <span data-ttu-id="40ee8-116">Тип контента в свойстве значения.</span><span class="sxs-lookup"><span data-stu-id="40ee8-116">The type of content in the value property.</span></span> <span data-ttu-id="40ee8-117">Возможные значения: `text` и `html`.</span><span class="sxs-lookup"><span data-stu-id="40ee8-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="40ee8-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ee8-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="40ee8-119">Связи</span><span class="sxs-lookup"><span data-stu-id="40ee8-119">Relationships</span></span>

<span data-ttu-id="40ee8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="40ee8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40ee8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40ee8-121">JSON representation</span></span>

<span data-ttu-id="40ee8-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40ee8-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
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