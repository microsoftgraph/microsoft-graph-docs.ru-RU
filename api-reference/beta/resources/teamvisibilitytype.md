---
title: Элементы
description: 'Описывает видимость группы. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 21f53b1d7631cde46f1bd70afcbb1346f9199d9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884541"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="66a9a-103">Тип перечисления teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="66a9a-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="66a9a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66a9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66a9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66a9a-106">Описывает видимость [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="66a9a-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="66a9a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="66a9a-107">Members</span></span>

| <span data-ttu-id="66a9a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="66a9a-108">Member</span></span> | <span data-ttu-id="66a9a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="66a9a-109">Value</span></span>| <span data-ttu-id="66a9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66a9a-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66a9a-111">закрытый</span><span class="sxs-lookup"><span data-stu-id="66a9a-111">private</span></span>|<span data-ttu-id="66a9a-112">0</span><span class="sxs-lookup"><span data-stu-id="66a9a-112">0</span></span>|<span data-ttu-id="66a9a-113">Любой пользователь может просматривать группы, но только владелец можно добавить пользователя в группу.</span><span class="sxs-lookup"><span data-stu-id="66a9a-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="66a9a-114">public</span><span class="sxs-lookup"><span data-stu-id="66a9a-114">public</span></span>|<span data-ttu-id="66a9a-115">1</span><span class="sxs-lookup"><span data-stu-id="66a9a-115">1</span></span>|<span data-ttu-id="66a9a-116">Для присоединения к группе.</span><span class="sxs-lookup"><span data-stu-id="66a9a-116">Anyone can join the team.</span></span>|
