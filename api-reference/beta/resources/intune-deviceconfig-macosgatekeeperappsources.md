---
title: Тип перечисления macOSGatekeeperAppSources
description: Параметры исходного приложения macOS Привратник.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c2c1d553408b7269a53f9fc3500493a44bc3645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918117"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="f2637-103">Тип перечисления macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="f2637-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="f2637-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2637-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2637-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2637-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2637-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f2637-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2637-107">Параметры исходного приложения macOS Привратник.</span><span class="sxs-lookup"><span data-stu-id="f2637-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="f2637-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f2637-108">Members</span></span>
|<span data-ttu-id="f2637-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f2637-109">Member</span></span>|<span data-ttu-id="f2637-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f2637-110">Value</span></span>|<span data-ttu-id="f2637-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2637-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2637-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f2637-112">notConfigured</span></span>|<span data-ttu-id="f2637-113">0</span><span class="sxs-lookup"><span data-stu-id="f2637-113">0</span></span>|<span data-ttu-id="f2637-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="f2637-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f2637-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="f2637-115">macAppStore</span></span>|<span data-ttu-id="f2637-116">1</span><span class="sxs-lookup"><span data-stu-id="f2637-116">1</span></span>|<span data-ttu-id="f2637-117">Можно выполнять только приложения из Mac AppStore.</span><span class="sxs-lookup"><span data-stu-id="f2637-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="f2637-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="f2637-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="f2637-119">2</span><span class="sxs-lookup"><span data-stu-id="f2637-119">2</span></span>|<span data-ttu-id="f2637-120">Можно выполнять только приложения из Mac AppStore и разработчиков (en) определенного.</span><span class="sxs-lookup"><span data-stu-id="f2637-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="f2637-121">в любом месте</span><span class="sxs-lookup"><span data-stu-id="f2637-121">anywhere</span></span>|<span data-ttu-id="f2637-122">3</span><span class="sxs-lookup"><span data-stu-id="f2637-122">3</span></span>|<span data-ttu-id="f2637-123">Приложения в любом месте можно запускать.</span><span class="sxs-lookup"><span data-stu-id="f2637-123">Apps from anywhere can be run.</span></span>|





