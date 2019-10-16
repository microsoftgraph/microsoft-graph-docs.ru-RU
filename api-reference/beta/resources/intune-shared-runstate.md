---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ecf868f77bc5460af95375ef88d73e7384ef4ccf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538702"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="fc09c-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="fc09c-103">runState enum type</span></span>

> <span data-ttu-id="fc09c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc09c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc09c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc09c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc09c-106">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="fc09c-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="fc09c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="fc09c-107">Members</span></span>
|<span data-ttu-id="fc09c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="fc09c-108">Member</span></span>|<span data-ttu-id="fc09c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="fc09c-109">Value</span></span>|<span data-ttu-id="fc09c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc09c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc09c-111">unknown</span><span class="sxs-lookup"><span data-stu-id="fc09c-111">unknown</span></span>|<span data-ttu-id="fc09c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="fc09c-112">0</span></span>|<span data-ttu-id="fc09c-113">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="fc09c-113">Unknown result.</span></span>|
|<span data-ttu-id="fc09c-114">success</span><span class="sxs-lookup"><span data-stu-id="fc09c-114">success</span></span>|<span data-ttu-id="fc09c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="fc09c-115">1</span></span>|<span data-ttu-id="fc09c-116">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="fc09c-116">Script is run successfully.</span></span>|
|<span data-ttu-id="fc09c-117">сбой</span><span class="sxs-lookup"><span data-stu-id="fc09c-117">fail</span></span>|<span data-ttu-id="fc09c-118">2</span><span class="sxs-lookup"><span data-stu-id="fc09c-118">2</span></span>|<span data-ttu-id="fc09c-119">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="fc09c-119">Script failed to run.</span></span>|
|<span data-ttu-id="fc09c-120">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="fc09c-120">scriptError</span></span>|<span data-ttu-id="fc09c-121">4</span><span class="sxs-lookup"><span data-stu-id="fc09c-121">3</span></span>|<span data-ttu-id="fc09c-122">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="fc09c-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="fc09c-123">закончен</span><span class="sxs-lookup"><span data-stu-id="fc09c-123">pending</span></span>|<span data-ttu-id="fc09c-124">4 </span><span class="sxs-lookup"><span data-stu-id="fc09c-124">4</span></span>|<span data-ttu-id="fc09c-125">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="fc09c-125">Script is pending to execute.</span></span>|
|<span data-ttu-id="fc09c-126">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="fc09c-126">notApplicable</span></span>|<span data-ttu-id="fc09c-127">5 </span><span class="sxs-lookup"><span data-stu-id="fc09c-127">5</span></span>|<span data-ttu-id="fc09c-128">Сценарий неприменим для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="fc09c-128">Script is not applicable for this device.</span></span>|



