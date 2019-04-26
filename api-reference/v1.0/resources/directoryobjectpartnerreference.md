---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b84b7447d689759444e9cfd99982857eafa71eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574689"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="fbff1-104">Тип ресурса Директорйобжектпартнерреференце</span><span class="sxs-lookup"><span data-stu-id="fbff1-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="fbff1-105">Представляет ссылку на объект каталога в партнерской организации.</span><span class="sxs-lookup"><span data-stu-id="fbff1-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="fbff1-106">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="fbff1-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="fbff1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbff1-107">Properties</span></span>

| <span data-ttu-id="fbff1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbff1-108">Property</span></span> | <span data-ttu-id="fbff1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fbff1-109">Type</span></span> | <span data-ttu-id="fbff1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fbff1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fbff1-111">description</span><span class="sxs-lookup"><span data-stu-id="fbff1-111">description</span></span>|<span data-ttu-id="fbff1-112">String</span><span class="sxs-lookup"><span data-stu-id="fbff1-112">String</span></span>| <span data-ttu-id="fbff1-113">Описание возвращаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="fbff1-113">Description of the object returned.</span></span> <span data-ttu-id="fbff1-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbff1-114">Read-only.</span></span> |
|<span data-ttu-id="fbff1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="fbff1-115">displayName</span></span>|<span data-ttu-id="fbff1-116">String</span><span class="sxs-lookup"><span data-stu-id="fbff1-116">String</span></span>| <span data-ttu-id="fbff1-117">Имя возвращаемого объекта каталога, например Group или Application.</span><span class="sxs-lookup"><span data-stu-id="fbff1-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="fbff1-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbff1-118">Read-only.</span></span> |
|<span data-ttu-id="fbff1-119">Екстерналпартнертенантид</span><span class="sxs-lookup"><span data-stu-id="fbff1-119">externalPartnerTenantId</span></span>|<span data-ttu-id="fbff1-120">Guid</span><span class="sxs-lookup"><span data-stu-id="fbff1-120">Guid</span></span>| <span data-ttu-id="fbff1-121">Идентификатор клиента для партнерского клиента.</span><span class="sxs-lookup"><span data-stu-id="fbff1-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="fbff1-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbff1-122">Read-only.</span></span> |
|<span data-ttu-id="fbff1-123">id</span><span class="sxs-lookup"><span data-stu-id="fbff1-123">id</span></span>|<span data-ttu-id="fbff1-124">Строка</span><span class="sxs-lookup"><span data-stu-id="fbff1-124">String</span></span>| <span data-ttu-id="fbff1-125">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="fbff1-125">The unique identifier for the resource.</span></span> <span data-ttu-id="fbff1-126">Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="fbff1-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="fbff1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbff1-127">Read-only.</span></span> |
|<span data-ttu-id="fbff1-128">objectType</span><span class="sxs-lookup"><span data-stu-id="fbff1-128">objectType</span></span>|<span data-ttu-id="fbff1-129">String</span><span class="sxs-lookup"><span data-stu-id="fbff1-129">String</span></span>| <span data-ttu-id="fbff1-130">Тип упоминаемого объекта в партнерской клиенте.</span><span class="sxs-lookup"><span data-stu-id="fbff1-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="fbff1-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbff1-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fbff1-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbff1-132">JSON representation</span></span>

<span data-ttu-id="fbff1-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbff1-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fbff1-134">См. также</span><span class="sxs-lookup"><span data-stu-id="fbff1-134">See also</span></span>

- [<span data-ttu-id="fbff1-135">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="fbff1-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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
