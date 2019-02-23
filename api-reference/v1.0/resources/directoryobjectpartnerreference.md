---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b84b7447d689759444e9cfd99982857eafa71eb
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/23/2019
ms.locfileid: "30224133"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="62587-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="62587-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="62587-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="62587-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="62587-106">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="62587-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="62587-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="62587-107">Properties</span></span>

| <span data-ttu-id="62587-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="62587-108">Property</span></span> | <span data-ttu-id="62587-109">Тип</span><span class="sxs-lookup"><span data-stu-id="62587-109">Type</span></span> | <span data-ttu-id="62587-110">Описание</span><span class="sxs-lookup"><span data-stu-id="62587-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="62587-111">description</span><span class="sxs-lookup"><span data-stu-id="62587-111">description</span></span>|<span data-ttu-id="62587-112">Строка</span><span class="sxs-lookup"><span data-stu-id="62587-112">String</span></span>| <span data-ttu-id="62587-113">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="62587-113">Description of the object returned.</span></span> <span data-ttu-id="62587-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62587-114">Read-only.</span></span> |
|<span data-ttu-id="62587-115">displayName</span><span class="sxs-lookup"><span data-stu-id="62587-115">displayName</span></span>|<span data-ttu-id="62587-116">String</span><span class="sxs-lookup"><span data-stu-id="62587-116">String</span></span>| <span data-ttu-id="62587-117">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="62587-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="62587-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62587-118">Read-only.</span></span> |
|<span data-ttu-id="62587-119">Екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="62587-119">externalPartnerTenantId</span></span>|<span data-ttu-id="62587-120">Guid</span><span class="sxs-lookup"><span data-stu-id="62587-120">Guid</span></span>| <span data-ttu-id="62587-121">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="62587-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="62587-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62587-122">Read-only.</span></span> |
|<span data-ttu-id="62587-123">id</span><span class="sxs-lookup"><span data-stu-id="62587-123">id</span></span>|<span data-ttu-id="62587-124">String</span><span class="sxs-lookup"><span data-stu-id="62587-124">String</span></span>| <span data-ttu-id="62587-125">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="62587-125">The unique identifier for the resource.</span></span> <span data-ttu-id="62587-126">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="62587-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="62587-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62587-127">Read-only.</span></span> |
|<span data-ttu-id="62587-128">objectType</span><span class="sxs-lookup"><span data-stu-id="62587-128">objectType</span></span>|<span data-ttu-id="62587-129">String</span><span class="sxs-lookup"><span data-stu-id="62587-129">String</span></span>| <span data-ttu-id="62587-130">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="62587-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="62587-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62587-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62587-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62587-132">JSON representation</span></span>

<span data-ttu-id="62587-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62587-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="62587-134">См. также</span><span class="sxs-lookup"><span data-stu-id="62587-134">See also</span></span>

- [<span data-ttu-id="62587-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="62587-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
