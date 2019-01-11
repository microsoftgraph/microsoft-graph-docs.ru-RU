---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
localization_priority: Normal
ms.openlocfilehash: e394d52a5f7ed5e8dce1c61d31d787d62bd36e56
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892339"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="7d261-102">Тип ресурса contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="7d261-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="7d261-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d261-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d261-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d261-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d261-105">Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d261-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d261-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d261-106">JSON representation</span></span>

<span data-ttu-id="7d261-107">Ниже показано представление ресурса **contentTypeInfo** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d261-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="7d261-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d261-108">Properties</span></span>

| <span data-ttu-id="7d261-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7d261-109">Property name</span></span>  | <span data-ttu-id="7d261-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d261-110">Type</span></span>    | <span data-ttu-id="7d261-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d261-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="7d261-112">**id**</span><span class="sxs-lookup"><span data-stu-id="7d261-112">**id**</span></span>         | <span data-ttu-id="7d261-113">строка</span><span class="sxs-lookup"><span data-stu-id="7d261-113">string</span></span>  | <span data-ttu-id="7d261-114">Идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="7d261-114">The id of the content type.</span></span>
| <span data-ttu-id="7d261-115">**name**</span><span class="sxs-lookup"><span data-stu-id="7d261-115">**name**</span></span>       | <span data-ttu-id="7d261-116">строка</span><span class="sxs-lookup"><span data-stu-id="7d261-116">string</span></span>  | <span data-ttu-id="7d261-117">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="7d261-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
