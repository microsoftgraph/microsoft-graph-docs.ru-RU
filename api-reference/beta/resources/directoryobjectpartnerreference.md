---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17bab72fad3e03b843975ae62261fac9c09af791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918541"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="bc3f9-104">Тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="bc3f9-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="bc3f9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc3f9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc3f9-107">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="bc3f9-108">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="bc3f9-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="bc3f9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc3f9-109">Properties</span></span>

| <span data-ttu-id="bc3f9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc3f9-110">Property</span></span> | <span data-ttu-id="bc3f9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bc3f9-111">Type</span></span> | <span data-ttu-id="bc3f9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bc3f9-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bc3f9-113">описание</span><span class="sxs-lookup"><span data-stu-id="bc3f9-113">description</span></span>|<span data-ttu-id="bc3f9-114">String</span><span class="sxs-lookup"><span data-stu-id="bc3f9-114">String</span></span>| <span data-ttu-id="bc3f9-115">Описание объект, возвращенный.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-115">Description of the object returned.</span></span> <span data-ttu-id="bc3f9-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-116">Read-only.</span></span> |
|<span data-ttu-id="bc3f9-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bc3f9-117">displayName</span></span>|<span data-ttu-id="bc3f9-118">String</span><span class="sxs-lookup"><span data-stu-id="bc3f9-118">String</span></span>| <span data-ttu-id="bc3f9-119">Имя объекта каталога, возвращаемых, такой как группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="bc3f9-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-120">Read-only.</span></span> |
|<span data-ttu-id="bc3f9-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="bc3f9-121">externalPartnerTenantId</span></span>|<span data-ttu-id="bc3f9-122">Guid</span><span class="sxs-lookup"><span data-stu-id="bc3f9-122">Guid</span></span>| <span data-ttu-id="bc3f9-123">Идентификатор клиента для клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="bc3f9-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-124">Read-only.</span></span> |
|<span data-ttu-id="bc3f9-125">id</span><span class="sxs-lookup"><span data-stu-id="bc3f9-125">id</span></span>|<span data-ttu-id="bc3f9-126">String</span><span class="sxs-lookup"><span data-stu-id="bc3f9-126">String</span></span>| <span data-ttu-id="bc3f9-127">Уникальный идентификатор для ресурса.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-127">The unique identifier for the resource.</span></span> <span data-ttu-id="bc3f9-128">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="bc3f9-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="bc3f9-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-129">Read-only.</span></span> |
|<span data-ttu-id="bc3f9-130">objectType</span><span class="sxs-lookup"><span data-stu-id="bc3f9-130">objectType</span></span>|<span data-ttu-id="bc3f9-131">String</span><span class="sxs-lookup"><span data-stu-id="bc3f9-131">String</span></span>| <span data-ttu-id="bc3f9-132">Тип объекта, который указывает ссылка в партнера для клиентов.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="bc3f9-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc3f9-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc3f9-134">JSON representation</span></span>

<span data-ttu-id="bc3f9-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc3f9-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bc3f9-136">См. также</span><span class="sxs-lookup"><span data-stu-id="bc3f9-136">See also</span></span>

- [<span data-ttu-id="bc3f9-137">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="bc3f9-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
