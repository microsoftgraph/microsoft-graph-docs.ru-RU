---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462251"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="bfec4-103">тип перечисления Теамсаппинсталледстате</span><span class="sxs-lookup"><span data-stu-id="bfec4-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfec4-104">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfec4-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="bfec4-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="bfec4-105">Members</span></span>

| <span data-ttu-id="bfec4-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="bfec4-106">Member</span></span> | <span data-ttu-id="bfec4-107">Значение</span><span class="sxs-lookup"><span data-stu-id="bfec4-107">Value</span></span>| <span data-ttu-id="bfec4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bfec4-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bfec4-109">Нотинсталлед</span><span class="sxs-lookup"><span data-stu-id="bfec4-109">notInstalled</span></span>|<span data-ttu-id="bfec4-110">нуль</span><span class="sxs-lookup"><span data-stu-id="bfec4-110">0</span></span>|<span data-ttu-id="bfec4-111">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="bfec4-111">App is not installed to team.</span></span>|
|<span data-ttu-id="bfec4-112">устанавлива</span><span class="sxs-lookup"><span data-stu-id="bfec4-112">installed</span></span>|<span data-ttu-id="bfec4-113">1,1</span><span class="sxs-lookup"><span data-stu-id="bfec4-113">1</span></span>|<span data-ttu-id="bfec4-114">Приложение устанавливается обычным образом.</span><span class="sxs-lookup"><span data-stu-id="bfec4-114">App is installed normally.</span></span>|
|<span data-ttu-id="bfec4-115">Инсталледандхидден</span><span class="sxs-lookup"><span data-stu-id="bfec4-115">installedAndHidden</span></span>|<span data-ttu-id="bfec4-116">2</span><span class="sxs-lookup"><span data-stu-id="bfec4-116">2</span></span>|<span data-ttu-id="bfec4-117">Приложение установлено, но скрыто в представлении.</span><span class="sxs-lookup"><span data-stu-id="bfec4-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="bfec4-118">Инсталледандперманент</span><span class="sxs-lookup"><span data-stu-id="bfec4-118">installedAndPermanent</span></span>|<span data-ttu-id="bfec4-119">4</span><span class="sxs-lookup"><span data-stu-id="bfec4-119">3</span></span>|<span data-ttu-id="bfec4-120">Приложение устанавливается без возможности восстановления и не может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="bfec4-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
