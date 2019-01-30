---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640310"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="aff7e-104">Тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="aff7e-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff7e-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="aff7e-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="aff7e-106">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="aff7e-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="aff7e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff7e-107">Properties</span></span>

| <span data-ttu-id="aff7e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff7e-108">Property</span></span> | <span data-ttu-id="aff7e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aff7e-109">Type</span></span> | <span data-ttu-id="aff7e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aff7e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aff7e-111">description</span><span class="sxs-lookup"><span data-stu-id="aff7e-111">description</span></span>|<span data-ttu-id="aff7e-112">String</span><span class="sxs-lookup"><span data-stu-id="aff7e-112">String</span></span>| <span data-ttu-id="aff7e-113">Описание объект, возвращенный.</span><span class="sxs-lookup"><span data-stu-id="aff7e-113">Description of the object returned.</span></span> <span data-ttu-id="aff7e-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-114">Read-only.</span></span> |
|<span data-ttu-id="aff7e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="aff7e-115">displayName</span></span>|<span data-ttu-id="aff7e-116">String</span><span class="sxs-lookup"><span data-stu-id="aff7e-116">String</span></span>| <span data-ttu-id="aff7e-117">Имя объекта каталога, возвращаемых, такой как группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="aff7e-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-118">Read-only.</span></span> |
|<span data-ttu-id="aff7e-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="aff7e-119">externalPartnerTenantId</span></span>|<span data-ttu-id="aff7e-120">GUID</span><span class="sxs-lookup"><span data-stu-id="aff7e-120">Guid</span></span>| <span data-ttu-id="aff7e-121">Идентификатор клиента для клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="aff7e-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="aff7e-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-122">Read-only.</span></span> |
|<span data-ttu-id="aff7e-123">id</span><span class="sxs-lookup"><span data-stu-id="aff7e-123">id</span></span>|<span data-ttu-id="aff7e-124">String</span><span class="sxs-lookup"><span data-stu-id="aff7e-124">String</span></span>| <span data-ttu-id="aff7e-125">Уникальный идентификатор для ресурса.</span><span class="sxs-lookup"><span data-stu-id="aff7e-125">The unique identifier for the resource.</span></span> <span data-ttu-id="aff7e-126">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="aff7e-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="aff7e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-127">Read-only.</span></span> |
|<span data-ttu-id="aff7e-128">objectType</span><span class="sxs-lookup"><span data-stu-id="aff7e-128">objectType</span></span>|<span data-ttu-id="aff7e-129">String</span><span class="sxs-lookup"><span data-stu-id="aff7e-129">String</span></span>| <span data-ttu-id="aff7e-130">Тип объекта, который указывает ссылка в партнера для клиентов.</span><span class="sxs-lookup"><span data-stu-id="aff7e-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="aff7e-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff7e-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aff7e-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff7e-132">JSON representation</span></span>

<span data-ttu-id="aff7e-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff7e-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="aff7e-134">См. также</span><span class="sxs-lookup"><span data-stu-id="aff7e-134">See also</span></span>

- [<span data-ttu-id="aff7e-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="aff7e-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
