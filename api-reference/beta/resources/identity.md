---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: c1cd28f4c2932e4196605c408470948e5b570894
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847588"
---
# <a name="identity-resource-type"></a><span data-ttu-id="17587-102">Тип ресурса удостоверений</span><span class="sxs-lookup"><span data-stu-id="17587-102">identity resource type</span></span>

> <span data-ttu-id="17587-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17587-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17587-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17587-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17587-p102">Ресурс **Identity** представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.</span><span class="sxs-lookup"><span data-stu-id="17587-p102">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17587-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17587-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="17587-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="17587-108">Properties</span></span>

| <span data-ttu-id="17587-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="17587-109">Property</span></span>            | <span data-ttu-id="17587-110">Тип</span><span class="sxs-lookup"><span data-stu-id="17587-110">Type</span></span>   | <span data-ttu-id="17587-111">Описание</span><span class="sxs-lookup"><span data-stu-id="17587-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="17587-112">displayName</span><span class="sxs-lookup"><span data-stu-id="17587-112">displayName</span></span>         | <span data-ttu-id="17587-113">String</span><span class="sxs-lookup"><span data-stu-id="17587-113">String</span></span> | <span data-ttu-id="17587-p103">Отображаемое имя удостоверения. Обратите внимание, что оно может не всегда быть доступно или актуально. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="17587-p103">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="17587-117">id</span><span class="sxs-lookup"><span data-stu-id="17587-117">id</span></span>                  | <span data-ttu-id="17587-118">String</span><span class="sxs-lookup"><span data-stu-id="17587-118">String</span></span> | <span data-ttu-id="17587-119">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="17587-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="17587-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="17587-120">tenantId</span></span>            | <span data-ttu-id="17587-121">Строка</span><span class="sxs-lookup"><span data-stu-id="17587-121">String</span></span> | <span data-ttu-id="17587-122">Уникальный идентификатор клиента (необязательно).</span><span class="sxs-lookup"><span data-stu-id="17587-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="17587-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="17587-123">Remarks</span></span>

<span data-ttu-id="17587-p104">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="17587-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"
} -->
