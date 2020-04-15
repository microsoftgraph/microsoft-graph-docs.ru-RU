---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78d202cea4b092671a63870c7172dd31d3f70846
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407090"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="d90f1-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="d90f1-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="d90f1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d90f1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d90f1-106">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="d90f1-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="d90f1-107">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="d90f1-107">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="d90f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d90f1-108">Properties</span></span>

| <span data-ttu-id="d90f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d90f1-109">Property</span></span> | <span data-ttu-id="d90f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d90f1-110">Type</span></span> | <span data-ttu-id="d90f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d90f1-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d90f1-112">description</span><span class="sxs-lookup"><span data-stu-id="d90f1-112">description</span></span>|<span data-ttu-id="d90f1-113">String</span><span class="sxs-lookup"><span data-stu-id="d90f1-113">String</span></span>| <span data-ttu-id="d90f1-114">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="d90f1-114">Description of the object returned.</span></span> <span data-ttu-id="d90f1-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d90f1-115">Read-only.</span></span> |
|<span data-ttu-id="d90f1-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d90f1-116">displayName</span></span>|<span data-ttu-id="d90f1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d90f1-117">String</span></span>| <span data-ttu-id="d90f1-118">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="d90f1-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="d90f1-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d90f1-119">Read-only.</span></span> |
|<span data-ttu-id="d90f1-120">екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="d90f1-120">externalPartnerTenantId</span></span>|<span data-ttu-id="d90f1-121">GUID</span><span class="sxs-lookup"><span data-stu-id="d90f1-121">Guid</span></span>| <span data-ttu-id="d90f1-122">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="d90f1-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="d90f1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d90f1-123">Read-only.</span></span> |
|<span data-ttu-id="d90f1-124">id</span><span class="sxs-lookup"><span data-stu-id="d90f1-124">id</span></span>|<span data-ttu-id="d90f1-125">String</span><span class="sxs-lookup"><span data-stu-id="d90f1-125">String</span></span>| <span data-ttu-id="d90f1-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="d90f1-126">The unique identifier for the resource.</span></span> <span data-ttu-id="d90f1-127">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="d90f1-127">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="d90f1-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d90f1-128">Read-only.</span></span> |
|<span data-ttu-id="d90f1-129">objectType</span><span class="sxs-lookup"><span data-stu-id="d90f1-129">objectType</span></span>|<span data-ttu-id="d90f1-130">String</span><span class="sxs-lookup"><span data-stu-id="d90f1-130">String</span></span>| <span data-ttu-id="d90f1-131">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="d90f1-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="d90f1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d90f1-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d90f1-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d90f1-133">JSON representation</span></span>

<span data-ttu-id="d90f1-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d90f1-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d90f1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d90f1-135">See also</span></span>

- [<span data-ttu-id="d90f1-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="d90f1-136">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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
