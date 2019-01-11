---
title: Тип перечисления resultantAppState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14d5469f6bbc5b261d8a9eb1f11a8b0ebd118d44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838334"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="8dec5-103">Тип перечисления resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8dec5-103">resultantAppState enum type</span></span>

> <span data-ttu-id="8dec5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8dec5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dec5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dec5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8dec5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8dec5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dec5-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8dec5-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="8dec5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8dec5-108">Members</span></span>
|<span data-ttu-id="8dec5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8dec5-109">Member</span></span>|<span data-ttu-id="8dec5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8dec5-110">Value</span></span>|<span data-ttu-id="8dec5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8dec5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dec5-112">установлен</span><span class="sxs-lookup"><span data-stu-id="8dec5-112">installed</span></span>|<span data-ttu-id="8dec5-113">1</span><span class="sxs-lookup"><span data-stu-id="8dec5-113">1</span></span>|<span data-ttu-id="8dec5-114">Приложение устанавливается без ошибок</span><span class="sxs-lookup"><span data-stu-id="8dec5-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="8dec5-115">failed</span><span class="sxs-lookup"><span data-stu-id="8dec5-115">failed</span></span>|<span data-ttu-id="8dec5-116">2</span><span class="sxs-lookup"><span data-stu-id="8dec5-116">2</span></span>|<span data-ttu-id="8dec5-117">Сбой при установке приложения.</span><span class="sxs-lookup"><span data-stu-id="8dec5-117">The application failed to install.</span></span>|
|<span data-ttu-id="8dec5-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="8dec5-118">notInstalled</span></span>|<span data-ttu-id="8dec5-119">3</span><span class="sxs-lookup"><span data-stu-id="8dec5-119">3</span></span>|<span data-ttu-id="8dec5-120">Приложение не установлено.</span><span class="sxs-lookup"><span data-stu-id="8dec5-120">The application is not installed.</span></span>|
|<span data-ttu-id="8dec5-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="8dec5-121">uninstallFailed</span></span>|<span data-ttu-id="8dec5-122">4</span><span class="sxs-lookup"><span data-stu-id="8dec5-122">4</span></span>|<span data-ttu-id="8dec5-123">Не удалось удалить приложение.</span><span class="sxs-lookup"><span data-stu-id="8dec5-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="8dec5-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="8dec5-124">pendingInstall</span></span>|<span data-ttu-id="8dec5-125">5</span><span class="sxs-lookup"><span data-stu-id="8dec5-125">5</span></span>|<span data-ttu-id="8dec5-126">Установка приложения находится в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="8dec5-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="8dec5-127">unknown</span><span class="sxs-lookup"><span data-stu-id="8dec5-127">unknown</span></span>|<span data-ttu-id="8dec5-128">99</span><span class="sxs-lookup"><span data-stu-id="8dec5-128">99</span></span>|<span data-ttu-id="8dec5-129">Состояние приложения не известен.</span><span class="sxs-lookup"><span data-stu-id="8dec5-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="8dec5-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="8dec5-130">notApplicable</span></span>|<span data-ttu-id="8dec5-131">–1</span><span class="sxs-lookup"><span data-stu-id="8dec5-131">-1</span></span>|<span data-ttu-id="8dec5-132">Приложение не применяется.</span><span class="sxs-lookup"><span data-stu-id="8dec5-132">The application is not applicable.</span></span>|





