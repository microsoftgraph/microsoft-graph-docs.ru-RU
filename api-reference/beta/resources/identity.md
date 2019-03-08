---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: Идентификатор
localization_priority: Normal
ms.openlocfilehash: 1f2d1f5a305698438748ee69f73b4143b8afd8fa
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481568"
---
# <a name="identity-resource-type"></a><span data-ttu-id="88948-102">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="88948-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88948-p101">Ресурс **Identity** представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.</span><span class="sxs-lookup"><span data-stu-id="88948-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88948-105">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="88948-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="88948-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="88948-106">Properties</span></span>

| <span data-ttu-id="88948-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="88948-107">Property</span></span>            | <span data-ttu-id="88948-108">Тип</span><span class="sxs-lookup"><span data-stu-id="88948-108">Type</span></span>   | <span data-ttu-id="88948-109">Описание</span><span class="sxs-lookup"><span data-stu-id="88948-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="88948-110">displayName</span><span class="sxs-lookup"><span data-stu-id="88948-110">displayName</span></span>         | <span data-ttu-id="88948-111">String</span><span class="sxs-lookup"><span data-stu-id="88948-111">String</span></span> | <span data-ttu-id="88948-p102">Отображаемое имя удостоверения. Обратите внимание, что оно может не всегда быть доступно или актуально. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="88948-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="88948-115">id</span><span class="sxs-lookup"><span data-stu-id="88948-115">id</span></span>                  | <span data-ttu-id="88948-116">String</span><span class="sxs-lookup"><span data-stu-id="88948-116">String</span></span> | <span data-ttu-id="88948-117">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="88948-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="88948-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="88948-118">tenantId</span></span>            | <span data-ttu-id="88948-119">String</span><span class="sxs-lookup"><span data-stu-id="88948-119">String</span></span> | <span data-ttu-id="88948-120">Уникальный идентификатор клиента (необязательно).</span><span class="sxs-lookup"><span data-stu-id="88948-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="88948-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="88948-121">Remarks</span></span>

<span data-ttu-id="88948-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="88948-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": [
    "Error: /api-reference/beta/resources/identity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
