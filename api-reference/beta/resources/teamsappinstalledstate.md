---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937175"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="bbc0f-103">Тип перечисления teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="bbc0f-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="bbc0f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbc0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbc0f-106">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="bbc0f-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="bbc0f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bbc0f-107">Members</span></span>

| <span data-ttu-id="bbc0f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bbc0f-108">Member</span></span> | <span data-ttu-id="bbc0f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bbc0f-109">Value</span></span>| <span data-ttu-id="bbc0f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc0f-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbc0f-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="bbc0f-111">notInstalled</span></span>|<span data-ttu-id="bbc0f-112">0</span><span class="sxs-lookup"><span data-stu-id="bbc0f-112">0</span></span>|<span data-ttu-id="bbc0f-113">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-113">App is not installed to team.</span></span>|
|<span data-ttu-id="bbc0f-114">установлен</span><span class="sxs-lookup"><span data-stu-id="bbc0f-114">installed</span></span>|<span data-ttu-id="bbc0f-115">1</span><span class="sxs-lookup"><span data-stu-id="bbc0f-115">1</span></span>|<span data-ttu-id="bbc0f-116">Приложение устанавливается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-116">App is installed normally.</span></span>|
|<span data-ttu-id="bbc0f-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="bbc0f-117">installedAndHidden</span></span>|<span data-ttu-id="bbc0f-118">2</span><span class="sxs-lookup"><span data-stu-id="bbc0f-118">2</span></span>|<span data-ttu-id="bbc0f-119">Приложение установлен, но скрыты.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="bbc0f-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="bbc0f-120">installedAndPermanent</span></span>|<span data-ttu-id="bbc0f-121">3</span><span class="sxs-lookup"><span data-stu-id="bbc0f-121">3</span></span>|<span data-ttu-id="bbc0f-122">Приложение устанавливается без возможности восстановления и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="bbc0f-122">App is permanently installed and may not be removed.</span></span>|
