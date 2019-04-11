---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6231ecebf407172f2c7178a130d90200868292
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776523"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="a487d-103">тип перечисления Конфигуратионманажерклиентстате</span><span class="sxs-lookup"><span data-stu-id="a487d-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="a487d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a487d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a487d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a487d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a487d-106">Состояние клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="a487d-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="a487d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a487d-107">Members</span></span>
|<span data-ttu-id="a487d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a487d-108">Member</span></span>|<span data-ttu-id="a487d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a487d-109">Value</span></span>|<span data-ttu-id="a487d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a487d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a487d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a487d-111">unknown</span></span>|<span data-ttu-id="a487d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a487d-112">0</span></span>|<span data-ttu-id="a487d-113">Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.</span><span class="sxs-lookup"><span data-stu-id="a487d-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="a487d-114">устанавлива</span><span class="sxs-lookup"><span data-stu-id="a487d-114">installed</span></span>|<span data-ttu-id="a487d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a487d-115">1</span></span>|<span data-ttu-id="a487d-116">Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="a487d-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="a487d-117">Подождите несколько часов, пока оно не будет обновлено.</span><span class="sxs-lookup"><span data-stu-id="a487d-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="a487d-118">рабочее</span><span class="sxs-lookup"><span data-stu-id="a487d-118">healthy</span></span>|<span data-ttu-id="a487d-119">см</span><span class="sxs-lookup"><span data-stu-id="a487d-119">7</span></span>|<span data-ttu-id="a487d-120">Этому устройству удалось успешно вернуть службу Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="a487d-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="a487d-121">Инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="a487d-121">installFailed</span></span>|<span data-ttu-id="a487d-122">8,5</span><span class="sxs-lookup"><span data-stu-id="a487d-122">8</span></span>|<span data-ttu-id="a487d-123">Не удалось установить агент диспетчера конфигураций.</span><span class="sxs-lookup"><span data-stu-id="a487d-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="a487d-124">Упдатефаилед</span><span class="sxs-lookup"><span data-stu-id="a487d-124">updateFailed</span></span>|<span data-ttu-id="a487d-125">-11:00</span><span class="sxs-lookup"><span data-stu-id="a487d-125">11</span></span>|<span data-ttu-id="a487d-126">Ошибка обновления от версии x до версии y агента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="a487d-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="a487d-127">Коммуникатионеррор</span><span class="sxs-lookup"><span data-stu-id="a487d-127">communicationError</span></span>|<span data-ttu-id="a487d-128">19</span><span class="sxs-lookup"><span data-stu-id="a487d-128">19</span></span>|<span data-ttu-id="a487d-129">Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может.</span><span class="sxs-lookup"><span data-stu-id="a487d-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





