---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341231"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="75028-102">Тип ресурса contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="75028-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75028-103">Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="75028-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75028-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75028-104">JSON representation</span></span>

<span data-ttu-id="75028-105">Ниже показано представление ресурса **contentTypeInfo** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75028-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="75028-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="75028-106">Properties</span></span>

| <span data-ttu-id="75028-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="75028-107">Property name</span></span>  | <span data-ttu-id="75028-108">Тип</span><span class="sxs-lookup"><span data-stu-id="75028-108">Type</span></span>    | <span data-ttu-id="75028-109">Описание</span><span class="sxs-lookup"><span data-stu-id="75028-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="75028-110">**id**</span><span class="sxs-lookup"><span data-stu-id="75028-110">**id**</span></span>         | <span data-ttu-id="75028-111">string</span><span class="sxs-lookup"><span data-stu-id="75028-111">string</span></span>  | <span data-ttu-id="75028-112">Идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="75028-112">The id of the content type.</span></span>
| <span data-ttu-id="75028-113">**name**</span><span class="sxs-lookup"><span data-stu-id="75028-113">**name**</span></span>       | <span data-ttu-id="75028-114">string</span><span class="sxs-lookup"><span data-stu-id="75028-114">string</span></span>  | <span data-ttu-id="75028-115">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="75028-115">The name of the content type.</span></span>

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
