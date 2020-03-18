---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7c295fca92a3f9e7ba4836e96714e8b576784dca
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781917"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="708bf-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="708bf-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="708bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="708bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="708bf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="708bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="708bf-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="708bf-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="708bf-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="708bf-107">Members</span></span>
|<span data-ttu-id="708bf-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="708bf-108">Member</span></span>|<span data-ttu-id="708bf-109">Значение</span><span class="sxs-lookup"><span data-stu-id="708bf-109">Value</span></span>|<span data-ttu-id="708bf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="708bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708bf-111">none</span><span class="sxs-lookup"><span data-stu-id="708bf-111">none</span></span>|<span data-ttu-id="708bf-112">нуль</span><span class="sxs-lookup"><span data-stu-id="708bf-112">0</span></span>|<span data-ttu-id="708bf-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="708bf-113">No issue.</span></span>|
|<span data-ttu-id="708bf-114">рутеддевице</span><span class="sxs-lookup"><span data-stu-id="708bf-114">rootedDevice</span></span>|<span data-ttu-id="708bf-115">1,1</span><span class="sxs-lookup"><span data-stu-id="708bf-115">1</span></span>|<span data-ttu-id="708bf-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="708bf-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="708bf-117">андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="708bf-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="708bf-118">2</span><span class="sxs-lookup"><span data-stu-id="708bf-118">2</span></span>|<span data-ttu-id="708bf-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="708bf-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="708bf-120">андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="708bf-120">androidFactoryRomModified</span></span>|<span data-ttu-id="708bf-121">4</span><span class="sxs-lookup"><span data-stu-id="708bf-121">3</span></span>|<span data-ttu-id="708bf-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="708bf-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



