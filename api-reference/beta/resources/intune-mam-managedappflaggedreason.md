---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8068a97b543f72acc0be818769b0e522c306437e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967996"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="880c0-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="880c0-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="880c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="880c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="880c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="880c0-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="880c0-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="880c0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="880c0-107">Members</span></span>
|<span data-ttu-id="880c0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="880c0-108">Member</span></span>|<span data-ttu-id="880c0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="880c0-109">Value</span></span>|<span data-ttu-id="880c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="880c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880c0-111">none</span><span class="sxs-lookup"><span data-stu-id="880c0-111">none</span></span>|<span data-ttu-id="880c0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="880c0-112">0</span></span>|<span data-ttu-id="880c0-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="880c0-113">No issue.</span></span>|
|<span data-ttu-id="880c0-114">Рутеддевице</span><span class="sxs-lookup"><span data-stu-id="880c0-114">rootedDevice</span></span>|<span data-ttu-id="880c0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="880c0-115">1</span></span>|<span data-ttu-id="880c0-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="880c0-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="880c0-117">Андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="880c0-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="880c0-118">2</span><span class="sxs-lookup"><span data-stu-id="880c0-118">2</span></span>|<span data-ttu-id="880c0-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="880c0-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="880c0-120">Андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="880c0-120">androidFactoryRomModified</span></span>|<span data-ttu-id="880c0-121">4</span><span class="sxs-lookup"><span data-stu-id="880c0-121">3</span></span>|<span data-ttu-id="880c0-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="880c0-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





