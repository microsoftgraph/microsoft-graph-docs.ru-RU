---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1e7a1d6a9c131417e4f0ef171ac364e5fe8b106b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863784"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="7d9cc-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="7d9cc-103">printDocument resource type</span></span>

<span data-ttu-id="7d9cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d9cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d9cc-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="7d9cc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7d9cc-106">Methods</span></span>

| <span data-ttu-id="7d9cc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7d9cc-107">Method</span></span>       | <span data-ttu-id="7d9cc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7d9cc-108">Return Type</span></span> | <span data-ttu-id="7d9cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9cc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7d9cc-110">уплоаддата</span><span class="sxs-lookup"><span data-stu-id="7d9cc-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="7d9cc-111">Нет</span><span class="sxs-lookup"><span data-stu-id="7d9cc-111">None</span></span> | <span data-ttu-id="7d9cc-112">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d9cc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d9cc-113">Properties</span></span>
| <span data-ttu-id="7d9cc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d9cc-114">Property</span></span>     | <span data-ttu-id="7d9cc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="7d9cc-115">Type</span></span>        | <span data-ttu-id="7d9cc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9cc-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d9cc-117">id</span><span class="sxs-lookup"><span data-stu-id="7d9cc-117">id</span></span>|<span data-ttu-id="7d9cc-118">String</span><span class="sxs-lookup"><span data-stu-id="7d9cc-118">String</span></span>|<span data-ttu-id="7d9cc-119">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-119">The document's identifier.</span></span> <span data-ttu-id="7d9cc-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-120">Read-only.</span></span>|
|<span data-ttu-id="7d9cc-121">displayName</span><span class="sxs-lookup"><span data-stu-id="7d9cc-121">displayName</span></span>|<span data-ttu-id="7d9cc-122">Строка</span><span class="sxs-lookup"><span data-stu-id="7d9cc-122">String</span></span>|<span data-ttu-id="7d9cc-123">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-123">The document's name.</span></span> <span data-ttu-id="7d9cc-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-124">Read-only.</span></span>|
|<span data-ttu-id="7d9cc-125">contentType</span><span class="sxs-lookup"><span data-stu-id="7d9cc-125">contentType</span></span>|<span data-ttu-id="7d9cc-126">String</span><span class="sxs-lookup"><span data-stu-id="7d9cc-126">String</span></span>|<span data-ttu-id="7d9cc-127">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="7d9cc-127">The document's content (MIME) type.</span></span> <span data-ttu-id="7d9cc-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-128">Read-only.</span></span>|
|<span data-ttu-id="7d9cc-129">size</span><span class="sxs-lookup"><span data-stu-id="7d9cc-129">size</span></span>|<span data-ttu-id="7d9cc-130">Int64</span><span class="sxs-lookup"><span data-stu-id="7d9cc-130">Int64</span></span>|<span data-ttu-id="7d9cc-131">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-131">The document's size in bytes.</span></span> <span data-ttu-id="7d9cc-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-132">Read-only.</span></span>|
|<span data-ttu-id="7d9cc-133">configuration</span><span class="sxs-lookup"><span data-stu-id="7d9cc-133">configuration</span></span>|[<span data-ttu-id="7d9cc-134">принтердокументконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7d9cc-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="7d9cc-135">Группа параметров, которые принтер должен использовать для печати документа.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="7d9cc-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d9cc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d9cc-137">JSON representation</span></span>

<span data-ttu-id="7d9cc-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d9cc-138">The following is a JSON representation of the resource.</span></span>

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
