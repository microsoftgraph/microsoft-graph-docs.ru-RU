---
title: Тип перечисления macOSGatekeeperAppSources
description: Параметры исходного приложения macOS Привратник.
ms.openlocfilehash: 97e8159c575c99fe142b67b4c6eeb24642cd0754
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080596"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="8dc7a-103">Тип перечисления macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="8dc7a-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="8dc7a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dc7a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8dc7a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dc7a-107">Параметры исходного приложения macOS Привратник.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="8dc7a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8dc7a-108">Members</span></span>
|<span data-ttu-id="8dc7a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8dc7a-109">Member</span></span>|<span data-ttu-id="8dc7a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8dc7a-110">Value</span></span>|<span data-ttu-id="8dc7a-111">Description</span><span class="sxs-lookup"><span data-stu-id="8dc7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc7a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8dc7a-112">notConfigured</span></span>|<span data-ttu-id="8dc7a-113">0</span><span class="sxs-lookup"><span data-stu-id="8dc7a-113">0</span></span>|<span data-ttu-id="8dc7a-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="8dc7a-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="8dc7a-115">macAppStore</span></span>|<span data-ttu-id="8dc7a-116">1</span><span class="sxs-lookup"><span data-stu-id="8dc7a-116">1</span></span>|<span data-ttu-id="8dc7a-117">Можно выполнять только приложения из Mac AppStore.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="8dc7a-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="8dc7a-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="8dc7a-119">2</span><span class="sxs-lookup"><span data-stu-id="8dc7a-119">2</span></span>|<span data-ttu-id="8dc7a-120">Можно выполнять только приложения из Mac AppStore и разработчиков (en) определенного.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="8dc7a-121">в любом месте</span><span class="sxs-lookup"><span data-stu-id="8dc7a-121">anywhere</span></span>|<span data-ttu-id="8dc7a-122">3</span><span class="sxs-lookup"><span data-stu-id="8dc7a-122">3</span></span>|<span data-ttu-id="8dc7a-123">Приложения в любом месте можно запускать.</span><span class="sxs-lookup"><span data-stu-id="8dc7a-123">Apps from anywhere can be run.</span></span>|





