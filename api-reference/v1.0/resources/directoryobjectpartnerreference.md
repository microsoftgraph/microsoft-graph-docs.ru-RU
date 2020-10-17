---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 39a3077862727f4d8457a6d0105f03296ba67950
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582158"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="380b9-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="380b9-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="380b9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="380b9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="380b9-106">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="380b9-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="380b9-107">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="380b9-107">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="380b9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="380b9-108">Properties</span></span>

| <span data-ttu-id="380b9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="380b9-109">Property</span></span> | <span data-ttu-id="380b9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="380b9-110">Type</span></span> | <span data-ttu-id="380b9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="380b9-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="380b9-112">description</span><span class="sxs-lookup"><span data-stu-id="380b9-112">description</span></span>|<span data-ttu-id="380b9-113">String</span><span class="sxs-lookup"><span data-stu-id="380b9-113">String</span></span>| <span data-ttu-id="380b9-114">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="380b9-114">Description of the object returned.</span></span> <span data-ttu-id="380b9-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="380b9-115">Read-only.</span></span> |
|<span data-ttu-id="380b9-116">displayName</span><span class="sxs-lookup"><span data-stu-id="380b9-116">displayName</span></span>|<span data-ttu-id="380b9-117">String</span><span class="sxs-lookup"><span data-stu-id="380b9-117">String</span></span>| <span data-ttu-id="380b9-118">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="380b9-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="380b9-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="380b9-119">Read-only.</span></span> |
|<span data-ttu-id="380b9-120">екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="380b9-120">externalPartnerTenantId</span></span>|<span data-ttu-id="380b9-121">Guid</span><span class="sxs-lookup"><span data-stu-id="380b9-121">Guid</span></span>| <span data-ttu-id="380b9-122">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="380b9-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="380b9-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="380b9-123">Read-only.</span></span> |
|<span data-ttu-id="380b9-124">id</span><span class="sxs-lookup"><span data-stu-id="380b9-124">id</span></span>|<span data-ttu-id="380b9-125">String</span><span class="sxs-lookup"><span data-stu-id="380b9-125">String</span></span>| <span data-ttu-id="380b9-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="380b9-126">The unique identifier for the resource.</span></span> <span data-ttu-id="380b9-127">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="380b9-127">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="380b9-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="380b9-128">Read-only.</span></span> |
|<span data-ttu-id="380b9-129">objectType</span><span class="sxs-lookup"><span data-stu-id="380b9-129">objectType</span></span>|<span data-ttu-id="380b9-130">String</span><span class="sxs-lookup"><span data-stu-id="380b9-130">String</span></span>| <span data-ttu-id="380b9-131">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="380b9-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="380b9-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="380b9-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="380b9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="380b9-133">JSON representation</span></span>

<span data-ttu-id="380b9-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="380b9-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="380b9-135">См. также</span><span class="sxs-lookup"><span data-stu-id="380b9-135">See also</span></span>

- [<span data-ttu-id="380b9-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="380b9-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
