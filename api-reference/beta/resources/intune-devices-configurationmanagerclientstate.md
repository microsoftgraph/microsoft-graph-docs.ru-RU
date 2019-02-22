---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8474e6886c1312fde4ce3afde3c3fe0185574c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170702"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="e8ee1-103">тип перечисления Конфигуратионманажерклиентстате</span><span class="sxs-lookup"><span data-stu-id="e8ee1-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="e8ee1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8ee1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ee1-106">Состояние клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="e8ee1-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="e8ee1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e8ee1-107">Members</span></span>
|<span data-ttu-id="e8ee1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e8ee1-108">Member</span></span>|<span data-ttu-id="e8ee1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e8ee1-109">Value</span></span>|<span data-ttu-id="e8ee1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ee1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ee1-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e8ee1-111">unknown</span></span>|<span data-ttu-id="e8ee1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e8ee1-112">0</span></span>|<span data-ttu-id="e8ee1-113">Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="e8ee1-114">устанавлива</span><span class="sxs-lookup"><span data-stu-id="e8ee1-114">installed</span></span>|<span data-ttu-id="e8ee1-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e8ee1-115">1</span></span>|<span data-ttu-id="e8ee1-116">Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="e8ee1-117">Подождите несколько часов, пока оно не будет обновлено.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="e8ee1-118">рабочее</span><span class="sxs-lookup"><span data-stu-id="e8ee1-118">healthy</span></span>|<span data-ttu-id="e8ee1-119">7</span><span class="sxs-lookup"><span data-stu-id="e8ee1-119">7</span></span>|<span data-ttu-id="e8ee1-120">Этому устройству удалось успешно вернуть службу Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="e8ee1-121">Инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="e8ee1-121">installFailed</span></span>|<span data-ttu-id="e8ee1-122">8,5</span><span class="sxs-lookup"><span data-stu-id="e8ee1-122">8</span></span>|<span data-ttu-id="e8ee1-123">Не удалось установить агент диспетчера конфигураций.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="e8ee1-124">Упдатефаилед</span><span class="sxs-lookup"><span data-stu-id="e8ee1-124">updateFailed</span></span>|<span data-ttu-id="e8ee1-125">-11:00</span><span class="sxs-lookup"><span data-stu-id="e8ee1-125">11</span></span>|<span data-ttu-id="e8ee1-126">Ошибка обновления от версии x до версии y агента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="e8ee1-127">Коммуникатионеррор</span><span class="sxs-lookup"><span data-stu-id="e8ee1-127">communicationError</span></span>|<span data-ttu-id="e8ee1-128">19</span><span class="sxs-lookup"><span data-stu-id="e8ee1-128">19</span></span>|<span data-ttu-id="e8ee1-129">Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может.</span><span class="sxs-lookup"><span data-stu-id="e8ee1-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




