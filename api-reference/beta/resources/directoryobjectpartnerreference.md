---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3158e081586cbcb822d385cbb357b017ac7239ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507025"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="cc56e-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="cc56e-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="cc56e-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cc56e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc56e-106">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="cc56e-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="cc56e-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="cc56e-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cc56e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc56e-108">Properties</span></span>

| <span data-ttu-id="cc56e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc56e-109">Property</span></span> | <span data-ttu-id="cc56e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cc56e-110">Type</span></span> | <span data-ttu-id="cc56e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc56e-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cc56e-112">description</span><span class="sxs-lookup"><span data-stu-id="cc56e-112">description</span></span>|<span data-ttu-id="cc56e-113">String</span><span class="sxs-lookup"><span data-stu-id="cc56e-113">String</span></span>| <span data-ttu-id="cc56e-114">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="cc56e-114">Description of the object returned.</span></span> <span data-ttu-id="cc56e-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc56e-115">Read-only.</span></span> |
|<span data-ttu-id="cc56e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="cc56e-116">displayName</span></span>|<span data-ttu-id="cc56e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="cc56e-117">String</span></span>| <span data-ttu-id="cc56e-118">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="cc56e-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="cc56e-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc56e-119">Read-only.</span></span> |
|<span data-ttu-id="cc56e-120">екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="cc56e-120">externalPartnerTenantId</span></span>|<span data-ttu-id="cc56e-121">GUID</span><span class="sxs-lookup"><span data-stu-id="cc56e-121">Guid</span></span>| <span data-ttu-id="cc56e-122">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="cc56e-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="cc56e-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc56e-123">Read-only.</span></span> |
|<span data-ttu-id="cc56e-124">id</span><span class="sxs-lookup"><span data-stu-id="cc56e-124">id</span></span>|<span data-ttu-id="cc56e-125">String</span><span class="sxs-lookup"><span data-stu-id="cc56e-125">String</span></span>| <span data-ttu-id="cc56e-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="cc56e-126">The unique identifier for the resource.</span></span> <span data-ttu-id="cc56e-127">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="cc56e-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="cc56e-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc56e-128">Read-only.</span></span> |
|<span data-ttu-id="cc56e-129">objectType</span><span class="sxs-lookup"><span data-stu-id="cc56e-129">objectType</span></span>|<span data-ttu-id="cc56e-130">String</span><span class="sxs-lookup"><span data-stu-id="cc56e-130">String</span></span>| <span data-ttu-id="cc56e-131">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="cc56e-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="cc56e-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc56e-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc56e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc56e-133">JSON representation</span></span>

<span data-ttu-id="cc56e-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc56e-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="cc56e-135">См. также</span><span class="sxs-lookup"><span data-stu-id="cc56e-135">See also</span></span>

- [<span data-ttu-id="cc56e-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="cc56e-136">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
