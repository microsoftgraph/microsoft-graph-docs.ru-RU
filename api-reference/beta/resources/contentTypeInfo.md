---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079125"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="0c030-102">Тип ресурса contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="0c030-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="0c030-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c030-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c030-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c030-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c030-105">Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0c030-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c030-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c030-106">JSON representation</span></span>

<span data-ttu-id="0c030-107">Ниже показано представление ресурса **contentTypeInfo** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c030-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0c030-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c030-108">Properties</span></span>

| <span data-ttu-id="0c030-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0c030-109">Property name</span></span>  | <span data-ttu-id="0c030-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c030-110">Type</span></span>    | <span data-ttu-id="0c030-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c030-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="0c030-112">**id**</span><span class="sxs-lookup"><span data-stu-id="0c030-112">**id**</span></span>         | <span data-ttu-id="0c030-113">строка</span><span class="sxs-lookup"><span data-stu-id="0c030-113">string</span></span>  | <span data-ttu-id="0c030-114">Идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="0c030-114">The id of the content type.</span></span>
| <span data-ttu-id="0c030-115">**name**</span><span class="sxs-lookup"><span data-stu-id="0c030-115">**name**</span></span>       | <span data-ttu-id="0c030-116">строка</span><span class="sxs-lookup"><span data-stu-id="0c030-116">string</span></span>  | <span data-ttu-id="0c030-117">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="0c030-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
