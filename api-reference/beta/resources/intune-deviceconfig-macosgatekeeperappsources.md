---
title: Тип перечисления macOSGatekeeperAppSources
description: Параметры исходного приложения macOS Привратник.
author: tfitzmac
ms.openlocfilehash: 323c913cf9136e26a060d98e399806370700094d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342835"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="bf656-103">Тип перечисления macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="bf656-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="bf656-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf656-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf656-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf656-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf656-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf656-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf656-107">Параметры исходного приложения macOS Привратник.</span><span class="sxs-lookup"><span data-stu-id="bf656-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="bf656-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf656-108">Members</span></span>
|<span data-ttu-id="bf656-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf656-109">Member</span></span>|<span data-ttu-id="bf656-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bf656-110">Value</span></span>|<span data-ttu-id="bf656-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf656-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf656-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bf656-112">notConfigured</span></span>|<span data-ttu-id="bf656-113">0</span><span class="sxs-lookup"><span data-stu-id="bf656-113">0</span></span>|<span data-ttu-id="bf656-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="bf656-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="bf656-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="bf656-115">macAppStore</span></span>|<span data-ttu-id="bf656-116">1</span><span class="sxs-lookup"><span data-stu-id="bf656-116">1</span></span>|<span data-ttu-id="bf656-117">Можно выполнять только приложения из Mac AppStore.</span><span class="sxs-lookup"><span data-stu-id="bf656-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="bf656-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="bf656-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="bf656-119">2</span><span class="sxs-lookup"><span data-stu-id="bf656-119">2</span></span>|<span data-ttu-id="bf656-120">Можно выполнять только приложения из Mac AppStore и разработчиков (en) определенного.</span><span class="sxs-lookup"><span data-stu-id="bf656-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="bf656-121">в любом месте</span><span class="sxs-lookup"><span data-stu-id="bf656-121">anywhere</span></span>|<span data-ttu-id="bf656-122">3</span><span class="sxs-lookup"><span data-stu-id="bf656-122">3</span></span>|<span data-ttu-id="bf656-123">Приложения в любом месте можно запускать.</span><span class="sxs-lookup"><span data-stu-id="bf656-123">Apps from anywhere can be run.</span></span>|





