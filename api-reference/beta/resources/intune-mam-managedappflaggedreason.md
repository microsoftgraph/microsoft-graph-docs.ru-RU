---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64f78ca8a074d35687f50e232a104b87717a6462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527921"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="19cc8-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="19cc8-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="19cc8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19cc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19cc8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19cc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19cc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19cc8-107">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="19cc8-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="19cc8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="19cc8-108">Members</span></span>
|<span data-ttu-id="19cc8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="19cc8-109">Member</span></span>|<span data-ttu-id="19cc8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="19cc8-110">Value</span></span>|<span data-ttu-id="19cc8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19cc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19cc8-112">нет</span><span class="sxs-lookup"><span data-stu-id="19cc8-112">none</span></span>|<span data-ttu-id="19cc8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="19cc8-113">0</span></span>|<span data-ttu-id="19cc8-114">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="19cc8-114">No issue.</span></span>|
|<span data-ttu-id="19cc8-115">рутеддевице</span><span class="sxs-lookup"><span data-stu-id="19cc8-115">rootedDevice</span></span>|<span data-ttu-id="19cc8-116">1 </span><span class="sxs-lookup"><span data-stu-id="19cc8-116">1</span></span>|<span data-ttu-id="19cc8-117">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="19cc8-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="19cc8-118">андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="19cc8-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="19cc8-119">2 </span><span class="sxs-lookup"><span data-stu-id="19cc8-119">2</span></span>|<span data-ttu-id="19cc8-120">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="19cc8-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="19cc8-121">андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="19cc8-121">androidFactoryRomModified</span></span>|<span data-ttu-id="19cc8-122">3 </span><span class="sxs-lookup"><span data-stu-id="19cc8-122">3</span></span>|<span data-ttu-id="19cc8-123">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="19cc8-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



