---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: e2502421f6976da3378909fd157280296a7550e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046764"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="92edf-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="92edf-103">printDocument resource type</span></span>

<span data-ttu-id="92edf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92edf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92edf-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="92edf-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="92edf-106">Методы</span><span class="sxs-lookup"><span data-stu-id="92edf-106">Methods</span></span>

| <span data-ttu-id="92edf-107">Метод</span><span class="sxs-lookup"><span data-stu-id="92edf-107">Method</span></span>       | <span data-ttu-id="92edf-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92edf-108">Return Type</span></span> | <span data-ttu-id="92edf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="92edf-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="92edf-110">уплоаддата</span><span class="sxs-lookup"><span data-stu-id="92edf-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="92edf-111">Нет</span><span class="sxs-lookup"><span data-stu-id="92edf-111">None</span></span> | <span data-ttu-id="92edf-112">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="92edf-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="92edf-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="92edf-113">Properties</span></span>
| <span data-ttu-id="92edf-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="92edf-114">Property</span></span>     | <span data-ttu-id="92edf-115">Тип</span><span class="sxs-lookup"><span data-stu-id="92edf-115">Type</span></span>        | <span data-ttu-id="92edf-116">Описание</span><span class="sxs-lookup"><span data-stu-id="92edf-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92edf-117">id</span><span class="sxs-lookup"><span data-stu-id="92edf-117">id</span></span>|<span data-ttu-id="92edf-118">String</span><span class="sxs-lookup"><span data-stu-id="92edf-118">String</span></span>|<span data-ttu-id="92edf-119">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="92edf-119">The document's identifier.</span></span> <span data-ttu-id="92edf-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92edf-120">Read-only.</span></span>|
|<span data-ttu-id="92edf-121">displayName</span><span class="sxs-lookup"><span data-stu-id="92edf-121">displayName</span></span>|<span data-ttu-id="92edf-122">String</span><span class="sxs-lookup"><span data-stu-id="92edf-122">String</span></span>|<span data-ttu-id="92edf-123">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="92edf-123">The document's name.</span></span> <span data-ttu-id="92edf-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92edf-124">Read-only.</span></span>|
|<span data-ttu-id="92edf-125">contentType</span><span class="sxs-lookup"><span data-stu-id="92edf-125">contentType</span></span>|<span data-ttu-id="92edf-126">String</span><span class="sxs-lookup"><span data-stu-id="92edf-126">String</span></span>|<span data-ttu-id="92edf-127">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="92edf-127">The document's content (MIME) type.</span></span> <span data-ttu-id="92edf-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92edf-128">Read-only.</span></span>|
|<span data-ttu-id="92edf-129">size</span><span class="sxs-lookup"><span data-stu-id="92edf-129">size</span></span>|<span data-ttu-id="92edf-130">Int64</span><span class="sxs-lookup"><span data-stu-id="92edf-130">Int64</span></span>|<span data-ttu-id="92edf-131">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="92edf-131">The document's size in bytes.</span></span> <span data-ttu-id="92edf-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92edf-132">Read-only.</span></span>|
|<span data-ttu-id="92edf-133">configuration</span><span class="sxs-lookup"><span data-stu-id="92edf-133">configuration</span></span>|[<span data-ttu-id="92edf-134">принтердокументконфигуратион</span><span class="sxs-lookup"><span data-stu-id="92edf-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="92edf-135">Группа параметров, которые принтер должен использовать для печати документа.</span><span class="sxs-lookup"><span data-stu-id="92edf-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="92edf-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92edf-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92edf-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92edf-137">JSON representation</span></span>

<span data-ttu-id="92edf-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92edf-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": 12345,
  "documentConfiguration": {
    "pageRanges": [ {"@odata.type": "microsoft.graph.printPageRange"} ],
    "printQuality": "String",
    "printResolutionInDpi": 123456,
    "feedDirection": "String",
    "orientation": "String",
    "duplexConfiguration": "String",
    "copies": 123456,
    "colorConfiguration": "String",
  }
}

```


