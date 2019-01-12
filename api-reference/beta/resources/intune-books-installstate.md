---
title: Тип перечисления installState
description: Возможные значения для состояние установки.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92fa9887760835a02c26858fb11503a0841d912e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985384"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="d0b73-103">Тип перечисления installState</span><span class="sxs-lookup"><span data-stu-id="d0b73-103">installState enum type</span></span>

> <span data-ttu-id="d0b73-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0b73-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0b73-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0b73-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0b73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0b73-107">Возможные значения для состояние установки.</span><span class="sxs-lookup"><span data-stu-id="d0b73-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="d0b73-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d0b73-108">Members</span></span>
|<span data-ttu-id="d0b73-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d0b73-109">Member</span></span>|<span data-ttu-id="d0b73-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d0b73-110">Value</span></span>|<span data-ttu-id="d0b73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0b73-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="d0b73-112">notApplicable</span></span>|<span data-ttu-id="d0b73-113">0</span><span class="sxs-lookup"><span data-stu-id="d0b73-113">0</span></span>|<span data-ttu-id="d0b73-114">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="d0b73-114">Not Applicable.</span></span>|
|<span data-ttu-id="d0b73-115">установлен</span><span class="sxs-lookup"><span data-stu-id="d0b73-115">installed</span></span>|<span data-ttu-id="d0b73-116">1</span><span class="sxs-lookup"><span data-stu-id="d0b73-116">1</span></span>|<span data-ttu-id="d0b73-117">Установить.</span><span class="sxs-lookup"><span data-stu-id="d0b73-117">Installed.</span></span>|
|<span data-ttu-id="d0b73-118">failed</span><span class="sxs-lookup"><span data-stu-id="d0b73-118">failed</span></span>|<span data-ttu-id="d0b73-119">2</span><span class="sxs-lookup"><span data-stu-id="d0b73-119">2</span></span>|<span data-ttu-id="d0b73-120">Не удалось.</span><span class="sxs-lookup"><span data-stu-id="d0b73-120">Failed.</span></span>|
|<span data-ttu-id="d0b73-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="d0b73-121">notInstalled</span></span>|<span data-ttu-id="d0b73-122">3</span><span class="sxs-lookup"><span data-stu-id="d0b73-122">3</span></span>|<span data-ttu-id="d0b73-123">Не установлен.</span><span class="sxs-lookup"><span data-stu-id="d0b73-123">Not Installed.</span></span>|
|<span data-ttu-id="d0b73-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="d0b73-124">uninstallFailed</span></span>|<span data-ttu-id="d0b73-125">4</span><span class="sxs-lookup"><span data-stu-id="d0b73-125">4</span></span>|<span data-ttu-id="d0b73-126">Удаление не удалось.</span><span class="sxs-lookup"><span data-stu-id="d0b73-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="d0b73-127">unknown</span><span class="sxs-lookup"><span data-stu-id="d0b73-127">unknown</span></span>|<span data-ttu-id="d0b73-128">5</span><span class="sxs-lookup"><span data-stu-id="d0b73-128">5</span></span>|<span data-ttu-id="d0b73-129">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="d0b73-129">Unknown.</span></span>|





