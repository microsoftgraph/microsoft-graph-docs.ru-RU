---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612296"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="891c7-103">тип runState enum</span><span class="sxs-lookup"><span data-stu-id="891c7-103">runState enum type</span></span>

<span data-ttu-id="891c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="891c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="891c7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="891c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891c7-107">Указывает тип выполнения сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="891c7-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="891c7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="891c7-108">Members</span></span>
|<span data-ttu-id="891c7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="891c7-109">Member</span></span>|<span data-ttu-id="891c7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="891c7-110">Value</span></span>|<span data-ttu-id="891c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="891c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891c7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="891c7-112">unknown</span></span>|<span data-ttu-id="891c7-113">0</span><span class="sxs-lookup"><span data-stu-id="891c7-113">0</span></span>|<span data-ttu-id="891c7-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="891c7-114">Unknown result.</span></span>|
|<span data-ttu-id="891c7-115">success</span><span class="sxs-lookup"><span data-stu-id="891c7-115">success</span></span>|<span data-ttu-id="891c7-116">1</span><span class="sxs-lookup"><span data-stu-id="891c7-116">1</span></span>|<span data-ttu-id="891c7-117">Скрипт успешно работает.</span><span class="sxs-lookup"><span data-stu-id="891c7-117">Script is run successfully.</span></span>|
|<span data-ttu-id="891c7-118">сбой</span><span class="sxs-lookup"><span data-stu-id="891c7-118">fail</span></span>|<span data-ttu-id="891c7-119">2</span><span class="sxs-lookup"><span data-stu-id="891c7-119">2</span></span>|<span data-ttu-id="891c7-120">Сценарий не удалось выполнить.</span><span class="sxs-lookup"><span data-stu-id="891c7-120">Script failed to run.</span></span>|
|<span data-ttu-id="891c7-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="891c7-121">scriptError</span></span>|<span data-ttu-id="891c7-122">3</span><span class="sxs-lookup"><span data-stu-id="891c7-122">3</span></span>|<span data-ttu-id="891c7-123">Скрипт обнаружения попадает в ошибку.</span><span class="sxs-lookup"><span data-stu-id="891c7-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="891c7-124">ожидание</span><span class="sxs-lookup"><span data-stu-id="891c7-124">pending</span></span>|<span data-ttu-id="891c7-125">4 </span><span class="sxs-lookup"><span data-stu-id="891c7-125">4</span></span>|<span data-ttu-id="891c7-126">Скрипт находится в ожидании выполнения.</span><span class="sxs-lookup"><span data-stu-id="891c7-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="891c7-127">notApplicable</span><span class="sxs-lookup"><span data-stu-id="891c7-127">notApplicable</span></span>|<span data-ttu-id="891c7-128">5 </span><span class="sxs-lookup"><span data-stu-id="891c7-128">5</span></span>|<span data-ttu-id="891c7-129">Скрипт для этого устройства не применяется.</span><span class="sxs-lookup"><span data-stu-id="891c7-129">Script is not applicable for this device.</span></span>|




