---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf3190ce35d56ef83d19368001175896cb794c01
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580822"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="7fd22-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="7fd22-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="7fd22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fd22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fd22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fd22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fd22-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="7fd22-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="7fd22-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7fd22-107">Members</span></span>
|<span data-ttu-id="7fd22-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7fd22-108">Member</span></span>|<span data-ttu-id="7fd22-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7fd22-109">Value</span></span>|<span data-ttu-id="7fd22-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7fd22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fd22-111">Нет</span><span class="sxs-lookup"><span data-stu-id="7fd22-111">none</span></span>|<span data-ttu-id="7fd22-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7fd22-112">0</span></span>|<span data-ttu-id="7fd22-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="7fd22-113">No issue.</span></span>|
|<span data-ttu-id="7fd22-114">Рутеддевице</span><span class="sxs-lookup"><span data-stu-id="7fd22-114">rootedDevice</span></span>|<span data-ttu-id="7fd22-115">1 </span><span class="sxs-lookup"><span data-stu-id="7fd22-115">1</span></span>|<span data-ttu-id="7fd22-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="7fd22-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="7fd22-117">Андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="7fd22-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="7fd22-118">2 </span><span class="sxs-lookup"><span data-stu-id="7fd22-118">2</span></span>|<span data-ttu-id="7fd22-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="7fd22-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="7fd22-120">Андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="7fd22-120">androidFactoryRomModified</span></span>|<span data-ttu-id="7fd22-121">3 </span><span class="sxs-lookup"><span data-stu-id="7fd22-121">3</span></span>|<span data-ttu-id="7fd22-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="7fd22-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





