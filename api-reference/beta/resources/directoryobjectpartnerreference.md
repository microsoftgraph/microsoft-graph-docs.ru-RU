---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
ms.openlocfilehash: ebdd7380eaa6b59488aca46120339f7175b640fa
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27224129"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="a8b7d-104">Тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="a8b7d-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="a8b7d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8b7d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8b7d-107">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="a8b7d-108">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="a8b7d-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="a8b7d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8b7d-109">Properties</span></span>

| <span data-ttu-id="a8b7d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8b7d-110">Property</span></span> | <span data-ttu-id="a8b7d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a8b7d-111">Type</span></span> | <span data-ttu-id="a8b7d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a8b7d-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8b7d-113">описание</span><span class="sxs-lookup"><span data-stu-id="a8b7d-113">description</span></span>|<span data-ttu-id="a8b7d-114">Строка</span><span class="sxs-lookup"><span data-stu-id="a8b7d-114">String</span></span>| <span data-ttu-id="a8b7d-115">Описание объект, возвращенный.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-115">Description of the object returned.</span></span> <span data-ttu-id="a8b7d-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-116">Read-only.</span></span> |
|<span data-ttu-id="a8b7d-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a8b7d-117">displayName</span></span>|<span data-ttu-id="a8b7d-118">Строка</span><span class="sxs-lookup"><span data-stu-id="a8b7d-118">String</span></span>| <span data-ttu-id="a8b7d-119">Имя объекта каталога, возвращаемых, такой как группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="a8b7d-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-120">Read-only.</span></span> |
|<span data-ttu-id="a8b7d-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="a8b7d-121">externalPartnerTenantId</span></span>|<span data-ttu-id="a8b7d-122">Guid</span><span class="sxs-lookup"><span data-stu-id="a8b7d-122">Guid</span></span>| <span data-ttu-id="a8b7d-123">Идентификатор клиента для клиента партнера.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="a8b7d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-124">Read-only.</span></span> |
|<span data-ttu-id="a8b7d-125">id</span><span class="sxs-lookup"><span data-stu-id="a8b7d-125">id</span></span>|<span data-ttu-id="a8b7d-126">Строка</span><span class="sxs-lookup"><span data-stu-id="a8b7d-126">String</span></span>| <span data-ttu-id="a8b7d-127">Уникальный идентификатор для ресурса.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-127">The unique identifier for the resource.</span></span> <span data-ttu-id="a8b7d-128">Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="a8b7d-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="a8b7d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-129">Read-only.</span></span> |
|<span data-ttu-id="a8b7d-130">objectType</span><span class="sxs-lookup"><span data-stu-id="a8b7d-130">objectType</span></span>|<span data-ttu-id="a8b7d-131">Строка</span><span class="sxs-lookup"><span data-stu-id="a8b7d-131">String</span></span>| <span data-ttu-id="a8b7d-132">Тип объекта, который указывает ссылка в партнера для клиентов.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="a8b7d-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8b7d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8b7d-134">JSON representation</span></span>

<span data-ttu-id="a8b7d-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8b7d-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a8b7d-136">См. также</span><span class="sxs-lookup"><span data-stu-id="a8b7d-136">See also</span></span>

- [<span data-ttu-id="a8b7d-137">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="a8b7d-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
