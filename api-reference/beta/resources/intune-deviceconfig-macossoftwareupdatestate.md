---
title: тип перечисления Макоссофтвареупдатестате
description: Состояние обновления программного обеспечения MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 05d2d951d8eacb93d952e20f01af6e42b30eecc1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731080"
---
# <a name="macossoftwareupdatestate-enum-type"></a><span data-ttu-id="2f2c0-103">тип перечисления Макоссофтвареупдатестате</span><span class="sxs-lookup"><span data-stu-id="2f2c0-103">macOSSoftwareUpdateState enum type</span></span>

<span data-ttu-id="2f2c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f2c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f2c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f2c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f2c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2c0-107">Состояние обновления программного обеспечения MacOS</span><span class="sxs-lookup"><span data-stu-id="2f2c0-107">MacOS Software Update State</span></span>

## <a name="members"></a><span data-ttu-id="2f2c0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2f2c0-108">Members</span></span>
|<span data-ttu-id="2f2c0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2f2c0-109">Member</span></span>|<span data-ttu-id="2f2c0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2f2c0-110">Value</span></span>|<span data-ttu-id="2f2c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2c0-112">success</span><span class="sxs-lookup"><span data-stu-id="2f2c0-112">success</span></span>|<span data-ttu-id="2f2c0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2f2c0-113">0</span></span>|<span data-ttu-id="2f2c0-114">Обновление программного обеспечения успешно установлено</span><span class="sxs-lookup"><span data-stu-id="2f2c0-114">The software update successfully installed</span></span>|
|<span data-ttu-id="2f2c0-115">скачивание</span><span class="sxs-lookup"><span data-stu-id="2f2c0-115">downloading</span></span>|<span data-ttu-id="2f2c0-116">1000</span><span class="sxs-lookup"><span data-stu-id="2f2c0-116">1000</span></span>|<span data-ttu-id="2f2c0-117">Идет скачивание обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="2f2c0-117">The software update is being downloaded</span></span>|
|<span data-ttu-id="2f2c0-118">загрузить</span><span class="sxs-lookup"><span data-stu-id="2f2c0-118">downloaded</span></span>|<span data-ttu-id="2f2c0-119">1001</span><span class="sxs-lookup"><span data-stu-id="2f2c0-119">1001</span></span>|<span data-ttu-id="2f2c0-120">Обновление программного обеспечения Загружено</span><span class="sxs-lookup"><span data-stu-id="2f2c0-120">The software update has been downloaded</span></span>|
|<span data-ttu-id="2f2c0-121">устанавливать</span><span class="sxs-lookup"><span data-stu-id="2f2c0-121">installing</span></span>|<span data-ttu-id="2f2c0-122">1002</span><span class="sxs-lookup"><span data-stu-id="2f2c0-122">1002</span></span>|<span data-ttu-id="2f2c0-123">Выполняется установка обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="2f2c0-123">The software update is being installed</span></span>|
|<span data-ttu-id="2f2c0-124">простоя</span><span class="sxs-lookup"><span data-stu-id="2f2c0-124">idle</span></span>|<span data-ttu-id="2f2c0-125">1003</span><span class="sxs-lookup"><span data-stu-id="2f2c0-125">1003</span></span>|<span data-ttu-id="2f2c0-126">Для этого обновления программного обеспечения не выполняется никаких действий</span><span class="sxs-lookup"><span data-stu-id="2f2c0-126">No action is being taken on this software update</span></span>|
|<span data-ttu-id="2f2c0-127">доступен</span><span class="sxs-lookup"><span data-stu-id="2f2c0-127">available</span></span>|<span data-ttu-id="2f2c0-128">1004</span><span class="sxs-lookup"><span data-stu-id="2f2c0-128">1004</span></span>|<span data-ttu-id="2f2c0-129">Обновление программного обеспечения доступно на устройстве</span><span class="sxs-lookup"><span data-stu-id="2f2c0-129">The software update is available on the device</span></span>|
|<span data-ttu-id="2f2c0-130">scheduled</span><span class="sxs-lookup"><span data-stu-id="2f2c0-130">scheduled</span></span>|<span data-ttu-id="2f2c0-131">1005</span><span class="sxs-lookup"><span data-stu-id="2f2c0-131">1005</span></span>|<span data-ttu-id="2f2c0-132">Обновление программного обеспечения запланировано на устройстве</span><span class="sxs-lookup"><span data-stu-id="2f2c0-132">The software update has been scheduled on the device</span></span>|
|<span data-ttu-id="2f2c0-133">довнлоадфаилед</span><span class="sxs-lookup"><span data-stu-id="2f2c0-133">downloadFailed</span></span>|<span data-ttu-id="2f2c0-134">2000</span><span class="sxs-lookup"><span data-stu-id="2f2c0-134">2000</span></span>|<span data-ttu-id="2f2c0-135">Не удалось скачать обновление программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="2f2c0-135">The software update download has failed</span></span>|
|<span data-ttu-id="2f2c0-136">довнлоадинсуффиЦиентспаце</span><span class="sxs-lookup"><span data-stu-id="2f2c0-136">downloadInsufficientSpace</span></span>|<span data-ttu-id="2f2c0-137">2001</span><span class="sxs-lookup"><span data-stu-id="2f2c0-137">2001</span></span>|<span data-ttu-id="2f2c0-138">Недостаточно места для скачивания обновления</span><span class="sxs-lookup"><span data-stu-id="2f2c0-138">There is not enough space to download the update</span></span>|
|<span data-ttu-id="2f2c0-139">довнлоадинсуффиЦиентповер</span><span class="sxs-lookup"><span data-stu-id="2f2c0-139">downloadInsufficientPower</span></span>|<span data-ttu-id="2f2c0-140">2002</span><span class="sxs-lookup"><span data-stu-id="2f2c0-140">2002</span></span>|<span data-ttu-id="2f2c0-141">Не хватает мощности для скачивания обновления</span><span class="sxs-lookup"><span data-stu-id="2f2c0-141">There is not enough power to download the update</span></span>|
|<span data-ttu-id="2f2c0-142">довнлоадинсуффиЦиентнетворк</span><span class="sxs-lookup"><span data-stu-id="2f2c0-142">downloadInsufficientNetwork</span></span>|<span data-ttu-id="2f2c0-143">2003</span><span class="sxs-lookup"><span data-stu-id="2f2c0-143">2003</span></span>|<span data-ttu-id="2f2c0-144">Недостаточно места в сети для скачивания обновления</span><span class="sxs-lookup"><span data-stu-id="2f2c0-144">There is insufficient network capacity to download the update</span></span>|
|<span data-ttu-id="2f2c0-145">инсталлинсуффиЦиентспаце</span><span class="sxs-lookup"><span data-stu-id="2f2c0-145">installInsufficientSpace</span></span>|<span data-ttu-id="2f2c0-146">2004</span><span class="sxs-lookup"><span data-stu-id="2f2c0-146">2004</span></span>|<span data-ttu-id="2f2c0-147">Недостаточно места для установки обновления</span><span class="sxs-lookup"><span data-stu-id="2f2c0-147">There is not enough space to install the update</span></span>|
|<span data-ttu-id="2f2c0-148">инсталлинсуффиЦиентповер</span><span class="sxs-lookup"><span data-stu-id="2f2c0-148">installInsufficientPower</span></span>|<span data-ttu-id="2f2c0-149">2005</span><span class="sxs-lookup"><span data-stu-id="2f2c0-149">2005</span></span>|<span data-ttu-id="2f2c0-150">Недостаточно электроэнергии для установки обновления.</span><span class="sxs-lookup"><span data-stu-id="2f2c0-150">There is not enough power to install the update</span></span>|
|<span data-ttu-id="2f2c0-151">инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="2f2c0-151">installFailed</span></span>|<span data-ttu-id="2f2c0-152">2006</span><span class="sxs-lookup"><span data-stu-id="2f2c0-152">2006</span></span>|<span data-ttu-id="2f2c0-153">Не удалось выполнить установку по неопределенной причине</span><span class="sxs-lookup"><span data-stu-id="2f2c0-153">Installation has failed for an unspecified reason</span></span>|
|<span data-ttu-id="2f2c0-154">коммандфаилед</span><span class="sxs-lookup"><span data-stu-id="2f2c0-154">commandFailed</span></span>|<span data-ttu-id="2f2c0-155">2007</span><span class="sxs-lookup"><span data-stu-id="2f2c0-155">2007</span></span>|<span data-ttu-id="2f2c0-156">Не удалось выполнить команду обновления расписания по неуказанной причине</span><span class="sxs-lookup"><span data-stu-id="2f2c0-156">The schedule update command has failed for an unspecified reason</span></span>|





