---
title: Тип перечисления resultantAppState
description: Н/Д
ms.openlocfilehash: 7c3dd96aca4ed94a45a36b9a48a2908f805bb1f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081573"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="d7af9-103">Тип перечисления resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d7af9-103">resultantAppState enum type</span></span>

> <span data-ttu-id="d7af9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7af9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7af9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7af9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7af9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7af9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7af9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d7af9-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="d7af9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d7af9-108">Members</span></span>
|<span data-ttu-id="d7af9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d7af9-109">Member</span></span>|<span data-ttu-id="d7af9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d7af9-110">Value</span></span>|<span data-ttu-id="d7af9-111">Description</span><span class="sxs-lookup"><span data-stu-id="d7af9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7af9-112">установлен</span><span class="sxs-lookup"><span data-stu-id="d7af9-112">installed</span></span>|<span data-ttu-id="d7af9-113">1</span><span class="sxs-lookup"><span data-stu-id="d7af9-113">1</span></span>|<span data-ttu-id="d7af9-114">Приложение устанавливается без ошибок</span><span class="sxs-lookup"><span data-stu-id="d7af9-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="d7af9-115">failed</span><span class="sxs-lookup"><span data-stu-id="d7af9-115">failed</span></span>|<span data-ttu-id="d7af9-116">2</span><span class="sxs-lookup"><span data-stu-id="d7af9-116">2</span></span>|<span data-ttu-id="d7af9-117">Сбой при установке приложения.</span><span class="sxs-lookup"><span data-stu-id="d7af9-117">The application failed to install.</span></span>|
|<span data-ttu-id="d7af9-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="d7af9-118">notInstalled</span></span>|<span data-ttu-id="d7af9-119">3</span><span class="sxs-lookup"><span data-stu-id="d7af9-119">3</span></span>|<span data-ttu-id="d7af9-120">Приложение не установлено.</span><span class="sxs-lookup"><span data-stu-id="d7af9-120">The application is not installed.</span></span>|
|<span data-ttu-id="d7af9-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="d7af9-121">uninstallFailed</span></span>|<span data-ttu-id="d7af9-122">4</span><span class="sxs-lookup"><span data-stu-id="d7af9-122">4</span></span>|<span data-ttu-id="d7af9-123">Не удалось удалить приложение.</span><span class="sxs-lookup"><span data-stu-id="d7af9-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="d7af9-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="d7af9-124">pendingInstall</span></span>|<span data-ttu-id="d7af9-125">5</span><span class="sxs-lookup"><span data-stu-id="d7af9-125">5</span></span>|<span data-ttu-id="d7af9-126">Установка приложения находится в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="d7af9-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="d7af9-127">unknown</span><span class="sxs-lookup"><span data-stu-id="d7af9-127">unknown</span></span>|<span data-ttu-id="d7af9-128">99</span><span class="sxs-lookup"><span data-stu-id="d7af9-128">99</span></span>|<span data-ttu-id="d7af9-129">Состояние приложения не известен.</span><span class="sxs-lookup"><span data-stu-id="d7af9-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="d7af9-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="d7af9-130">notApplicable</span></span>|<span data-ttu-id="d7af9-131">-1</span><span class="sxs-lookup"><span data-stu-id="d7af9-131">-1</span></span>|<span data-ttu-id="d7af9-132">Приложение не применяется.</span><span class="sxs-lookup"><span data-stu-id="d7af9-132">The application is not applicable.</span></span>|





