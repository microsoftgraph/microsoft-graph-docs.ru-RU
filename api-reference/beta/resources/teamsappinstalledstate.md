---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080672"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="3e759-103">Тип перечисления teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="3e759-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="3e759-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e759-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e759-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e759-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e759-106">Описывает текущее состояние установки [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e759-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="3e759-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3e759-107">Members</span></span>

| <span data-ttu-id="3e759-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3e759-108">Member</span></span> | <span data-ttu-id="3e759-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3e759-109">Value</span></span>| <span data-ttu-id="3e759-110">Description</span><span class="sxs-lookup"><span data-stu-id="3e759-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3e759-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="3e759-111">notInstalled</span></span>|<span data-ttu-id="3e759-112">0</span><span class="sxs-lookup"><span data-stu-id="3e759-112">0</span></span>|<span data-ttu-id="3e759-113">Приложение не установлено в группу.</span><span class="sxs-lookup"><span data-stu-id="3e759-113">App is not installed to team.</span></span>|
|<span data-ttu-id="3e759-114">установлен</span><span class="sxs-lookup"><span data-stu-id="3e759-114">installed</span></span>|<span data-ttu-id="3e759-115">1</span><span class="sxs-lookup"><span data-stu-id="3e759-115">1</span></span>|<span data-ttu-id="3e759-116">Приложение устанавливается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="3e759-116">App is installed normally.</span></span>|
|<span data-ttu-id="3e759-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="3e759-117">installedAndHidden</span></span>|<span data-ttu-id="3e759-118">2</span><span class="sxs-lookup"><span data-stu-id="3e759-118">2</span></span>|<span data-ttu-id="3e759-119">Приложение установлен, но скрыты.</span><span class="sxs-lookup"><span data-stu-id="3e759-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="3e759-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="3e759-120">installedAndPermanent</span></span>|<span data-ttu-id="3e759-121">3</span><span class="sxs-lookup"><span data-stu-id="3e759-121">3</span></span>|<span data-ttu-id="3e759-122">Приложение устанавливается без возможности восстановления и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="3e759-122">App is permanently installed and may not be removed.</span></span>|
