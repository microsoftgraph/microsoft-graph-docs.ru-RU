---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 102cf81f0770f02b1206bff1fa927121696047c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727978"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="d9c76-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="d9c76-103">printDocument resource type</span></span>

<span data-ttu-id="d9c76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9c76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9c76-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="d9c76-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="d9c76-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d9c76-106">Methods</span></span>

| <span data-ttu-id="d9c76-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d9c76-107">Method</span></span>       | <span data-ttu-id="d9c76-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9c76-108">Return Type</span></span> | <span data-ttu-id="d9c76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9c76-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d9c76-110">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="d9c76-110">Create upload session</span></span>](../api/printdocument-get-file.md) | [<span data-ttu-id="d9c76-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="d9c76-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="d9c76-112">Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="d9c76-112">Create an upload session to iteratively upload ranges of binary file of **printDocument**.</span></span> |
| [<span data-ttu-id="d9c76-113">Скачать двоичный файл</span><span class="sxs-lookup"><span data-stu-id="d9c76-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="d9c76-114">URL-адрес скачивания</span><span class="sxs-lookup"><span data-stu-id="d9c76-114">Download Url</span></span> | <span data-ttu-id="d9c76-115">Скачайте двоичный файл, связанный с классом **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="d9c76-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="d9c76-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9c76-116">Properties</span></span>
| <span data-ttu-id="d9c76-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9c76-117">Property</span></span>     | <span data-ttu-id="d9c76-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d9c76-118">Type</span></span>        | <span data-ttu-id="d9c76-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d9c76-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9c76-120">id</span><span class="sxs-lookup"><span data-stu-id="d9c76-120">id</span></span>|<span data-ttu-id="d9c76-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d9c76-121">String</span></span>|<span data-ttu-id="d9c76-122">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="d9c76-122">The document's identifier.</span></span> <span data-ttu-id="d9c76-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c76-123">Read-only.</span></span>|
|<span data-ttu-id="d9c76-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d9c76-124">displayName</span></span>|<span data-ttu-id="d9c76-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d9c76-125">String</span></span>|<span data-ttu-id="d9c76-126">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="d9c76-126">The document's name.</span></span> <span data-ttu-id="d9c76-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c76-127">Read-only.</span></span>|
|<span data-ttu-id="d9c76-128">contentType</span><span class="sxs-lookup"><span data-stu-id="d9c76-128">contentType</span></span>|<span data-ttu-id="d9c76-129">String</span><span class="sxs-lookup"><span data-stu-id="d9c76-129">String</span></span>|<span data-ttu-id="d9c76-130">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="d9c76-130">The document's content (MIME) type.</span></span> <span data-ttu-id="d9c76-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c76-131">Read-only.</span></span>|
|<span data-ttu-id="d9c76-132">size</span><span class="sxs-lookup"><span data-stu-id="d9c76-132">size</span></span>|<span data-ttu-id="d9c76-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c76-133">Int64</span></span>|<span data-ttu-id="d9c76-134">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="d9c76-134">The document's size in bytes.</span></span> <span data-ttu-id="d9c76-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9c76-135">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9c76-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9c76-136">JSON representation</span></span>

<span data-ttu-id="d9c76-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9c76-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


