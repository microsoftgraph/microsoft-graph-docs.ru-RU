---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447399"
---
# <a name="documentset-resource-type"></a><span data-ttu-id="e4459-103">Тип ресурса documentSet</span><span class="sxs-lookup"><span data-stu-id="e4459-103">documentSet resource type</span></span>

<span data-ttu-id="e4459-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4459-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="e4459-105">Содержит метаданные о параметрах набора документов.</span><span class="sxs-lookup"><span data-stu-id="e4459-105">Contains metadata about document set settings.</span></span>

## <a name="properties"></a><span data-ttu-id="e4459-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4459-106">Properties</span></span>

| <span data-ttu-id="e4459-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e4459-107">Property name</span></span>  | <span data-ttu-id="e4459-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4459-108">Type</span></span>    | <span data-ttu-id="e4459-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4459-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="e4459-110">shouldPrefixNameToFile</span><span class="sxs-lookup"><span data-stu-id="e4459-110">shouldPrefixNameToFile</span></span> | <span data-ttu-id="e4459-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4459-111">Boolean</span></span>  | <span data-ttu-id="e4459-112">Добавьте имя набора документов в каждое имя файла.</span><span class="sxs-lookup"><span data-stu-id="e4459-112">Add the name of the Document Set to each file name.</span></span>
| <span data-ttu-id="e4459-113">allowedContentTypes</span><span class="sxs-lookup"><span data-stu-id="e4459-113">allowedContentTypes</span></span> | <span data-ttu-id="e4459-114">Collection (microsoft.graph.contentTypeInfo)</span><span class="sxs-lookup"><span data-stu-id="e4459-114">Collection(microsoft.graph.contentTypeInfo)</span></span> | <span data-ttu-id="e4459-115">Типы контента разрешены в наборе документов.</span><span class="sxs-lookup"><span data-stu-id="e4459-115">Content types allowed in document set.</span></span>
| <span data-ttu-id="e4459-116">defaultContents</span><span class="sxs-lookup"><span data-stu-id="e4459-116">defaultContents</span></span>     | <span data-ttu-id="e4459-117">Collection (microsoft.graph.documentSetContent)</span><span class="sxs-lookup"><span data-stu-id="e4459-117">Collection(microsoft.graph.documentSetContent)</span></span> | <span data-ttu-id="e4459-118">Содержимое набора документов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e4459-118">Default contents of document set.</span></span>  
| <span data-ttu-id="e4459-119">propagateWelcomePageChanges</span><span class="sxs-lookup"><span data-stu-id="e4459-119">propagateWelcomePageChanges</span></span> | <span data-ttu-id="e4459-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4459-120">Boolean</span></span> | <span data-ttu-id="e4459-121">Указывает, следует ли нажимать изменения приветствия страниц на унаследованные типы контента.</span><span class="sxs-lookup"><span data-stu-id="e4459-121">Specifies whether to push welcome page changes to inherited content types.</span></span>  
| <span data-ttu-id="e4459-122">sharedColumns</span><span class="sxs-lookup"><span data-stu-id="e4459-122">sharedColumns</span></span>       | <span data-ttu-id="e4459-123">Коллекция (microsoft.graph.columnDefinition)</span><span class="sxs-lookup"><span data-stu-id="e4459-123">Collection(microsoft.graph.columnDefinition)</span></span> | <span data-ttu-id="e4459-124">Столбцы, отредактированы в наборе документов, которые синхронизируются со всеми документами в наборе.</span><span class="sxs-lookup"><span data-stu-id="e4459-124">Columns edited on the document set that synchronize to all documents in the set.</span></span> <span data-ttu-id="e4459-125">Эти данные можно прочитать только в самих документах.</span><span class="sxs-lookup"><span data-stu-id="e4459-125">These are read-only on the documents themselves.</span></span> 
| <span data-ttu-id="e4459-126">welcomePageColumns</span><span class="sxs-lookup"><span data-stu-id="e4459-126">welcomePageColumns</span></span>  | <span data-ttu-id="e4459-127">Коллекция (microsoft.graph.columnDefinition)</span><span class="sxs-lookup"><span data-stu-id="e4459-127">Collection(microsoft.graph.columnDefinition)</span></span>  | <span data-ttu-id="e4459-128">Указывает столбцы, которые будут показываться на странице приветствия для набора документов.</span><span class="sxs-lookup"><span data-stu-id="e4459-128">Specifies columns to show on the welcome page for the document set.</span></span>  
| <span data-ttu-id="e4459-129">welcomePageUrl</span><span class="sxs-lookup"><span data-stu-id="e4459-129">welcomePageUrl</span></span>      | <span data-ttu-id="e4459-130">string</span><span class="sxs-lookup"><span data-stu-id="e4459-130">string</span></span> | <span data-ttu-id="e4459-131">Url-адрес страницы welcome.</span><span class="sxs-lookup"><span data-stu-id="e4459-131">Welcome page absolute URL.</span></span>  

## <a name="json-representation"></a><span data-ttu-id="e4459-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4459-132">JSON representation</span></span>

<span data-ttu-id="e4459-133">Ниже приводится представление JSON ресурса **documentSet.**</span><span class="sxs-lookup"><span data-stu-id="e4459-133">The following is a JSON representation of a **documentSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
