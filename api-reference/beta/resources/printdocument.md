---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c0bc886b618e061bee51ad82d7032737015f58ab
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849216"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="e26ce-103">Тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="e26ce-103">printDocument resource type</span></span>

<span data-ttu-id="e26ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e26ce-105">Представляет документ, который печатается.</span><span class="sxs-lookup"><span data-stu-id="e26ce-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="e26ce-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e26ce-106">Methods</span></span>

| <span data-ttu-id="e26ce-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e26ce-107">Method</span></span>       | <span data-ttu-id="e26ce-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e26ce-108">Return Type</span></span> | <span data-ttu-id="e26ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e26ce-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e26ce-110">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="e26ce-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="e26ce-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="e26ce-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="e26ce-112">Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="e26ce-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="e26ce-113">Скачать двоичный файл</span><span class="sxs-lookup"><span data-stu-id="e26ce-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="e26ce-114">URL-адрес скачивания</span><span class="sxs-lookup"><span data-stu-id="e26ce-114">Download Url</span></span> | <span data-ttu-id="e26ce-115">Скачайте двоичный файл, связанный с классом **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="e26ce-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="e26ce-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e26ce-116">Properties</span></span>
| <span data-ttu-id="e26ce-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e26ce-117">Property</span></span>     | <span data-ttu-id="e26ce-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e26ce-118">Type</span></span>        | <span data-ttu-id="e26ce-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e26ce-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e26ce-120">id</span><span class="sxs-lookup"><span data-stu-id="e26ce-120">id</span></span>|<span data-ttu-id="e26ce-121">String</span><span class="sxs-lookup"><span data-stu-id="e26ce-121">String</span></span>|<span data-ttu-id="e26ce-122">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="e26ce-122">The document's identifier.</span></span> <span data-ttu-id="e26ce-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e26ce-123">Read-only.</span></span>|
|<span data-ttu-id="e26ce-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e26ce-124">displayName</span></span>|<span data-ttu-id="e26ce-125">String</span><span class="sxs-lookup"><span data-stu-id="e26ce-125">String</span></span>|<span data-ttu-id="e26ce-126">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="e26ce-126">The document's name.</span></span> <span data-ttu-id="e26ce-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e26ce-127">Read-only.</span></span>|
|<span data-ttu-id="e26ce-128">contentType</span><span class="sxs-lookup"><span data-stu-id="e26ce-128">contentType</span></span>|<span data-ttu-id="e26ce-129">String</span><span class="sxs-lookup"><span data-stu-id="e26ce-129">String</span></span>|<span data-ttu-id="e26ce-130">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="e26ce-130">The document's content (MIME) type.</span></span> <span data-ttu-id="e26ce-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e26ce-131">Read-only.</span></span>|
|<span data-ttu-id="e26ce-132">size</span><span class="sxs-lookup"><span data-stu-id="e26ce-132">size</span></span>|<span data-ttu-id="e26ce-133">Int64</span><span class="sxs-lookup"><span data-stu-id="e26ce-133">Int64</span></span>|<span data-ttu-id="e26ce-134">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="e26ce-134">The document's size in bytes.</span></span> <span data-ttu-id="e26ce-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e26ce-135">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e26ce-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e26ce-136">JSON representation</span></span>

<span data-ttu-id="e26ce-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e26ce-137">The following is a JSON representation of the resource.</span></span>

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


