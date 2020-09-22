---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a161fcd8dea1084ebb004e054daa220c85d83d26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027120"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="faeb1-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="faeb1-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="faeb1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faeb1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faeb1-106">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="faeb1-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="faeb1-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="faeb1-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="faeb1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="faeb1-108">Properties</span></span>

| <span data-ttu-id="faeb1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="faeb1-109">Property</span></span> | <span data-ttu-id="faeb1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="faeb1-110">Type</span></span> | <span data-ttu-id="faeb1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="faeb1-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="faeb1-112">description</span><span class="sxs-lookup"><span data-stu-id="faeb1-112">description</span></span>|<span data-ttu-id="faeb1-113">String</span><span class="sxs-lookup"><span data-stu-id="faeb1-113">String</span></span>| <span data-ttu-id="faeb1-114">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="faeb1-114">Description of the object returned.</span></span> <span data-ttu-id="faeb1-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeb1-115">Read-only.</span></span> |
|<span data-ttu-id="faeb1-116">displayName</span><span class="sxs-lookup"><span data-stu-id="faeb1-116">displayName</span></span>|<span data-ttu-id="faeb1-117">String</span><span class="sxs-lookup"><span data-stu-id="faeb1-117">String</span></span>| <span data-ttu-id="faeb1-118">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="faeb1-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="faeb1-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeb1-119">Read-only.</span></span> |
|<span data-ttu-id="faeb1-120">екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="faeb1-120">externalPartnerTenantId</span></span>|<span data-ttu-id="faeb1-121">Guid</span><span class="sxs-lookup"><span data-stu-id="faeb1-121">Guid</span></span>| <span data-ttu-id="faeb1-122">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="faeb1-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="faeb1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeb1-123">Read-only.</span></span> |
|<span data-ttu-id="faeb1-124">id</span><span class="sxs-lookup"><span data-stu-id="faeb1-124">id</span></span>|<span data-ttu-id="faeb1-125">String</span><span class="sxs-lookup"><span data-stu-id="faeb1-125">String</span></span>| <span data-ttu-id="faeb1-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="faeb1-126">The unique identifier for the resource.</span></span> <span data-ttu-id="faeb1-127">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="faeb1-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="faeb1-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeb1-128">Read-only.</span></span> |
|<span data-ttu-id="faeb1-129">objectType</span><span class="sxs-lookup"><span data-stu-id="faeb1-129">objectType</span></span>|<span data-ttu-id="faeb1-130">String</span><span class="sxs-lookup"><span data-stu-id="faeb1-130">String</span></span>| <span data-ttu-id="faeb1-131">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="faeb1-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="faeb1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeb1-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="faeb1-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="faeb1-133">JSON representation</span></span>

<span data-ttu-id="faeb1-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faeb1-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="faeb1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="faeb1-135">See also</span></span>

- [<span data-ttu-id="faeb1-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="faeb1-136">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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


