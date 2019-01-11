---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847574"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="e8d1e-103">Тип перечисления teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="e8d1e-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="e8d1e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8d1e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8d1e-106">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8d1e-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="e8d1e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e8d1e-107">Members</span></span>

| <span data-ttu-id="e8d1e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e8d1e-108">Member</span></span> | <span data-ttu-id="e8d1e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e8d1e-109">Value</span></span>| <span data-ttu-id="e8d1e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8d1e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e8d1e-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="e8d1e-111">notInstalled</span></span>|<span data-ttu-id="e8d1e-112">0</span><span class="sxs-lookup"><span data-stu-id="e8d1e-112">0</span></span>|<span data-ttu-id="e8d1e-113">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-113">App is not installed to team.</span></span>|
|<span data-ttu-id="e8d1e-114">установлен</span><span class="sxs-lookup"><span data-stu-id="e8d1e-114">installed</span></span>|<span data-ttu-id="e8d1e-115">1</span><span class="sxs-lookup"><span data-stu-id="e8d1e-115">1</span></span>|<span data-ttu-id="e8d1e-116">Приложение устанавливается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-116">App is installed normally.</span></span>|
|<span data-ttu-id="e8d1e-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="e8d1e-117">installedAndHidden</span></span>|<span data-ttu-id="e8d1e-118">2</span><span class="sxs-lookup"><span data-stu-id="e8d1e-118">2</span></span>|<span data-ttu-id="e8d1e-119">Приложение установлен, но скрыты.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="e8d1e-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="e8d1e-120">installedAndPermanent</span></span>|<span data-ttu-id="e8d1e-121">3</span><span class="sxs-lookup"><span data-stu-id="e8d1e-121">3</span></span>|<span data-ttu-id="e8d1e-122">Приложение устанавливается без возможности восстановления и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="e8d1e-122">App is permanently installed and may not be removed.</span></span>|
