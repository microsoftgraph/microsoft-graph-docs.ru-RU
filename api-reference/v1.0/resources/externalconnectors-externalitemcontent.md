---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4dd853ca32c918988f2f99e1f1238d9ac937da02
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467454"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="90f32-103">тип ресурса externalItemContent</span><span class="sxs-lookup"><span data-stu-id="90f32-103">externalItemContent resource type</span></span>

<span data-ttu-id="90f32-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="90f32-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="90f32-105">Содержимое [externalItem,](externalconnectors-externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="90f32-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90f32-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="90f32-106">Properties</span></span>
|<span data-ttu-id="90f32-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="90f32-107">Property</span></span>|<span data-ttu-id="90f32-108">Тип</span><span class="sxs-lookup"><span data-stu-id="90f32-108">Type</span></span>|<span data-ttu-id="90f32-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90f32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90f32-110">type</span><span class="sxs-lookup"><span data-stu-id="90f32-110">type</span></span>|<span data-ttu-id="90f32-111">microsoft.graph.externalConnectors.externalItemContentType</span><span class="sxs-lookup"><span data-stu-id="90f32-111">microsoft.graph.externalConnectors.externalItemContentType</span></span>|<span data-ttu-id="90f32-112">Тип контента в свойстве значения.</span><span class="sxs-lookup"><span data-stu-id="90f32-112">The type of content in the value property.</span></span> <span data-ttu-id="90f32-113">Возможные значения: `text`, `html`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="90f32-113">Possible values are: `text`, `html`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="90f32-114">value</span><span class="sxs-lookup"><span data-stu-id="90f32-114">value</span></span>|<span data-ttu-id="90f32-115">String</span><span class="sxs-lookup"><span data-stu-id="90f32-115">String</span></span>|<span data-ttu-id="90f32-116">Содержимое для externalItem.</span><span class="sxs-lookup"><span data-stu-id="90f32-116">The content for the externalItem.</span></span> <span data-ttu-id="90f32-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90f32-117">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90f32-118">Связи</span><span class="sxs-lookup"><span data-stu-id="90f32-118">Relationships</span></span>
<span data-ttu-id="90f32-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="90f32-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90f32-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90f32-120">JSON representation</span></span>
<span data-ttu-id="90f32-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90f32-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

