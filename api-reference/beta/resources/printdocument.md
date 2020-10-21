---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 34f35181e9d1ba70c2efe8df31d6d6457aa0acde
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635140"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="6f2e2-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="6f2e2-103">printDocument resource type</span></span>

<span data-ttu-id="6f2e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f2e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f2e2-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="6f2e2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6f2e2-106">Methods</span></span>

| <span data-ttu-id="6f2e2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6f2e2-107">Method</span></span>       | <span data-ttu-id="6f2e2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f2e2-108">Return Type</span></span> | <span data-ttu-id="6f2e2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2e2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6f2e2-110">уплоаддата</span><span class="sxs-lookup"><span data-stu-id="6f2e2-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="6f2e2-111">Нет</span><span class="sxs-lookup"><span data-stu-id="6f2e2-111">None</span></span> | <span data-ttu-id="6f2e2-112">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-112">Upload a single binary segment of the **printDocument**.</span></span> |
| [<span data-ttu-id="6f2e2-113">Скачать двоичный файл</span><span class="sxs-lookup"><span data-stu-id="6f2e2-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="6f2e2-114">URL-адрес скачивания</span><span class="sxs-lookup"><span data-stu-id="6f2e2-114">Download Url</span></span> | <span data-ttu-id="6f2e2-115">Скачайте двоичный файл, связанный с классом **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f2e2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f2e2-116">Properties</span></span>
| <span data-ttu-id="6f2e2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f2e2-117">Property</span></span>     | <span data-ttu-id="6f2e2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2e2-118">Type</span></span>        | <span data-ttu-id="6f2e2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2e2-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f2e2-120">id</span><span class="sxs-lookup"><span data-stu-id="6f2e2-120">id</span></span>|<span data-ttu-id="6f2e2-121">String</span><span class="sxs-lookup"><span data-stu-id="6f2e2-121">String</span></span>|<span data-ttu-id="6f2e2-122">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-122">The document's identifier.</span></span> <span data-ttu-id="6f2e2-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-123">Read-only.</span></span>|
|<span data-ttu-id="6f2e2-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6f2e2-124">displayName</span></span>|<span data-ttu-id="6f2e2-125">String</span><span class="sxs-lookup"><span data-stu-id="6f2e2-125">String</span></span>|<span data-ttu-id="6f2e2-126">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-126">The document's name.</span></span> <span data-ttu-id="6f2e2-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-127">Read-only.</span></span>|
|<span data-ttu-id="6f2e2-128">contentType</span><span class="sxs-lookup"><span data-stu-id="6f2e2-128">contentType</span></span>|<span data-ttu-id="6f2e2-129">String</span><span class="sxs-lookup"><span data-stu-id="6f2e2-129">String</span></span>|<span data-ttu-id="6f2e2-130">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="6f2e2-130">The document's content (MIME) type.</span></span> <span data-ttu-id="6f2e2-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-131">Read-only.</span></span>|
|<span data-ttu-id="6f2e2-132">size</span><span class="sxs-lookup"><span data-stu-id="6f2e2-132">size</span></span>|<span data-ttu-id="6f2e2-133">Int64</span><span class="sxs-lookup"><span data-stu-id="6f2e2-133">Int64</span></span>|<span data-ttu-id="6f2e2-134">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-134">The document's size in bytes.</span></span> <span data-ttu-id="6f2e2-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-135">Read-only.</span></span>|
|<span data-ttu-id="6f2e2-136">configuration</span><span class="sxs-lookup"><span data-stu-id="6f2e2-136">configuration</span></span>|[<span data-ttu-id="6f2e2-137">принтердокументконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6f2e2-137">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="6f2e2-138">Группа параметров, которые принтер должен использовать для печати документа.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-138">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="6f2e2-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f2e2-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f2e2-140">JSON representation</span></span>

<span data-ttu-id="6f2e2-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f2e2-141">The following is a JSON representation of the resource.</span></span>

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
    "colorConfiguration": "String"
  }
}

```


