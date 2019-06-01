---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 327528f41795360e0da109b513f3f3f08ac0b268
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657933"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="85461-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="85461-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85461-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="85461-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="85461-106">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="85461-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="85461-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="85461-107">Properties</span></span>

| <span data-ttu-id="85461-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="85461-108">Property</span></span> | <span data-ttu-id="85461-109">Тип</span><span class="sxs-lookup"><span data-stu-id="85461-109">Type</span></span> | <span data-ttu-id="85461-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85461-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="85461-111">description</span><span class="sxs-lookup"><span data-stu-id="85461-111">description</span></span>|<span data-ttu-id="85461-112">String</span><span class="sxs-lookup"><span data-stu-id="85461-112">String</span></span>| <span data-ttu-id="85461-113">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="85461-113">Description of the object returned.</span></span> <span data-ttu-id="85461-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85461-114">Read-only.</span></span> |
|<span data-ttu-id="85461-115">displayName</span><span class="sxs-lookup"><span data-stu-id="85461-115">displayName</span></span>|<span data-ttu-id="85461-116">Строка</span><span class="sxs-lookup"><span data-stu-id="85461-116">String</span></span>| <span data-ttu-id="85461-117">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="85461-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="85461-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85461-118">Read-only.</span></span> |
|<span data-ttu-id="85461-119">Екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="85461-119">externalPartnerTenantId</span></span>|<span data-ttu-id="85461-120">GUID</span><span class="sxs-lookup"><span data-stu-id="85461-120">Guid</span></span>| <span data-ttu-id="85461-121">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="85461-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="85461-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85461-122">Read-only.</span></span> |
|<span data-ttu-id="85461-123">id</span><span class="sxs-lookup"><span data-stu-id="85461-123">id</span></span>|<span data-ttu-id="85461-124">String</span><span class="sxs-lookup"><span data-stu-id="85461-124">String</span></span>| <span data-ttu-id="85461-125">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="85461-125">The unique identifier for the resource.</span></span> <span data-ttu-id="85461-126">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="85461-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="85461-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85461-127">Read-only.</span></span> |
|<span data-ttu-id="85461-128">objectType</span><span class="sxs-lookup"><span data-stu-id="85461-128">objectType</span></span>|<span data-ttu-id="85461-129">String</span><span class="sxs-lookup"><span data-stu-id="85461-129">String</span></span>| <span data-ttu-id="85461-130">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="85461-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="85461-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85461-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85461-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85461-132">JSON representation</span></span>

<span data-ttu-id="85461-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85461-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="85461-134">См. также</span><span class="sxs-lookup"><span data-stu-id="85461-134">See also</span></span>

- [<span data-ttu-id="85461-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="85461-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
