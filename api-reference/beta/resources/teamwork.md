---
title: Тип ресурса teamwork
description: Контейнер для функций Microsoft Teams, доступных организации.
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a68c7422b43106882327dd0a3068f89aad20b6e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519801"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="98719-103">Тип ресурса teamwork</span><span class="sxs-lookup"><span data-stu-id="98719-103">teamwork resource type</span></span>

<span data-ttu-id="98719-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98719-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98719-105">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.</span><span class="sxs-lookup"><span data-stu-id="98719-105">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="98719-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98719-106">Properties</span></span>

| <span data-ttu-id="98719-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98719-107">Property</span></span> | <span data-ttu-id="98719-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98719-108">Type</span></span> | <span data-ttu-id="98719-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98719-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="98719-110">id</span><span class="sxs-lookup"><span data-stu-id="98719-110">id</span></span>|<span data-ttu-id="98719-111">string</span><span class="sxs-lookup"><span data-stu-id="98719-111">string</span></span>| <span data-ttu-id="98719-112">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="98719-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98719-113">Связи</span><span class="sxs-lookup"><span data-stu-id="98719-113">Relationships</span></span>

| <span data-ttu-id="98719-114">Связь</span><span class="sxs-lookup"><span data-stu-id="98719-114">Relationship</span></span> | <span data-ttu-id="98719-115">Тип</span><span class="sxs-lookup"><span data-stu-id="98719-115">Type</span></span> | <span data-ttu-id="98719-116">Описание</span><span class="sxs-lookup"><span data-stu-id="98719-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="98719-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="98719-117">installedApps</span></span>|<span data-ttu-id="98719-118">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="98719-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="98719-119">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="98719-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98719-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98719-120">JSON representation</span></span>

<span data-ttu-id="98719-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98719-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="98719-122">См. также</span><span class="sxs-lookup"><span data-stu-id="98719-122">See Also</span></span>

- [<span data-ttu-id="98719-123">Ресурс userTeamwork</span><span class="sxs-lookup"><span data-stu-id="98719-123">userTeamwork resource</span></span>](userteamwork.md)
