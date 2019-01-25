---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511053"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="4a032-104">Тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="4a032-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a032-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="4a032-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="4a032-106">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="4a032-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="4a032-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a032-107">Properties</span></span>

| <span data-ttu-id="4a032-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a032-108">Property</span></span> | <span data-ttu-id="4a032-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4a032-109">Type</span></span> | <span data-ttu-id="4a032-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a032-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a032-111">description</span><span class="sxs-lookup"><span data-stu-id="4a032-111">description</span></span>|<span data-ttu-id="4a032-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4a032-112">String</span></span>| <span data-ttu-id="4a032-113">Описание объект, возвращенный.</span><span class="sxs-lookup"><span data-stu-id="4a032-113">Description of the object returned.</span></span> <span data-ttu-id="4a032-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a032-114">Read-only.</span></span> |
|<span data-ttu-id="4a032-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4a032-115">displayName</span></span>|<span data-ttu-id="4a032-116">String</span><span class="sxs-lookup"><span data-stu-id="4a032-116">String</span></span>| <span data-ttu-id="4a032-117">Имя объекта каталога, возвращаемых, такой как группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="4a032-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="4a032-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a032-118">Read-only.</span></span> |
|<span data-ttu-id="4a032-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="4a032-119">externalPartnerTenantId</span></span>|<span data-ttu-id="4a032-120">Guid</span><span class="sxs-lookup"><span data-stu-id="4a032-120">Guid</span></span>| <span data-ttu-id="4a032-121">Идентификатор клиента для клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="4a032-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="4a032-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a032-122">Read-only.</span></span> |
|<span data-ttu-id="4a032-123">id</span><span class="sxs-lookup"><span data-stu-id="4a032-123">id</span></span>|<span data-ttu-id="4a032-124">String</span><span class="sxs-lookup"><span data-stu-id="4a032-124">String</span></span>| <span data-ttu-id="4a032-125">Уникальный идентификатор для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a032-125">The unique identifier for the resource.</span></span> <span data-ttu-id="4a032-126">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="4a032-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="4a032-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a032-127">Read-only.</span></span> |
|<span data-ttu-id="4a032-128">objectType</span><span class="sxs-lookup"><span data-stu-id="4a032-128">objectType</span></span>|<span data-ttu-id="4a032-129">String</span><span class="sxs-lookup"><span data-stu-id="4a032-129">String</span></span>| <span data-ttu-id="4a032-130">Тип объекта, который указывает ссылка в партнера для клиентов.</span><span class="sxs-lookup"><span data-stu-id="4a032-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="4a032-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a032-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a032-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a032-132">JSON representation</span></span>

<span data-ttu-id="4a032-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a032-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4a032-134">См. также</span><span class="sxs-lookup"><span data-stu-id="4a032-134">See also</span></span>

- <span data-ttu-id="4a032-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="4a032-135">[Get directory objects from a list of ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)</span></span>

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
