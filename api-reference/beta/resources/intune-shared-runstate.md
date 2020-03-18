---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f4c1605734afef3caefc4b51e2c8a826d2f2cd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767822"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="cb71c-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="cb71c-103">runState enum type</span></span>

> <span data-ttu-id="cb71c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb71c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb71c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb71c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb71c-106">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb71c-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="cb71c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cb71c-107">Members</span></span>
|<span data-ttu-id="cb71c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cb71c-108">Member</span></span>|<span data-ttu-id="cb71c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cb71c-109">Value</span></span>|<span data-ttu-id="cb71c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cb71c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb71c-111">unknown</span><span class="sxs-lookup"><span data-stu-id="cb71c-111">unknown</span></span>|<span data-ttu-id="cb71c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cb71c-112">0</span></span>|<span data-ttu-id="cb71c-113">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="cb71c-113">Unknown result.</span></span>|
|<span data-ttu-id="cb71c-114">success</span><span class="sxs-lookup"><span data-stu-id="cb71c-114">success</span></span>|<span data-ttu-id="cb71c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cb71c-115">1</span></span>|<span data-ttu-id="cb71c-116">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="cb71c-116">Script is run successfully.</span></span>|
|<span data-ttu-id="cb71c-117">сбой</span><span class="sxs-lookup"><span data-stu-id="cb71c-117">fail</span></span>|<span data-ttu-id="cb71c-118">2</span><span class="sxs-lookup"><span data-stu-id="cb71c-118">2</span></span>|<span data-ttu-id="cb71c-119">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="cb71c-119">Script failed to run.</span></span>|
|<span data-ttu-id="cb71c-120">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="cb71c-120">scriptError</span></span>|<span data-ttu-id="cb71c-121">4</span><span class="sxs-lookup"><span data-stu-id="cb71c-121">3</span></span>|<span data-ttu-id="cb71c-122">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="cb71c-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="cb71c-123">закончен</span><span class="sxs-lookup"><span data-stu-id="cb71c-123">pending</span></span>|<span data-ttu-id="cb71c-124">4 </span><span class="sxs-lookup"><span data-stu-id="cb71c-124">4</span></span>|<span data-ttu-id="cb71c-125">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="cb71c-125">Script is pending to execute.</span></span>|
|<span data-ttu-id="cb71c-126">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="cb71c-126">notApplicable</span></span>|<span data-ttu-id="cb71c-127">5 </span><span class="sxs-lookup"><span data-stu-id="cb71c-127">5</span></span>|<span data-ttu-id="cb71c-128">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="cb71c-128">Script is not applicable for this device.</span></span>|



