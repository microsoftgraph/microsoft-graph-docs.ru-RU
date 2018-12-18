---
title: Тип перечисления installState
description: Возможные значения для состояние установки.
author: tfitzmac
ms.openlocfilehash: c8e1a6ef50574eaa6f704e1d9f49d56c83046ab7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304636"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="6b802-103">Тип перечисления installState</span><span class="sxs-lookup"><span data-stu-id="6b802-103">installState enum type</span></span>

> <span data-ttu-id="6b802-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b802-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b802-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b802-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b802-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b802-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b802-107">Возможные значения для состояние установки.</span><span class="sxs-lookup"><span data-stu-id="6b802-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="6b802-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6b802-108">Members</span></span>
|<span data-ttu-id="6b802-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6b802-109">Member</span></span>|<span data-ttu-id="6b802-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6b802-110">Value</span></span>|<span data-ttu-id="6b802-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b802-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b802-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="6b802-112">notApplicable</span></span>|<span data-ttu-id="6b802-113">0</span><span class="sxs-lookup"><span data-stu-id="6b802-113">0</span></span>|<span data-ttu-id="6b802-114">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="6b802-114">Not Applicable.</span></span>|
|<span data-ttu-id="6b802-115">установлен</span><span class="sxs-lookup"><span data-stu-id="6b802-115">installed</span></span>|<span data-ttu-id="6b802-116">1</span><span class="sxs-lookup"><span data-stu-id="6b802-116">1</span></span>|<span data-ttu-id="6b802-117">Установить.</span><span class="sxs-lookup"><span data-stu-id="6b802-117">Installed.</span></span>|
|<span data-ttu-id="6b802-118">failed</span><span class="sxs-lookup"><span data-stu-id="6b802-118">failed</span></span>|<span data-ttu-id="6b802-119">2</span><span class="sxs-lookup"><span data-stu-id="6b802-119">2</span></span>|<span data-ttu-id="6b802-120">Не удалось.</span><span class="sxs-lookup"><span data-stu-id="6b802-120">Failed.</span></span>|
|<span data-ttu-id="6b802-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="6b802-121">notInstalled</span></span>|<span data-ttu-id="6b802-122">3</span><span class="sxs-lookup"><span data-stu-id="6b802-122">3</span></span>|<span data-ttu-id="6b802-123">Не установлен.</span><span class="sxs-lookup"><span data-stu-id="6b802-123">Not Installed.</span></span>|
|<span data-ttu-id="6b802-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="6b802-124">uninstallFailed</span></span>|<span data-ttu-id="6b802-125">4</span><span class="sxs-lookup"><span data-stu-id="6b802-125">4</span></span>|<span data-ttu-id="6b802-126">Удаление не удалось.</span><span class="sxs-lookup"><span data-stu-id="6b802-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="6b802-127">unknown</span><span class="sxs-lookup"><span data-stu-id="6b802-127">unknown</span></span>|<span data-ttu-id="6b802-128">5</span><span class="sxs-lookup"><span data-stu-id="6b802-128">5</span></span>|<span data-ttu-id="6b802-129">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="6b802-129">Unknown.</span></span>|





