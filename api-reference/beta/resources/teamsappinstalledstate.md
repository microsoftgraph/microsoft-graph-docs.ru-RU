---
title: Members
description: Описывает текущее состояние установки teamsApp.
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316795"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="98790-103">Тип перечисления teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="98790-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="98790-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98790-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98790-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98790-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98790-106">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="98790-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="98790-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="98790-107">Members</span></span>

| <span data-ttu-id="98790-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="98790-108">Member</span></span> | <span data-ttu-id="98790-109">Значение</span><span class="sxs-lookup"><span data-stu-id="98790-109">Value</span></span>| <span data-ttu-id="98790-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98790-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="98790-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="98790-111">notInstalled</span></span>|<span data-ttu-id="98790-112">0</span><span class="sxs-lookup"><span data-stu-id="98790-112">0</span></span>|<span data-ttu-id="98790-113">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="98790-113">App is not installed to team.</span></span>|
|<span data-ttu-id="98790-114">установлен</span><span class="sxs-lookup"><span data-stu-id="98790-114">installed</span></span>|<span data-ttu-id="98790-115">1</span><span class="sxs-lookup"><span data-stu-id="98790-115">1</span></span>|<span data-ttu-id="98790-116">Приложение устанавливается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="98790-116">App is installed normally.</span></span>|
|<span data-ttu-id="98790-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="98790-117">installedAndHidden</span></span>|<span data-ttu-id="98790-118">2</span><span class="sxs-lookup"><span data-stu-id="98790-118">2</span></span>|<span data-ttu-id="98790-119">Приложение установлен, но скрыты.</span><span class="sxs-lookup"><span data-stu-id="98790-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="98790-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="98790-120">installedAndPermanent</span></span>|<span data-ttu-id="98790-121">3</span><span class="sxs-lookup"><span data-stu-id="98790-121">3</span></span>|<span data-ttu-id="98790-122">Приложение устанавливается без возможности восстановления и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="98790-122">App is permanently installed and may not be removed.</span></span>|
