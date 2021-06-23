---
title: Тип ресурса teamwork
description: Контейнер для функций Microsoft Teams, доступных организации.
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 439a4c5234d6442c2394dc8154b08d7cce2e5c69
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060447"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="6bf10-103">Тип ресурса teamwork</span><span class="sxs-lookup"><span data-stu-id="6bf10-103">teamwork resource type</span></span>

<span data-ttu-id="6bf10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bf10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bf10-105">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.</span><span class="sxs-lookup"><span data-stu-id="6bf10-105">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="6bf10-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bf10-106">Properties</span></span>

| <span data-ttu-id="6bf10-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bf10-107">Property</span></span> | <span data-ttu-id="6bf10-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf10-108">Type</span></span> | <span data-ttu-id="6bf10-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf10-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6bf10-110">id</span><span class="sxs-lookup"><span data-stu-id="6bf10-110">id</span></span>|<span data-ttu-id="6bf10-111">string</span><span class="sxs-lookup"><span data-stu-id="6bf10-111">string</span></span>| <span data-ttu-id="6bf10-112">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="6bf10-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6bf10-113">Связи</span><span class="sxs-lookup"><span data-stu-id="6bf10-113">Relationships</span></span>

| <span data-ttu-id="6bf10-114">Связь</span><span class="sxs-lookup"><span data-stu-id="6bf10-114">Relationship</span></span> | <span data-ttu-id="6bf10-115">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf10-115">Type</span></span> | <span data-ttu-id="6bf10-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf10-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6bf10-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="6bf10-117">installedApps</span></span>|<span data-ttu-id="6bf10-118">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="6bf10-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="6bf10-119">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="6bf10-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bf10-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bf10-120">JSON representation</span></span>

<span data-ttu-id="6bf10-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf10-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6bf10-122">См. также</span><span class="sxs-lookup"><span data-stu-id="6bf10-122">See Also</span></span>

- [<span data-ttu-id="6bf10-123">Ресурс userTeamwork</span><span class="sxs-lookup"><span data-stu-id="6bf10-123">userTeamwork resource</span></span>](userteamwork.md)


