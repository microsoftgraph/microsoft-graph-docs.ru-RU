---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e2e8d473ba1dad1db8cd53d990a4cd8150b5544
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940745"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="c23bc-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="c23bc-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="c23bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c23bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c23bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c23bc-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="c23bc-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="c23bc-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c23bc-107">Members</span></span>
|<span data-ttu-id="c23bc-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c23bc-108">Member</span></span>|<span data-ttu-id="c23bc-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c23bc-109">Value</span></span>|<span data-ttu-id="c23bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c23bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c23bc-111">none</span><span class="sxs-lookup"><span data-stu-id="c23bc-111">none</span></span>|<span data-ttu-id="c23bc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c23bc-112">0</span></span>|<span data-ttu-id="c23bc-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="c23bc-113">No issue.</span></span>|
|<span data-ttu-id="c23bc-114">Рутеддевице</span><span class="sxs-lookup"><span data-stu-id="c23bc-114">rootedDevice</span></span>|<span data-ttu-id="c23bc-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c23bc-115">1</span></span>|<span data-ttu-id="c23bc-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c23bc-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="c23bc-117">Андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="c23bc-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="c23bc-118">2</span><span class="sxs-lookup"><span data-stu-id="c23bc-118">2</span></span>|<span data-ttu-id="c23bc-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="c23bc-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="c23bc-120">Андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="c23bc-120">androidFactoryRomModified</span></span>|<span data-ttu-id="c23bc-121">4</span><span class="sxs-lookup"><span data-stu-id="c23bc-121">3</span></span>|<span data-ttu-id="c23bc-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="c23bc-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




