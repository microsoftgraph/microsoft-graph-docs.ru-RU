---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fef95d2d5744d0cdc6b92328b15a44f8b21c6cb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523550"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="61bee-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="61bee-103">runState enum type</span></span>

<span data-ttu-id="61bee-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61bee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61bee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61bee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61bee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61bee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61bee-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="61bee-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="61bee-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="61bee-108">Members</span></span>
|<span data-ttu-id="61bee-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="61bee-109">Member</span></span>|<span data-ttu-id="61bee-110">Значение</span><span class="sxs-lookup"><span data-stu-id="61bee-110">Value</span></span>|<span data-ttu-id="61bee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61bee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61bee-112">unknown</span><span class="sxs-lookup"><span data-stu-id="61bee-112">unknown</span></span>|<span data-ttu-id="61bee-113">нуль</span><span class="sxs-lookup"><span data-stu-id="61bee-113">0</span></span>|<span data-ttu-id="61bee-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="61bee-114">Unknown result.</span></span>|
|<span data-ttu-id="61bee-115">success</span><span class="sxs-lookup"><span data-stu-id="61bee-115">success</span></span>|<span data-ttu-id="61bee-116">1 </span><span class="sxs-lookup"><span data-stu-id="61bee-116">1</span></span>|<span data-ttu-id="61bee-117">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="61bee-117">Script is run successfully.</span></span>|
|<span data-ttu-id="61bee-118">сбой</span><span class="sxs-lookup"><span data-stu-id="61bee-118">fail</span></span>|<span data-ttu-id="61bee-119">2 </span><span class="sxs-lookup"><span data-stu-id="61bee-119">2</span></span>|<span data-ttu-id="61bee-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="61bee-120">Script failed to run.</span></span>|
|<span data-ttu-id="61bee-121">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="61bee-121">scriptError</span></span>|<span data-ttu-id="61bee-122">3 </span><span class="sxs-lookup"><span data-stu-id="61bee-122">3</span></span>|<span data-ttu-id="61bee-123">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="61bee-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="61bee-124">закончен</span><span class="sxs-lookup"><span data-stu-id="61bee-124">pending</span></span>|<span data-ttu-id="61bee-125">4 </span><span class="sxs-lookup"><span data-stu-id="61bee-125">4</span></span>|<span data-ttu-id="61bee-126">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="61bee-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="61bee-127">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="61bee-127">notApplicable</span></span>|<span data-ttu-id="61bee-128">5 </span><span class="sxs-lookup"><span data-stu-id="61bee-128">5</span></span>|<span data-ttu-id="61bee-129">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="61bee-129">Script is not applicable for this device.</span></span>|



