---
title: Тип перечисления resultantAppState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b97f8f9fc44faf0c27c31f8bab60103547fcf743
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947290"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="8d3c8-103">Тип перечисления resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8d3c8-103">resultantAppState enum type</span></span>

> <span data-ttu-id="8d3c8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d3c8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d3c8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d3c8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8d3c8-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="8d3c8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8d3c8-108">Members</span></span>
|<span data-ttu-id="8d3c8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8d3c8-109">Member</span></span>|<span data-ttu-id="8d3c8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8d3c8-110">Value</span></span>|<span data-ttu-id="8d3c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3c8-112">установлен</span><span class="sxs-lookup"><span data-stu-id="8d3c8-112">installed</span></span>|<span data-ttu-id="8d3c8-113">1</span><span class="sxs-lookup"><span data-stu-id="8d3c8-113">1</span></span>|<span data-ttu-id="8d3c8-114">Приложение устанавливается без ошибок</span><span class="sxs-lookup"><span data-stu-id="8d3c8-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="8d3c8-115">failed</span><span class="sxs-lookup"><span data-stu-id="8d3c8-115">failed</span></span>|<span data-ttu-id="8d3c8-116">2</span><span class="sxs-lookup"><span data-stu-id="8d3c8-116">2</span></span>|<span data-ttu-id="8d3c8-117">Сбой при установке приложения.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-117">The application failed to install.</span></span>|
|<span data-ttu-id="8d3c8-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="8d3c8-118">notInstalled</span></span>|<span data-ttu-id="8d3c8-119">3</span><span class="sxs-lookup"><span data-stu-id="8d3c8-119">3</span></span>|<span data-ttu-id="8d3c8-120">Приложение не установлено.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-120">The application is not installed.</span></span>|
|<span data-ttu-id="8d3c8-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="8d3c8-121">uninstallFailed</span></span>|<span data-ttu-id="8d3c8-122">4</span><span class="sxs-lookup"><span data-stu-id="8d3c8-122">4</span></span>|<span data-ttu-id="8d3c8-123">Не удалось удалить приложение.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="8d3c8-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="8d3c8-124">pendingInstall</span></span>|<span data-ttu-id="8d3c8-125">5</span><span class="sxs-lookup"><span data-stu-id="8d3c8-125">5</span></span>|<span data-ttu-id="8d3c8-126">Установка приложения находится в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="8d3c8-127">unknown</span><span class="sxs-lookup"><span data-stu-id="8d3c8-127">unknown</span></span>|<span data-ttu-id="8d3c8-128">99</span><span class="sxs-lookup"><span data-stu-id="8d3c8-128">99</span></span>|<span data-ttu-id="8d3c8-129">Состояние приложения не известен.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="8d3c8-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="8d3c8-130">notApplicable</span></span>|<span data-ttu-id="8d3c8-131">–1</span><span class="sxs-lookup"><span data-stu-id="8d3c8-131">-1</span></span>|<span data-ttu-id="8d3c8-132">Приложение не применяется.</span><span class="sxs-lookup"><span data-stu-id="8d3c8-132">The application is not applicable.</span></span>|





