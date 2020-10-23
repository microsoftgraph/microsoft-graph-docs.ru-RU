---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ec8d3f9333393b946539d639c9cc9eeb30c6b027
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725157"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="d158d-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="d158d-103">runState enum type</span></span>

<span data-ttu-id="d158d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d158d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d158d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d158d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d158d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d158d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d158d-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d158d-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="d158d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d158d-108">Members</span></span>
|<span data-ttu-id="d158d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d158d-109">Member</span></span>|<span data-ttu-id="d158d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d158d-110">Value</span></span>|<span data-ttu-id="d158d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d158d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d158d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d158d-112">unknown</span></span>|<span data-ttu-id="d158d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d158d-113">0</span></span>|<span data-ttu-id="d158d-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="d158d-114">Unknown result.</span></span>|
|<span data-ttu-id="d158d-115">success</span><span class="sxs-lookup"><span data-stu-id="d158d-115">success</span></span>|<span data-ttu-id="d158d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d158d-116">1</span></span>|<span data-ttu-id="d158d-117">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="d158d-117">Script is run successfully.</span></span>|
|<span data-ttu-id="d158d-118">сбой</span><span class="sxs-lookup"><span data-stu-id="d158d-118">fail</span></span>|<span data-ttu-id="d158d-119">2</span><span class="sxs-lookup"><span data-stu-id="d158d-119">2</span></span>|<span data-ttu-id="d158d-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="d158d-120">Script failed to run.</span></span>|
|<span data-ttu-id="d158d-121">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="d158d-121">scriptError</span></span>|<span data-ttu-id="d158d-122">4</span><span class="sxs-lookup"><span data-stu-id="d158d-122">3</span></span>|<span data-ttu-id="d158d-123">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="d158d-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="d158d-124">закончен</span><span class="sxs-lookup"><span data-stu-id="d158d-124">pending</span></span>|<span data-ttu-id="d158d-125">4 </span><span class="sxs-lookup"><span data-stu-id="d158d-125">4</span></span>|<span data-ttu-id="d158d-126">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="d158d-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="d158d-127">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="d158d-127">notApplicable</span></span>|<span data-ttu-id="d158d-128">5 </span><span class="sxs-lookup"><span data-stu-id="d158d-128">5</span></span>|<span data-ttu-id="d158d-129">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="d158d-129">Script is not applicable for this device.</span></span>|





