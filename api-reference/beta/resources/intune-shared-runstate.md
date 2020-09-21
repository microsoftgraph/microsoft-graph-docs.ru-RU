---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36022987fb96671399523a5936c7799e97db33c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084046"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="eeb9c-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="eeb9c-103">runState enum type</span></span>

<span data-ttu-id="eeb9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeb9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeb9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeb9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeb9c-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="eeb9c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="eeb9c-108">Members</span></span>
|<span data-ttu-id="eeb9c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="eeb9c-109">Member</span></span>|<span data-ttu-id="eeb9c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="eeb9c-110">Value</span></span>|<span data-ttu-id="eeb9c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeb9c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="eeb9c-112">unknown</span></span>|<span data-ttu-id="eeb9c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="eeb9c-113">0</span></span>|<span data-ttu-id="eeb9c-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-114">Unknown result.</span></span>|
|<span data-ttu-id="eeb9c-115">success</span><span class="sxs-lookup"><span data-stu-id="eeb9c-115">success</span></span>|<span data-ttu-id="eeb9c-116">1 </span><span class="sxs-lookup"><span data-stu-id="eeb9c-116">1</span></span>|<span data-ttu-id="eeb9c-117">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-117">Script is run successfully.</span></span>|
|<span data-ttu-id="eeb9c-118">сбой</span><span class="sxs-lookup"><span data-stu-id="eeb9c-118">fail</span></span>|<span data-ttu-id="eeb9c-119">2 </span><span class="sxs-lookup"><span data-stu-id="eeb9c-119">2</span></span>|<span data-ttu-id="eeb9c-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-120">Script failed to run.</span></span>|
|<span data-ttu-id="eeb9c-121">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="eeb9c-121">scriptError</span></span>|<span data-ttu-id="eeb9c-122">4</span><span class="sxs-lookup"><span data-stu-id="eeb9c-122">3</span></span>|<span data-ttu-id="eeb9c-123">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="eeb9c-124">закончен</span><span class="sxs-lookup"><span data-stu-id="eeb9c-124">pending</span></span>|<span data-ttu-id="eeb9c-125">4 </span><span class="sxs-lookup"><span data-stu-id="eeb9c-125">4</span></span>|<span data-ttu-id="eeb9c-126">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="eeb9c-127">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="eeb9c-127">notApplicable</span></span>|<span data-ttu-id="eeb9c-128">5 </span><span class="sxs-lookup"><span data-stu-id="eeb9c-128">5</span></span>|<span data-ttu-id="eeb9c-129">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="eeb9c-129">Script is not applicable for this device.</span></span>|






