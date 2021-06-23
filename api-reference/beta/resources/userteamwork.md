---
title: Тип ресурса userTeamwork
description: 'Контейнер для функций Microsoft Teams, доступных пользователю. '
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6ef5bb1ddf0944e7d61ab5321ae50e766713326c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060439"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="de39c-103">Тип ресурса userTeamwork</span><span class="sxs-lookup"><span data-stu-id="de39c-103">userTeamwork resource type</span></span>

<span data-ttu-id="de39c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de39c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de39c-105">Контейнер для набора функциональных возможностей Microsoft Teams, доступных для пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="de39c-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="de39c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="de39c-106">Properties</span></span>

| <span data-ttu-id="de39c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="de39c-107">Property</span></span> | <span data-ttu-id="de39c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="de39c-108">Type</span></span> | <span data-ttu-id="de39c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de39c-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="de39c-110">id</span><span class="sxs-lookup"><span data-stu-id="de39c-110">id</span></span>|<span data-ttu-id="de39c-111">string</span><span class="sxs-lookup"><span data-stu-id="de39c-111">string</span></span>| <span data-ttu-id="de39c-112">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="de39c-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de39c-113">Связи</span><span class="sxs-lookup"><span data-stu-id="de39c-113">Relationships</span></span>

| <span data-ttu-id="de39c-114">Связь</span><span class="sxs-lookup"><span data-stu-id="de39c-114">Relationship</span></span> | <span data-ttu-id="de39c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="de39c-115">Type</span></span> | <span data-ttu-id="de39c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="de39c-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="de39c-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="de39c-117">installedApps</span></span>|<span data-ttu-id="de39c-118">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="de39c-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="de39c-119">Приложения, установленные в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="de39c-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de39c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de39c-120">JSON representation</span></span>

<span data-ttu-id="de39c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de39c-121">The following is a JSON representation of the resource.</span></span>

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


