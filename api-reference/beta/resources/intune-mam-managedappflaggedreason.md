---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 40a9d347a86df672f80ffe9b7aeda7f7f2750283
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43372933"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="f15ea-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="f15ea-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="f15ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f15ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f15ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f15ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f15ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f15ea-107">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="f15ea-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="f15ea-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f15ea-108">Members</span></span>
|<span data-ttu-id="f15ea-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f15ea-109">Member</span></span>|<span data-ttu-id="f15ea-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f15ea-110">Value</span></span>|<span data-ttu-id="f15ea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f15ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f15ea-112">нет</span><span class="sxs-lookup"><span data-stu-id="f15ea-112">none</span></span>|<span data-ttu-id="f15ea-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f15ea-113">0</span></span>|<span data-ttu-id="f15ea-114">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="f15ea-114">No issue.</span></span>|
|<span data-ttu-id="f15ea-115">рутеддевице</span><span class="sxs-lookup"><span data-stu-id="f15ea-115">rootedDevice</span></span>|<span data-ttu-id="f15ea-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f15ea-116">1</span></span>|<span data-ttu-id="f15ea-117">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f15ea-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="f15ea-118">андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="f15ea-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="f15ea-119">2</span><span class="sxs-lookup"><span data-stu-id="f15ea-119">2</span></span>|<span data-ttu-id="f15ea-120">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="f15ea-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="f15ea-121">андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="f15ea-121">androidFactoryRomModified</span></span>|<span data-ttu-id="f15ea-122">4</span><span class="sxs-lookup"><span data-stu-id="f15ea-122">3</span></span>|<span data-ttu-id="f15ea-123">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="f15ea-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



