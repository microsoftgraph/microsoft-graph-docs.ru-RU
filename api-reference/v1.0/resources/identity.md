---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Identity
ms.openlocfilehash: 2ee5a17b8673a92dd66ceda2b18660b9692e1cae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026413"
---
# <a name="identity-resource-type"></a><span data-ttu-id="3292a-102">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="3292a-102">Identity resource type</span></span>

<span data-ttu-id="3292a-p101">Ресурс **Identity** представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.</span><span class="sxs-lookup"><span data-stu-id="3292a-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3292a-105">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3292a-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="3292a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3292a-106">Properties</span></span>

| <span data-ttu-id="3292a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3292a-107">Property</span></span>    | <span data-ttu-id="3292a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3292a-108">Type</span></span>   | <span data-ttu-id="3292a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3292a-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3292a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3292a-110">displayName</span></span> | <span data-ttu-id="3292a-111">String</span><span class="sxs-lookup"><span data-stu-id="3292a-111">String</span></span> | <span data-ttu-id="3292a-p102">Отображаемое имя удостоверения. Обратите внимание, что оно может не всегда быть доступно или актуально. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="3292a-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>     |
| <span data-ttu-id="3292a-115">id</span><span class="sxs-lookup"><span data-stu-id="3292a-115">id</span></span>          | <span data-ttu-id="3292a-116">String</span><span class="sxs-lookup"><span data-stu-id="3292a-116">String</span></span> | <span data-ttu-id="3292a-117">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3292a-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a><span data-ttu-id="3292a-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="3292a-118">Remarks</span></span>

<span data-ttu-id="3292a-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="3292a-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->
