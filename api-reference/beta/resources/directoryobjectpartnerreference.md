---
title: тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8b9d6a8826c38171dc7b32c281c371e841906f82
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761563"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="e15ba-104">тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="e15ba-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="e15ba-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15ba-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e15ba-106">Представляет ссылку на объект каталога в организации-партнере.</span><span class="sxs-lookup"><span data-stu-id="e15ba-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="e15ba-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e15ba-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e15ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e15ba-108">Properties</span></span>

| <span data-ttu-id="e15ba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e15ba-109">Property</span></span> | <span data-ttu-id="e15ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e15ba-110">Type</span></span> | <span data-ttu-id="e15ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e15ba-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e15ba-112">description</span><span class="sxs-lookup"><span data-stu-id="e15ba-112">description</span></span>|<span data-ttu-id="e15ba-113">String</span><span class="sxs-lookup"><span data-stu-id="e15ba-113">String</span></span>| <span data-ttu-id="e15ba-114">Описание возвращенного объекта.</span><span class="sxs-lookup"><span data-stu-id="e15ba-114">Description of the object returned.</span></span> <span data-ttu-id="e15ba-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-115">Read-only.</span></span> |
|<span data-ttu-id="e15ba-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e15ba-116">displayName</span></span>|<span data-ttu-id="e15ba-117">String</span><span class="sxs-lookup"><span data-stu-id="e15ba-117">String</span></span>| <span data-ttu-id="e15ba-118">Имя возвращаемого объекта каталога, например группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="e15ba-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-119">Read-only.</span></span> |
|<span data-ttu-id="e15ba-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="e15ba-120">externalPartnerTenantId</span></span>|<span data-ttu-id="e15ba-121">Guid</span><span class="sxs-lookup"><span data-stu-id="e15ba-121">Guid</span></span>| <span data-ttu-id="e15ba-122">Идентификатор клиента для клиента-партнера.</span><span class="sxs-lookup"><span data-stu-id="e15ba-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="e15ba-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-123">Read-only.</span></span> |
|<span data-ttu-id="e15ba-124">id</span><span class="sxs-lookup"><span data-stu-id="e15ba-124">id</span></span>|<span data-ttu-id="e15ba-125">String</span><span class="sxs-lookup"><span data-stu-id="e15ba-125">String</span></span>| <span data-ttu-id="e15ba-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="e15ba-126">The unique identifier for the resource.</span></span> <span data-ttu-id="e15ba-127">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e15ba-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="e15ba-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-128">Read-only.</span></span> |
|<span data-ttu-id="e15ba-129">objectType</span><span class="sxs-lookup"><span data-stu-id="e15ba-129">objectType</span></span>|<span data-ttu-id="e15ba-130">String</span><span class="sxs-lookup"><span data-stu-id="e15ba-130">String</span></span>| <span data-ttu-id="e15ba-131">Тип ссылаемого объекта в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="e15ba-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="e15ba-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e15ba-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e15ba-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e15ba-133">JSON representation</span></span>

<span data-ttu-id="e15ba-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e15ba-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e15ba-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e15ba-135">See also</span></span>

- [<span data-ttu-id="e15ba-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="e15ba-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
