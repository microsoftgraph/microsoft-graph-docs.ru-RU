---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf3190ce35d56ef83d19368001175896cb794c01
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772372"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="529dd-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="529dd-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="529dd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="529dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="529dd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="529dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="529dd-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="529dd-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="529dd-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="529dd-107">Members</span></span>
|<span data-ttu-id="529dd-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="529dd-108">Member</span></span>|<span data-ttu-id="529dd-109">Значение</span><span class="sxs-lookup"><span data-stu-id="529dd-109">Value</span></span>|<span data-ttu-id="529dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="529dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="529dd-111">нет</span><span class="sxs-lookup"><span data-stu-id="529dd-111">none</span></span>|<span data-ttu-id="529dd-112">нуль</span><span class="sxs-lookup"><span data-stu-id="529dd-112">0</span></span>|<span data-ttu-id="529dd-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="529dd-113">No issue.</span></span>|
|<span data-ttu-id="529dd-114">Рутеддевице</span><span class="sxs-lookup"><span data-stu-id="529dd-114">rootedDevice</span></span>|<span data-ttu-id="529dd-115">1,1</span><span class="sxs-lookup"><span data-stu-id="529dd-115">1</span></span>|<span data-ttu-id="529dd-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="529dd-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="529dd-117">Андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="529dd-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="529dd-118">2</span><span class="sxs-lookup"><span data-stu-id="529dd-118">2</span></span>|<span data-ttu-id="529dd-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="529dd-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="529dd-120">Андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="529dd-120">androidFactoryRomModified</span></span>|<span data-ttu-id="529dd-121">4</span><span class="sxs-lookup"><span data-stu-id="529dd-121">3</span></span>|<span data-ttu-id="529dd-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="529dd-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





