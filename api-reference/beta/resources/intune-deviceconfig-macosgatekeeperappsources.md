---
title: Тип перечисления macOSGatekeeperAppSources
description: Параметры исходного приложения macOS Привратник.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 18ab6884d211faccb81e93a40ee91f742d03475f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394392"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="354a4-103">Тип перечисления macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="354a4-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="354a4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="354a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="354a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="354a4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="354a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="354a4-107">Параметры исходного приложения macOS Привратник.</span><span class="sxs-lookup"><span data-stu-id="354a4-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="354a4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="354a4-108">Members</span></span>
|<span data-ttu-id="354a4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="354a4-109">Member</span></span>|<span data-ttu-id="354a4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="354a4-110">Value</span></span>|<span data-ttu-id="354a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="354a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="354a4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="354a4-112">notConfigured</span></span>|<span data-ttu-id="354a4-113">0</span><span class="sxs-lookup"><span data-stu-id="354a4-113">0</span></span>|<span data-ttu-id="354a4-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="354a4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="354a4-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="354a4-115">macAppStore</span></span>|<span data-ttu-id="354a4-116">1</span><span class="sxs-lookup"><span data-stu-id="354a4-116">1</span></span>|<span data-ttu-id="354a4-117">Можно выполнять только приложения из Mac AppStore.</span><span class="sxs-lookup"><span data-stu-id="354a4-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="354a4-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="354a4-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="354a4-119">2</span><span class="sxs-lookup"><span data-stu-id="354a4-119">2</span></span>|<span data-ttu-id="354a4-120">Можно выполнять только приложения из Mac AppStore и разработчиков (en) определенного.</span><span class="sxs-lookup"><span data-stu-id="354a4-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="354a4-121">в любом месте</span><span class="sxs-lookup"><span data-stu-id="354a4-121">anywhere</span></span>|<span data-ttu-id="354a4-122">3</span><span class="sxs-lookup"><span data-stu-id="354a4-122">3</span></span>|<span data-ttu-id="354a4-123">Приложения в любом месте можно запускать.</span><span class="sxs-lookup"><span data-stu-id="354a4-123">Apps from anywhere can be run.</span></span>|




