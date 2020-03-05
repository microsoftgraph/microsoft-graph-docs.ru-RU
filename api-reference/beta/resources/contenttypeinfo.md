---
author: daspek
description: Ресурс contentTypeInfo указывает тип контента элемента в SharePoint.
ms.date: 09/12/2017
title: contentTypeInfo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0aa9518f2b9597f910586ab49284dfe6f44a17ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507431"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="e0875-103">Тип ресурса contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="e0875-103">ContentTypeInfo resource type</span></span>

<span data-ttu-id="e0875-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e0875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0875-105">Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e0875-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0875-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0875-106">JSON representation</span></span>

<span data-ttu-id="e0875-107">Ниже показано представление ресурса **contentTypeInfo** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0875-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e0875-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0875-108">Properties</span></span>

| <span data-ttu-id="e0875-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e0875-109">Property name</span></span>  | <span data-ttu-id="e0875-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0875-110">Type</span></span>    | <span data-ttu-id="e0875-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0875-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="e0875-112">**id**</span><span class="sxs-lookup"><span data-stu-id="e0875-112">**id**</span></span>         | <span data-ttu-id="e0875-113">строка</span><span class="sxs-lookup"><span data-stu-id="e0875-113">string</span></span>  | <span data-ttu-id="e0875-114">Идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="e0875-114">The id of the content type.</span></span>
| <span data-ttu-id="e0875-115">**name**</span><span class="sxs-lookup"><span data-stu-id="e0875-115">**name**</span></span>       | <span data-ttu-id="e0875-116">string</span><span class="sxs-lookup"><span data-stu-id="e0875-116">string</span></span>  | <span data-ttu-id="e0875-117">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="e0875-117">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
