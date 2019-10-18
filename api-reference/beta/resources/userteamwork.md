---
title: Тип ресурса userTeamwork
description: 'Контейнер для функций Microsoft Teams, доступных пользователю. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d68ceff79856b23f2d86b2c57a6278b7c6ad7e9d
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908588"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="19d5d-103">Тип ресурса userTeamwork</span><span class="sxs-lookup"><span data-stu-id="19d5d-103">userTeamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d5d-104">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="19d5d-104">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="19d5d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="19d5d-105">Properties</span></span>

| <span data-ttu-id="19d5d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="19d5d-106">Property</span></span> | <span data-ttu-id="19d5d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="19d5d-107">Type</span></span> | <span data-ttu-id="19d5d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="19d5d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="19d5d-109">id</span><span class="sxs-lookup"><span data-stu-id="19d5d-109">id</span></span>|<span data-ttu-id="19d5d-110">string</span><span class="sxs-lookup"><span data-stu-id="19d5d-110">string</span></span>| <span data-ttu-id="19d5d-111">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="19d5d-111">A globally unique identifier (GUID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="19d5d-112">Связи</span><span class="sxs-lookup"><span data-stu-id="19d5d-112">Relationships</span></span>

| <span data-ttu-id="19d5d-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="19d5d-113">Relationship</span></span> | <span data-ttu-id="19d5d-114">Тип</span><span class="sxs-lookup"><span data-stu-id="19d5d-114">Type</span></span> | <span data-ttu-id="19d5d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="19d5d-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="19d5d-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="19d5d-116">installedApps</span></span>|<span data-ttu-id="19d5d-117">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="19d5d-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="19d5d-118">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="19d5d-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19d5d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19d5d-119">JSON representation</span></span>

<span data-ttu-id="19d5d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19d5d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
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
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
