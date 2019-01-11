---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860559"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="33179-103">Тип перечисления clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="33179-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="33179-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33179-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33179-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33179-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33179-106">Описывается, какие части [группы](../resources/team.md) должны клонировании.</span><span class="sxs-lookup"><span data-stu-id="33179-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="33179-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="33179-107">Members</span></span>

| <span data-ttu-id="33179-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="33179-108">Member</span></span> | <span data-ttu-id="33179-109">Значение</span><span class="sxs-lookup"><span data-stu-id="33179-109">Value</span></span>| <span data-ttu-id="33179-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33179-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="33179-111">apps</span><span class="sxs-lookup"><span data-stu-id="33179-111">apps</span></span>|<span data-ttu-id="33179-112">1</span><span class="sxs-lookup"><span data-stu-id="33179-112">1</span></span>|<span data-ttu-id="33179-113">Скопируйте список установленных приложениях.</span><span class="sxs-lookup"><span data-stu-id="33179-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="33179-114">вкладки</span><span class="sxs-lookup"><span data-stu-id="33179-114">tabs</span></span>|<span data-ttu-id="33179-115">2</span><span class="sxs-lookup"><span data-stu-id="33179-115">2</span></span>|<span data-ttu-id="33179-116">Копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="33179-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="33179-117">settings</span><span class="sxs-lookup"><span data-stu-id="33179-117">settings</span></span>|<span data-ttu-id="33179-118">4</span><span class="sxs-lookup"><span data-stu-id="33179-118">4</span></span>|<span data-ttu-id="33179-119">Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="33179-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="33179-120">каналы</span><span class="sxs-lookup"><span data-stu-id="33179-120">channels</span></span>|<span data-ttu-id="33179-121">8</span><span class="sxs-lookup"><span data-stu-id="33179-121">8</span></span>|<span data-ttu-id="33179-122">Копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="33179-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="33179-123">members</span><span class="sxs-lookup"><span data-stu-id="33179-123">members</span></span>|<span data-ttu-id="33179-124">16</span><span class="sxs-lookup"><span data-stu-id="33179-124">16</span></span>|<span data-ttu-id="33179-125">Копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="33179-125">copies the members and owners of the team.</span></span>|
