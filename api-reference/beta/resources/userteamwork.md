---
title: Тип ресурса userTeamwork
description: 'Контейнер для функций Microsoft Teams, доступных пользователю. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: f633f6ea214374aa7171bdd6ada24f4fadb4b507
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519493"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="3b90f-103">Тип ресурса userTeamwork</span><span class="sxs-lookup"><span data-stu-id="3b90f-103">userTeamwork resource type</span></span>

<span data-ttu-id="3b90f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b90f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b90f-105">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3b90f-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="3b90f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b90f-106">Properties</span></span>

| <span data-ttu-id="3b90f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b90f-107">Property</span></span> | <span data-ttu-id="3b90f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3b90f-108">Type</span></span> | <span data-ttu-id="3b90f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3b90f-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3b90f-110">id</span><span class="sxs-lookup"><span data-stu-id="3b90f-110">id</span></span>|<span data-ttu-id="3b90f-111">string</span><span class="sxs-lookup"><span data-stu-id="3b90f-111">string</span></span>| <span data-ttu-id="3b90f-112">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3b90f-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3b90f-113">Связи</span><span class="sxs-lookup"><span data-stu-id="3b90f-113">Relationships</span></span>

| <span data-ttu-id="3b90f-114">Связь</span><span class="sxs-lookup"><span data-stu-id="3b90f-114">Relationship</span></span> | <span data-ttu-id="3b90f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3b90f-115">Type</span></span> | <span data-ttu-id="3b90f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3b90f-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3b90f-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="3b90f-117">installedApps</span></span>|<span data-ttu-id="3b90f-118">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="3b90f-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="3b90f-119">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b90f-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b90f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b90f-120">JSON representation</span></span>

<span data-ttu-id="3b90f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b90f-121">The following is a JSON representation of the resource.</span></span>

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
