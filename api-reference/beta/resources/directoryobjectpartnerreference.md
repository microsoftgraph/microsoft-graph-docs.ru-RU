---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91d33993ea83ea7eba883534efb513fa80287a64
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340854"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="2e442-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="2e442-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e442-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="2e442-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="2e442-106">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2e442-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2e442-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e442-107">Properties</span></span>

| <span data-ttu-id="2e442-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e442-108">Property</span></span> | <span data-ttu-id="2e442-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e442-109">Type</span></span> | <span data-ttu-id="2e442-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e442-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2e442-111">description</span><span class="sxs-lookup"><span data-stu-id="2e442-111">description</span></span>|<span data-ttu-id="2e442-112">String</span><span class="sxs-lookup"><span data-stu-id="2e442-112">String</span></span>| <span data-ttu-id="2e442-113">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="2e442-113">Description of the object returned.</span></span> <span data-ttu-id="2e442-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e442-114">Read-only.</span></span> |
|<span data-ttu-id="2e442-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2e442-115">displayName</span></span>|<span data-ttu-id="2e442-116">String</span><span class="sxs-lookup"><span data-stu-id="2e442-116">String</span></span>| <span data-ttu-id="2e442-117">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="2e442-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="2e442-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e442-118">Read-only.</span></span> |
|<span data-ttu-id="2e442-119">Екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="2e442-119">externalPartnerTenantId</span></span>|<span data-ttu-id="2e442-120">GUID</span><span class="sxs-lookup"><span data-stu-id="2e442-120">Guid</span></span>| <span data-ttu-id="2e442-121">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="2e442-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="2e442-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e442-122">Read-only.</span></span> |
|<span data-ttu-id="2e442-123">id</span><span class="sxs-lookup"><span data-stu-id="2e442-123">id</span></span>|<span data-ttu-id="2e442-124">Строка</span><span class="sxs-lookup"><span data-stu-id="2e442-124">String</span></span>| <span data-ttu-id="2e442-125">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="2e442-125">The unique identifier for the resource.</span></span> <span data-ttu-id="2e442-126">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2e442-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="2e442-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e442-127">Read-only.</span></span> |
|<span data-ttu-id="2e442-128">objectType</span><span class="sxs-lookup"><span data-stu-id="2e442-128">objectType</span></span>|<span data-ttu-id="2e442-129">String</span><span class="sxs-lookup"><span data-stu-id="2e442-129">String</span></span>| <span data-ttu-id="2e442-130">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="2e442-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="2e442-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e442-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e442-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e442-132">JSON representation</span></span>

<span data-ttu-id="2e442-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e442-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2e442-134">См. также</span><span class="sxs-lookup"><span data-stu-id="2e442-134">See also</span></span>

- [<span data-ttu-id="2e442-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="2e442-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
