---
title: тип перечисления Манажедаппфлагжедреасон
description: Причина, по которой пользователю был применен флаг
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bfe1ee2fe8385150336bef52ba2e498832b60562
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684542"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="867e7-103">тип перечисления Манажедаппфлагжедреасон</span><span class="sxs-lookup"><span data-stu-id="867e7-103">managedAppFlaggedReason enum type</span></span>

<span data-ttu-id="867e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="867e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="867e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="867e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="867e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="867e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="867e7-107">Причина, по которой пользователю был применен флаг</span><span class="sxs-lookup"><span data-stu-id="867e7-107">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="867e7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="867e7-108">Members</span></span>
|<span data-ttu-id="867e7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="867e7-109">Member</span></span>|<span data-ttu-id="867e7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="867e7-110">Value</span></span>|<span data-ttu-id="867e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="867e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867e7-112">none</span><span class="sxs-lookup"><span data-stu-id="867e7-112">none</span></span>|<span data-ttu-id="867e7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="867e7-113">0</span></span>|<span data-ttu-id="867e7-114">Нет ошибок.</span><span class="sxs-lookup"><span data-stu-id="867e7-114">No issue.</span></span>|
|<span data-ttu-id="867e7-115">рутеддевице</span><span class="sxs-lookup"><span data-stu-id="867e7-115">rootedDevice</span></span>|<span data-ttu-id="867e7-116">1,1</span><span class="sxs-lookup"><span data-stu-id="867e7-116">1</span></span>|<span data-ttu-id="867e7-117">Регистрация приложения выполняется на корневом/незаблокированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="867e7-117">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="867e7-118">андроидбутлоадерунлоккед</span><span class="sxs-lookup"><span data-stu-id="867e7-118">androidBootloaderUnlocked</span></span>|<span data-ttu-id="867e7-119">2</span><span class="sxs-lookup"><span data-stu-id="867e7-119">2</span></span>|<span data-ttu-id="867e7-120">Регистрация приложения выполняется на устройстве с Android, на котором разблокирован загрузчик.</span><span class="sxs-lookup"><span data-stu-id="867e7-120">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="867e7-121">андроидфакторироммодифиед</span><span class="sxs-lookup"><span data-stu-id="867e7-121">androidFactoryRomModified</span></span>|<span data-ttu-id="867e7-122">4</span><span class="sxs-lookup"><span data-stu-id="867e7-122">3</span></span>|<span data-ttu-id="867e7-123">Регистрация приложения выполняется на устройстве с Android, на котором было изменено фабричное ПЗУ.</span><span class="sxs-lookup"><span data-stu-id="867e7-123">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|





