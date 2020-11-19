---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255821"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="c7261-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="c7261-103">runState enum type</span></span>

<span data-ttu-id="c7261-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7261-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7261-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7261-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7261-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7261-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7261-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="c7261-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c7261-108">Members</span></span>
|<span data-ttu-id="c7261-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c7261-109">Member</span></span>|<span data-ttu-id="c7261-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c7261-110">Value</span></span>|<span data-ttu-id="c7261-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7261-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7261-112">unknown</span><span class="sxs-lookup"><span data-stu-id="c7261-112">unknown</span></span>|<span data-ttu-id="c7261-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c7261-113">0</span></span>|<span data-ttu-id="c7261-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="c7261-114">Unknown result.</span></span>|
|<span data-ttu-id="c7261-115">success</span><span class="sxs-lookup"><span data-stu-id="c7261-115">success</span></span>|<span data-ttu-id="c7261-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c7261-116">1</span></span>|<span data-ttu-id="c7261-117">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="c7261-117">Script is run successfully.</span></span>|
|<span data-ttu-id="c7261-118">сбой</span><span class="sxs-lookup"><span data-stu-id="c7261-118">fail</span></span>|<span data-ttu-id="c7261-119">2</span><span class="sxs-lookup"><span data-stu-id="c7261-119">2</span></span>|<span data-ttu-id="c7261-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="c7261-120">Script failed to run.</span></span>|
|<span data-ttu-id="c7261-121">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="c7261-121">scriptError</span></span>|<span data-ttu-id="c7261-122">4</span><span class="sxs-lookup"><span data-stu-id="c7261-122">3</span></span>|<span data-ttu-id="c7261-123">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="c7261-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="c7261-124">закончен</span><span class="sxs-lookup"><span data-stu-id="c7261-124">pending</span></span>|<span data-ttu-id="c7261-125">4 </span><span class="sxs-lookup"><span data-stu-id="c7261-125">4</span></span>|<span data-ttu-id="c7261-126">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="c7261-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="c7261-127">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="c7261-127">notApplicable</span></span>|<span data-ttu-id="c7261-128">5 </span><span class="sxs-lookup"><span data-stu-id="c7261-128">5</span></span>|<span data-ttu-id="c7261-129">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="c7261-129">Script is not applicable for this device.</span></span>|




