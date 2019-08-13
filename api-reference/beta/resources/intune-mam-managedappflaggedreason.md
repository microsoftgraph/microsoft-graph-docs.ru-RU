---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7aedda5d89d41ba936651c10d81ceeb33dfe603a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332129"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="5c275-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="5c275-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="5c275-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c275-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c275-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c275-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c275-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="5c275-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="5c275-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c275-107">Members</span></span>
|<span data-ttu-id="5c275-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c275-108">Member</span></span>|<span data-ttu-id="5c275-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5c275-109">Value</span></span>|<span data-ttu-id="5c275-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c275-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c275-111">none</span><span class="sxs-lookup"><span data-stu-id="5c275-111">none</span></span>|<span data-ttu-id="5c275-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5c275-112">0</span></span>|<span data-ttu-id="5c275-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="5c275-113">No issue.</span></span>|
|<span data-ttu-id="5c275-114">рутеддевице</span><span class="sxs-lookup"><span data-stu-id="5c275-114">rootedDevice</span></span>|<span data-ttu-id="5c275-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5c275-115">1</span></span>|<span data-ttu-id="5c275-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="5c275-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="5c275-117">андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="5c275-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="5c275-118">2</span><span class="sxs-lookup"><span data-stu-id="5c275-118">2</span></span>|<span data-ttu-id="5c275-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="5c275-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="5c275-120">андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="5c275-120">androidFactoryRomModified</span></span>|<span data-ttu-id="5c275-121">4</span><span class="sxs-lookup"><span data-stu-id="5c275-121">3</span></span>|<span data-ttu-id="5c275-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="5c275-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



