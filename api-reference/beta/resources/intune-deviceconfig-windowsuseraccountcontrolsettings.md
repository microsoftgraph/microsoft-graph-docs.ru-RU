---
title: Тип перечисления windowsUserAccountControlSettings
description: Возможные значения для параметров контроля учетных записей пользователей Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2803e2d15b907fc2a05303be8a0b4e4db4ce66f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861455"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="58679-103">Тип перечисления windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="58679-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="58679-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58679-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58679-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58679-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58679-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58679-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58679-107">Возможные значения для параметров контроля учетных записей пользователей Windows.</span><span class="sxs-lookup"><span data-stu-id="58679-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="58679-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="58679-108">Members</span></span>
|<span data-ttu-id="58679-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="58679-109">Member</span></span>|<span data-ttu-id="58679-110">Значение</span><span class="sxs-lookup"><span data-stu-id="58679-110">Value</span></span>|<span data-ttu-id="58679-111">Описание</span><span class="sxs-lookup"><span data-stu-id="58679-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58679-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="58679-112">userDefined</span></span>|<span data-ttu-id="58679-113">0</span><span class="sxs-lookup"><span data-stu-id="58679-113">0</span></span>|<span data-ttu-id="58679-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="58679-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="58679-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="58679-115">alwaysNotify</span></span>|<span data-ttu-id="58679-116">1</span><span class="sxs-lookup"><span data-stu-id="58679-116">1</span></span>|<span data-ttu-id="58679-117">Всегда уведомите.</span><span class="sxs-lookup"><span data-stu-id="58679-117">Always notify.</span></span>|
|<span data-ttu-id="58679-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="58679-118">notifyOnAppChanges</span></span>|<span data-ttu-id="58679-119">2</span><span class="sxs-lookup"><span data-stu-id="58679-119">2</span></span>|<span data-ttu-id="58679-120">Уведомление об изменениях приложения.</span><span class="sxs-lookup"><span data-stu-id="58679-120">Notify on app changes.</span></span>|
|<span data-ttu-id="58679-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="58679-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="58679-122">3</span><span class="sxs-lookup"><span data-stu-id="58679-122">3</span></span>|<span data-ttu-id="58679-123">Уведомления на изменения в приложении без затемнение рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="58679-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="58679-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="58679-124">neverNotify</span></span>|<span data-ttu-id="58679-125">4</span><span class="sxs-lookup"><span data-stu-id="58679-125">4</span></span>|<span data-ttu-id="58679-126">Никогда не уведомлять.</span><span class="sxs-lookup"><span data-stu-id="58679-126">Never notify.</span></span>|





