---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2a981fbdf7e1126783ae97d93c20e3ec08b1f2f0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896086"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="3fc74-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="3fc74-103">printDocument resource type</span></span>

<span data-ttu-id="3fc74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fc74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fc74-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="3fc74-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="3fc74-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3fc74-106">Methods</span></span>

| <span data-ttu-id="3fc74-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3fc74-107">Method</span></span>       | <span data-ttu-id="3fc74-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3fc74-108">Return Type</span></span> | <span data-ttu-id="3fc74-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc74-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3fc74-110">уплоаддата</span><span class="sxs-lookup"><span data-stu-id="3fc74-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="3fc74-111">Нет</span><span class="sxs-lookup"><span data-stu-id="3fc74-111">None</span></span> | <span data-ttu-id="3fc74-112">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="3fc74-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="3fc74-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fc74-113">Properties</span></span>
| <span data-ttu-id="3fc74-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fc74-114">Property</span></span>     | <span data-ttu-id="3fc74-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3fc74-115">Type</span></span>        | <span data-ttu-id="3fc74-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc74-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fc74-117">id</span><span class="sxs-lookup"><span data-stu-id="3fc74-117">id</span></span>|<span data-ttu-id="3fc74-118">Строка</span><span class="sxs-lookup"><span data-stu-id="3fc74-118">String</span></span>|<span data-ttu-id="3fc74-119">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="3fc74-119">The document's identifier.</span></span> <span data-ttu-id="3fc74-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc74-120">Read-only.</span></span>|
|<span data-ttu-id="3fc74-121">name</span><span class="sxs-lookup"><span data-stu-id="3fc74-121">name</span></span>|<span data-ttu-id="3fc74-122">String</span><span class="sxs-lookup"><span data-stu-id="3fc74-122">String</span></span>|<span data-ttu-id="3fc74-123">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="3fc74-123">The document's name.</span></span> <span data-ttu-id="3fc74-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc74-124">Read-only.</span></span>|
|<span data-ttu-id="3fc74-125">mimeType</span><span class="sxs-lookup"><span data-stu-id="3fc74-125">mimeType</span></span>|<span data-ttu-id="3fc74-126">String</span><span class="sxs-lookup"><span data-stu-id="3fc74-126">String</span></span>|<span data-ttu-id="3fc74-127">Тип MIME документа.</span><span class="sxs-lookup"><span data-stu-id="3fc74-127">The document's MIME type.</span></span> <span data-ttu-id="3fc74-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc74-128">Read-only.</span></span>|
|<span data-ttu-id="3fc74-129">сизеинбитес</span><span class="sxs-lookup"><span data-stu-id="3fc74-129">sizeInBytes</span></span>|<span data-ttu-id="3fc74-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3fc74-130">Int64</span></span>|<span data-ttu-id="3fc74-131">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="3fc74-131">The document's size in bytes.</span></span> <span data-ttu-id="3fc74-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc74-132">Read-only.</span></span>|
|<span data-ttu-id="3fc74-133">документконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3fc74-133">documentConfiguration</span></span>|[<span data-ttu-id="3fc74-134">принтердокументконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3fc74-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="3fc74-135">Группа параметров, которые принтер должен использовать для печати документа.</span><span class="sxs-lookup"><span data-stu-id="3fc74-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="3fc74-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc74-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fc74-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fc74-137">JSON representation</span></span>

<span data-ttu-id="3fc74-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fc74-138">The following is a JSON representation of the resource.</span></span>

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
