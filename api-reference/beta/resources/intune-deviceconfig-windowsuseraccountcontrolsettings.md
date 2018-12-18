---
title: Тип перечисления windowsUserAccountControlSettings
description: Возможные значения для параметров контроля учетных записей пользователей Windows.
author: tfitzmac
ms.openlocfilehash: dcec2ca6e5b6401b5277e513867c0646bff79c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320302"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="21f01-103">Тип перечисления windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="21f01-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="21f01-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21f01-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21f01-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21f01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21f01-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21f01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21f01-107">Возможные значения для параметров контроля учетных записей пользователей Windows.</span><span class="sxs-lookup"><span data-stu-id="21f01-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="21f01-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="21f01-108">Members</span></span>
|<span data-ttu-id="21f01-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="21f01-109">Member</span></span>|<span data-ttu-id="21f01-110">Значение</span><span class="sxs-lookup"><span data-stu-id="21f01-110">Value</span></span>|<span data-ttu-id="21f01-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21f01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21f01-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="21f01-112">userDefined</span></span>|<span data-ttu-id="21f01-113">0</span><span class="sxs-lookup"><span data-stu-id="21f01-113">0</span></span>|<span data-ttu-id="21f01-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="21f01-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="21f01-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="21f01-115">alwaysNotify</span></span>|<span data-ttu-id="21f01-116">1</span><span class="sxs-lookup"><span data-stu-id="21f01-116">1</span></span>|<span data-ttu-id="21f01-117">Всегда уведомите.</span><span class="sxs-lookup"><span data-stu-id="21f01-117">Always notify.</span></span>|
|<span data-ttu-id="21f01-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="21f01-118">notifyOnAppChanges</span></span>|<span data-ttu-id="21f01-119">2</span><span class="sxs-lookup"><span data-stu-id="21f01-119">2</span></span>|<span data-ttu-id="21f01-120">Уведомление об изменениях приложения.</span><span class="sxs-lookup"><span data-stu-id="21f01-120">Notify on app changes.</span></span>|
|<span data-ttu-id="21f01-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="21f01-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="21f01-122">3</span><span class="sxs-lookup"><span data-stu-id="21f01-122">3</span></span>|<span data-ttu-id="21f01-123">Уведомления на изменения в приложении без затемнение рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="21f01-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="21f01-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="21f01-124">neverNotify</span></span>|<span data-ttu-id="21f01-125">4</span><span class="sxs-lookup"><span data-stu-id="21f01-125">4</span></span>|<span data-ttu-id="21f01-126">Никогда не уведомлять.</span><span class="sxs-lookup"><span data-stu-id="21f01-126">Never notify.</span></span>|





