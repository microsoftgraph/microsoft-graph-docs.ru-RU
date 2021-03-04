---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447402"
---
# <a name="documentsetcontent-resource-type"></a><span data-ttu-id="008a5-103">тип ресурса documentSetContent</span><span class="sxs-lookup"><span data-stu-id="008a5-103">documentSetContent resource type</span></span>

<span data-ttu-id="008a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="008a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="008a5-105">Содержит метаданные о файле, присутствуют в расположении контента по умолчанию типа контента.</span><span class="sxs-lookup"><span data-stu-id="008a5-105">Contains metadata about a file present in default content location of a content type.</span></span>

## <a name="properties"></a><span data-ttu-id="008a5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="008a5-106">Properties</span></span>

| <span data-ttu-id="008a5-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="008a5-107">Property name</span></span>  | <span data-ttu-id="008a5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="008a5-108">Type</span></span>    | <span data-ttu-id="008a5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="008a5-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="008a5-110">contentType</span><span class="sxs-lookup"><span data-stu-id="008a5-110">contentType</span></span>    | <span data-ttu-id="008a5-111">microsoft.graph.contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="008a5-111">microsoft.graph.contentTypeInfo</span></span> | <span data-ttu-id="008a5-112">Сведения о типе контента файла.</span><span class="sxs-lookup"><span data-stu-id="008a5-112">Content type information of the file.</span></span> 
| <span data-ttu-id="008a5-113">fileName</span><span class="sxs-lookup"><span data-stu-id="008a5-113">fileName</span></span>      | <span data-ttu-id="008a5-114">string</span><span class="sxs-lookup"><span data-stu-id="008a5-114">string</span></span>  | <span data-ttu-id="008a5-115">Имя файла в папке ресурсов, которое должно быть добавлено в качестве контента по умолчанию или шаблона в наборе документов</span><span class="sxs-lookup"><span data-stu-id="008a5-115">Name of the file in resource folder that should be added as a default content or a template in the document set</span></span>  
| <span data-ttu-id="008a5-116">folderName</span><span class="sxs-lookup"><span data-stu-id="008a5-116">folderName</span></span>         | <span data-ttu-id="008a5-117">string</span><span class="sxs-lookup"><span data-stu-id="008a5-117">string</span></span>  | <span data-ttu-id="008a5-118">Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.</span><span class="sxs-lookup"><span data-stu-id="008a5-118">Folder name in which the file will be placed when a new document set is created in the library.</span></span>

## <a name="json-representation"></a><span data-ttu-id="008a5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="008a5-119">JSON representation</span></span>

<span data-ttu-id="008a5-120">Вот представление JSON ресурса **documentSetContent.**</span><span class="sxs-lookup"><span data-stu-id="008a5-120">Here is a JSON representation of a **documentSetContent** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```