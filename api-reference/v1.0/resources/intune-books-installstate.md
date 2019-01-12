---
title: Тип перечисления installState
description: Возможные значения для состояние установки.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b50fb44c2af31efff81f2dd7097505f71bc791d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947554"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="d0def-103">Тип перечисления installState</span><span class="sxs-lookup"><span data-stu-id="d0def-103">installState enum type</span></span>

> <span data-ttu-id="d0def-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0def-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0def-105">Возможные значения для состояние установки.</span><span class="sxs-lookup"><span data-stu-id="d0def-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="d0def-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d0def-106">Members</span></span>
|<span data-ttu-id="d0def-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d0def-107">Member</span></span>|<span data-ttu-id="d0def-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d0def-108">Value</span></span>|<span data-ttu-id="d0def-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d0def-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0def-110">notApplicable</span><span class="sxs-lookup"><span data-stu-id="d0def-110">notApplicable</span></span>|<span data-ttu-id="d0def-111">0</span><span class="sxs-lookup"><span data-stu-id="d0def-111">0</span></span>|<span data-ttu-id="d0def-112">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="d0def-112">Not Applicable.</span></span>|
|<span data-ttu-id="d0def-113">установлен</span><span class="sxs-lookup"><span data-stu-id="d0def-113">installed</span></span>|<span data-ttu-id="d0def-114">1</span><span class="sxs-lookup"><span data-stu-id="d0def-114">1</span></span>|<span data-ttu-id="d0def-115">Установить.</span><span class="sxs-lookup"><span data-stu-id="d0def-115">Installed.</span></span>|
|<span data-ttu-id="d0def-116">failed</span><span class="sxs-lookup"><span data-stu-id="d0def-116">failed</span></span>|<span data-ttu-id="d0def-117">2</span><span class="sxs-lookup"><span data-stu-id="d0def-117">2</span></span>|<span data-ttu-id="d0def-118">Не удалось.</span><span class="sxs-lookup"><span data-stu-id="d0def-118">Failed.</span></span>|
|<span data-ttu-id="d0def-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="d0def-119">notInstalled</span></span>|<span data-ttu-id="d0def-120">3</span><span class="sxs-lookup"><span data-stu-id="d0def-120">3</span></span>|<span data-ttu-id="d0def-121">Не установлен.</span><span class="sxs-lookup"><span data-stu-id="d0def-121">Not Installed.</span></span>|
|<span data-ttu-id="d0def-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="d0def-122">uninstallFailed</span></span>|<span data-ttu-id="d0def-123">4</span><span class="sxs-lookup"><span data-stu-id="d0def-123">4</span></span>|<span data-ttu-id="d0def-124">Удаление не удалось.</span><span class="sxs-lookup"><span data-stu-id="d0def-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="d0def-125">unknown</span><span class="sxs-lookup"><span data-stu-id="d0def-125">unknown</span></span>|<span data-ttu-id="d0def-126">5</span><span class="sxs-lookup"><span data-stu-id="d0def-126">5</span></span>|<span data-ttu-id="d0def-127">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="d0def-127">Unknown.</span></span>|



