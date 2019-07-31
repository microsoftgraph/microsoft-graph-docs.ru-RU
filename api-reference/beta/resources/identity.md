---
author: JeremyKelley
description: Ресурс Identity представляет удостоверение субъекта.
ms.date: 09/14/2017
title: Удостоверение
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cb05aa4a8ddf9d4e641bcebdff3f5984ddd34d61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971825"
---
# <a name="identity-resource-type"></a><span data-ttu-id="d880c-103">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="d880c-103">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d880c-p101">Ресурс **Identity** представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.</span><span class="sxs-lookup"><span data-stu-id="d880c-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d880c-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d880c-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="d880c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d880c-107">Properties</span></span>

| <span data-ttu-id="d880c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d880c-108">Property</span></span>            | <span data-ttu-id="d880c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d880c-109">Type</span></span>   | <span data-ttu-id="d880c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d880c-110">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d880c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d880c-111">displayName</span></span>         | <span data-ttu-id="d880c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="d880c-112">String</span></span> | <span data-ttu-id="d880c-p102">Отображаемое имя удостоверения. Обратите внимание, что оно может не всегда быть доступно или актуально. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="d880c-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="d880c-116">id</span><span class="sxs-lookup"><span data-stu-id="d880c-116">id</span></span>                  | <span data-ttu-id="d880c-117">String</span><span class="sxs-lookup"><span data-stu-id="d880c-117">String</span></span> | <span data-ttu-id="d880c-118">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d880c-118">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="d880c-119">tenantId</span><span class="sxs-lookup"><span data-stu-id="d880c-119">tenantId</span></span>            | <span data-ttu-id="d880c-120">String</span><span class="sxs-lookup"><span data-stu-id="d880c-120">String</span></span> | <span data-ttu-id="d880c-121">Уникальный идентификатор клиента (необязательно).</span><span class="sxs-lookup"><span data-stu-id="d880c-121">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="d880c-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="d880c-122">Remarks</span></span>

<span data-ttu-id="d880c-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="d880c-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->
