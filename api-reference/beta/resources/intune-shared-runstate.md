---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d77f3ef9a2d7fd37edeaf2b4cc25d5e6d5bfcf4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347852"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="f602e-103">тип перечисления Рунстате</span><span class="sxs-lookup"><span data-stu-id="f602e-103">runState enum type</span></span>

> <span data-ttu-id="f602e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f602e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f602e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f602e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f602e-106">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f602e-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="f602e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f602e-107">Members</span></span>
|<span data-ttu-id="f602e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f602e-108">Member</span></span>|<span data-ttu-id="f602e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f602e-109">Value</span></span>|<span data-ttu-id="f602e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f602e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f602e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="f602e-111">unknown</span></span>|<span data-ttu-id="f602e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f602e-112">0</span></span>|<span data-ttu-id="f602e-113">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="f602e-113">Unknown result.</span></span>|
|<span data-ttu-id="f602e-114">success</span><span class="sxs-lookup"><span data-stu-id="f602e-114">success</span></span>|<span data-ttu-id="f602e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f602e-115">1</span></span>|<span data-ttu-id="f602e-116">Сценарий успешно запущен.</span><span class="sxs-lookup"><span data-stu-id="f602e-116">Script is run successfully.</span></span>|
|<span data-ttu-id="f602e-117">сбой</span><span class="sxs-lookup"><span data-stu-id="f602e-117">fail</span></span>|<span data-ttu-id="f602e-118">2</span><span class="sxs-lookup"><span data-stu-id="f602e-118">2</span></span>|<span data-ttu-id="f602e-119">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="f602e-119">Script failed to run.</span></span>|
|<span data-ttu-id="f602e-120">error</span><span class="sxs-lookup"><span data-stu-id="f602e-120">error</span></span>|<span data-ttu-id="f602e-121">4</span><span class="sxs-lookup"><span data-stu-id="f602e-121">3</span></span>|<span data-ttu-id="f602e-122">Ошибка при обращении к скрипту обнаружения.</span><span class="sxs-lookup"><span data-stu-id="f602e-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="f602e-123">закончен</span><span class="sxs-lookup"><span data-stu-id="f602e-123">pending</span></span>|<span data-ttu-id="f602e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="f602e-124">4</span></span>|<span data-ttu-id="f602e-125">Сценарий находится в состоянии ожидания выполнения.</span><span class="sxs-lookup"><span data-stu-id="f602e-125">Script is pending to execute.</span></span>|



