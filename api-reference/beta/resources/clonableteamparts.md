---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076147"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="923ac-103">Тип перечисления clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="923ac-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="923ac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="923ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="923ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="923ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="923ac-106">Описывается, какие части [группы](../resources/team.md) должны клонировании.</span><span class="sxs-lookup"><span data-stu-id="923ac-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="923ac-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="923ac-107">Members</span></span>

| <span data-ttu-id="923ac-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="923ac-108">Member</span></span> | <span data-ttu-id="923ac-109">Значение</span><span class="sxs-lookup"><span data-stu-id="923ac-109">Value</span></span>| <span data-ttu-id="923ac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="923ac-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="923ac-111">apps</span><span class="sxs-lookup"><span data-stu-id="923ac-111">apps</span></span>|<span data-ttu-id="923ac-112">1</span><span class="sxs-lookup"><span data-stu-id="923ac-112">1</span></span>|<span data-ttu-id="923ac-113">Скопируйте список установленных приложениях.</span><span class="sxs-lookup"><span data-stu-id="923ac-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="923ac-114">вкладки</span><span class="sxs-lookup"><span data-stu-id="923ac-114">tabs</span></span>|<span data-ttu-id="923ac-115">2</span><span class="sxs-lookup"><span data-stu-id="923ac-115">2</span></span>|<span data-ttu-id="923ac-116">Копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="923ac-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="923ac-117">settings</span><span class="sxs-lookup"><span data-stu-id="923ac-117">settings</span></span>|<span data-ttu-id="923ac-118">4</span><span class="sxs-lookup"><span data-stu-id="923ac-118">4</span></span>|<span data-ttu-id="923ac-119">Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="923ac-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="923ac-120">каналы</span><span class="sxs-lookup"><span data-stu-id="923ac-120">channels</span></span>|<span data-ttu-id="923ac-121">8</span><span class="sxs-lookup"><span data-stu-id="923ac-121">8</span></span>|<span data-ttu-id="923ac-122">Копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="923ac-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="923ac-123">members</span><span class="sxs-lookup"><span data-stu-id="923ac-123">members</span></span>|<span data-ttu-id="923ac-124">16</span><span class="sxs-lookup"><span data-stu-id="923ac-124">16</span></span>|<span data-ttu-id="923ac-125">Копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="923ac-125">copies the members and owners of the team.</span></span>|
