---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b07670130f386a5b4a3c53495464652aee7e686
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996290"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="b5aea-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="b5aea-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="b5aea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5aea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5aea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5aea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5aea-106">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="b5aea-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="b5aea-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b5aea-107">Members</span></span>
|<span data-ttu-id="b5aea-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b5aea-108">Member</span></span>|<span data-ttu-id="b5aea-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b5aea-109">Value</span></span>|<span data-ttu-id="b5aea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b5aea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5aea-111">none</span><span class="sxs-lookup"><span data-stu-id="b5aea-111">none</span></span>|<span data-ttu-id="b5aea-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b5aea-112">0</span></span>|<span data-ttu-id="b5aea-113">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="b5aea-113">No issue.</span></span>|
|<span data-ttu-id="b5aea-114">Рутеддевице</span><span class="sxs-lookup"><span data-stu-id="b5aea-114">rootedDevice</span></span>|<span data-ttu-id="b5aea-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b5aea-115">1</span></span>|<span data-ttu-id="b5aea-116">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="b5aea-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="b5aea-117">Андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="b5aea-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="b5aea-118">2</span><span class="sxs-lookup"><span data-stu-id="b5aea-118">2</span></span>|<span data-ttu-id="b5aea-119">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="b5aea-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="b5aea-120">Андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="b5aea-120">androidFactoryRomModified</span></span>|<span data-ttu-id="b5aea-121">4</span><span class="sxs-lookup"><span data-stu-id="b5aea-121">3</span></span>|<span data-ttu-id="b5aea-122">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="b5aea-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





