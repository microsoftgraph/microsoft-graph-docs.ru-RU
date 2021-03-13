---
title: тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8f68c2660903c088082ec0baca995f2707a88883
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761207"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="4a590-104">тип ресурса directoryObjectPartnerReference</span><span class="sxs-lookup"><span data-stu-id="4a590-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="4a590-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a590-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a590-106">Представляет ссылку на объект каталога в организации-партнере.</span><span class="sxs-lookup"><span data-stu-id="4a590-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="4a590-107">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="4a590-107">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="4a590-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a590-108">Properties</span></span>

| <span data-ttu-id="4a590-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a590-109">Property</span></span> | <span data-ttu-id="4a590-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a590-110">Type</span></span> | <span data-ttu-id="4a590-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a590-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a590-112">description</span><span class="sxs-lookup"><span data-stu-id="4a590-112">description</span></span>|<span data-ttu-id="4a590-113">String</span><span class="sxs-lookup"><span data-stu-id="4a590-113">String</span></span>| <span data-ttu-id="4a590-114">Описание возвращенного объекта.</span><span class="sxs-lookup"><span data-stu-id="4a590-114">Description of the object returned.</span></span> <span data-ttu-id="4a590-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a590-115">Read-only.</span></span> |
|<span data-ttu-id="4a590-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4a590-116">displayName</span></span>|<span data-ttu-id="4a590-117">String</span><span class="sxs-lookup"><span data-stu-id="4a590-117">String</span></span>| <span data-ttu-id="4a590-118">Имя возвращаемого объекта каталога, например группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="4a590-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="4a590-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a590-119">Read-only.</span></span> |
|<span data-ttu-id="4a590-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="4a590-120">externalPartnerTenantId</span></span>|<span data-ttu-id="4a590-121">Guid</span><span class="sxs-lookup"><span data-stu-id="4a590-121">Guid</span></span>| <span data-ttu-id="4a590-122">Идентификатор клиента для клиента-партнера.</span><span class="sxs-lookup"><span data-stu-id="4a590-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="4a590-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a590-123">Read-only.</span></span> |
|<span data-ttu-id="4a590-124">id</span><span class="sxs-lookup"><span data-stu-id="4a590-124">id</span></span>|<span data-ttu-id="4a590-125">String</span><span class="sxs-lookup"><span data-stu-id="4a590-125">String</span></span>| <span data-ttu-id="4a590-126">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a590-126">The unique identifier for the resource.</span></span> <span data-ttu-id="4a590-127">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="4a590-127">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="4a590-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a590-128">Read-only.</span></span> |
|<span data-ttu-id="4a590-129">objectType</span><span class="sxs-lookup"><span data-stu-id="4a590-129">objectType</span></span>|<span data-ttu-id="4a590-130">String</span><span class="sxs-lookup"><span data-stu-id="4a590-130">String</span></span>| <span data-ttu-id="4a590-131">Тип ссылаемого объекта в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="4a590-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="4a590-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a590-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a590-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a590-133">JSON representation</span></span>

<span data-ttu-id="4a590-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a590-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4a590-135">См. также</span><span class="sxs-lookup"><span data-stu-id="4a590-135">See also</span></span>

- [<span data-ttu-id="4a590-136">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="4a590-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
