---
title: Тип ресурса teamwork
description: Контейнер для функций Microsoft Teams, доступных организации.
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908595"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="f8319-103">Тип ресурса teamwork</span><span class="sxs-lookup"><span data-stu-id="f8319-103">teamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8319-104">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.</span><span class="sxs-lookup"><span data-stu-id="f8319-104">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="f8319-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8319-105">Properties</span></span>

| <span data-ttu-id="f8319-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8319-106">Property</span></span> | <span data-ttu-id="f8319-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f8319-107">Type</span></span> | <span data-ttu-id="f8319-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f8319-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8319-109">id</span><span class="sxs-lookup"><span data-stu-id="f8319-109">id</span></span>|<span data-ttu-id="f8319-110">string</span><span class="sxs-lookup"><span data-stu-id="f8319-110">string</span></span>| <span data-ttu-id="f8319-111">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f8319-111">A globally unique identifier (GUID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="f8319-112">Связи</span><span class="sxs-lookup"><span data-stu-id="f8319-112">Relationships</span></span>

| <span data-ttu-id="f8319-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="f8319-113">Relationship</span></span> | <span data-ttu-id="f8319-114">Тип</span><span class="sxs-lookup"><span data-stu-id="f8319-114">Type</span></span> | <span data-ttu-id="f8319-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f8319-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8319-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="f8319-116">installedApps</span></span>|<span data-ttu-id="f8319-117">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="f8319-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="f8319-118">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="f8319-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8319-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8319-119">JSON representation</span></span>

<span data-ttu-id="f8319-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8319-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="f8319-121">См. также</span><span class="sxs-lookup"><span data-stu-id="f8319-121">See Also</span></span>

- [<span data-ttu-id="f8319-122">Ресурс userTeamwork</span><span class="sxs-lookup"><span data-stu-id="f8319-122">userTeamwork resource</span></span>](userteamwork.md)
