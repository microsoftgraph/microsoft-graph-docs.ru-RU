---
title: Members
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517276"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="30256-103">Тип перечисления teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="30256-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30256-104">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="30256-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="30256-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="30256-105">Members</span></span>

| <span data-ttu-id="30256-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="30256-106">Member</span></span> | <span data-ttu-id="30256-107">Значение</span><span class="sxs-lookup"><span data-stu-id="30256-107">Value</span></span>| <span data-ttu-id="30256-108">Описание</span><span class="sxs-lookup"><span data-stu-id="30256-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="30256-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="30256-109">notInstalled</span></span>|<span data-ttu-id="30256-110">(0)</span><span class="sxs-lookup"><span data-stu-id="30256-110">0</span></span>|<span data-ttu-id="30256-111">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="30256-111">App is not installed to team.</span></span>|
|<span data-ttu-id="30256-112">Installed</span><span class="sxs-lookup"><span data-stu-id="30256-112">installed</span></span>|<span data-ttu-id="30256-113">$1</span><span class="sxs-lookup"><span data-stu-id="30256-113">1</span></span>|<span data-ttu-id="30256-114">Приложение устанавливается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="30256-114">App is installed normally.</span></span>|
|<span data-ttu-id="30256-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="30256-115">installedAndHidden</span></span>|<span data-ttu-id="30256-116">–2</span><span class="sxs-lookup"><span data-stu-id="30256-116">2</span></span>|<span data-ttu-id="30256-117">Приложение установлен, но скрыты.</span><span class="sxs-lookup"><span data-stu-id="30256-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="30256-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="30256-118">installedAndPermanent</span></span>|<span data-ttu-id="30256-119">–3</span><span class="sxs-lookup"><span data-stu-id="30256-119">3</span></span>|<span data-ttu-id="30256-120">Приложение устанавливается без возможности восстановления и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="30256-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
