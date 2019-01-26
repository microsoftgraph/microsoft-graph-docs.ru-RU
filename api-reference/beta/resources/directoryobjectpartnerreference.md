---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba72f70a29e778127454ec3bd4f259331d1fe4c5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570746"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="a20f0-104">Тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="a20f0-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a20f0-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="a20f0-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="a20f0-106">Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a20f0-106">Inherits from [directoryObject](../resources/directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a20f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a20f0-107">Properties</span></span>

| <span data-ttu-id="a20f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a20f0-108">Property</span></span> | <span data-ttu-id="a20f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a20f0-109">Type</span></span> | <span data-ttu-id="a20f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a20f0-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a20f0-111">description</span><span class="sxs-lookup"><span data-stu-id="a20f0-111">description</span></span>|<span data-ttu-id="a20f0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a20f0-112">String</span></span>| <span data-ttu-id="a20f0-113">Описание объект, возвращенный.</span><span class="sxs-lookup"><span data-stu-id="a20f0-113">Description of the object returned.</span></span> <span data-ttu-id="a20f0-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-114">Read-only.</span></span> |
|<span data-ttu-id="a20f0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a20f0-115">displayName</span></span>|<span data-ttu-id="a20f0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a20f0-116">String</span></span>| <span data-ttu-id="a20f0-117">Имя объекта каталога, возвращаемых, такой как группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="a20f0-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-118">Read-only.</span></span> |
|<span data-ttu-id="a20f0-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="a20f0-119">externalPartnerTenantId</span></span>|<span data-ttu-id="a20f0-120">Guid</span><span class="sxs-lookup"><span data-stu-id="a20f0-120">Guid</span></span>| <span data-ttu-id="a20f0-121">Идентификатор клиента для клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="a20f0-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="a20f0-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-122">Read-only.</span></span> |
|<span data-ttu-id="a20f0-123">id</span><span class="sxs-lookup"><span data-stu-id="a20f0-123">id</span></span>|<span data-ttu-id="a20f0-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a20f0-124">String</span></span>| <span data-ttu-id="a20f0-125">Уникальный идентификатор для ресурса.</span><span class="sxs-lookup"><span data-stu-id="a20f0-125">The unique identifier for the resource.</span></span> <span data-ttu-id="a20f0-126">Наследуется от [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a20f0-126">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="a20f0-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-127">Read-only.</span></span> |
|<span data-ttu-id="a20f0-128">objectType</span><span class="sxs-lookup"><span data-stu-id="a20f0-128">objectType</span></span>|<span data-ttu-id="a20f0-129">Строка</span><span class="sxs-lookup"><span data-stu-id="a20f0-129">String</span></span>| <span data-ttu-id="a20f0-130">Тип объекта, который указывает ссылка в партнера для клиентов.</span><span class="sxs-lookup"><span data-stu-id="a20f0-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="a20f0-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a20f0-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a20f0-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a20f0-132">JSON representation</span></span>

<span data-ttu-id="a20f0-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a20f0-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a20f0-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a20f0-134">See also</span></span>

- [<span data-ttu-id="a20f0-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="a20f0-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
