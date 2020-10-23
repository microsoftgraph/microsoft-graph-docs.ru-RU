---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: de8f2af7c6d35b28154f00a4eac3bb20a4bdf64d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690233"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="4330a-103">тип перечисления Конфигуратионманажерклиентстате</span><span class="sxs-lookup"><span data-stu-id="4330a-103">configurationManagerClientState enum type</span></span>

<span data-ttu-id="4330a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4330a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4330a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4330a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4330a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4330a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4330a-107">Состояние клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="4330a-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="4330a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4330a-108">Members</span></span>
|<span data-ttu-id="4330a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4330a-109">Member</span></span>|<span data-ttu-id="4330a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4330a-110">Value</span></span>|<span data-ttu-id="4330a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4330a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4330a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="4330a-112">unknown</span></span>|<span data-ttu-id="4330a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4330a-113">0</span></span>|<span data-ttu-id="4330a-114">Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.</span><span class="sxs-lookup"><span data-stu-id="4330a-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="4330a-115">устанавлива</span><span class="sxs-lookup"><span data-stu-id="4330a-115">installed</span></span>|<span data-ttu-id="4330a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="4330a-116">1</span></span>|<span data-ttu-id="4330a-117">Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="4330a-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="4330a-118">Подождите несколько часов, пока оно не будет обновлено.</span><span class="sxs-lookup"><span data-stu-id="4330a-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="4330a-119">рабочее</span><span class="sxs-lookup"><span data-stu-id="4330a-119">healthy</span></span>|<span data-ttu-id="4330a-120">7 </span><span class="sxs-lookup"><span data-stu-id="4330a-120">7</span></span>|<span data-ttu-id="4330a-121">Этому устройству удалось успешно вернуть службу Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="4330a-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="4330a-122">инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="4330a-122">installFailed</span></span>|<span data-ttu-id="4330a-123">8 </span><span class="sxs-lookup"><span data-stu-id="4330a-123">8</span></span>|<span data-ttu-id="4330a-124">Не удалось установить агент диспетчера конфигураций.</span><span class="sxs-lookup"><span data-stu-id="4330a-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="4330a-125">упдатефаилед</span><span class="sxs-lookup"><span data-stu-id="4330a-125">updateFailed</span></span>|<span data-ttu-id="4330a-126">-11:00</span><span class="sxs-lookup"><span data-stu-id="4330a-126">11</span></span>|<span data-ttu-id="4330a-127">Ошибка обновления от версии x до версии y агента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="4330a-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="4330a-128">коммуникатионеррор</span><span class="sxs-lookup"><span data-stu-id="4330a-128">communicationError</span></span>|<span data-ttu-id="4330a-129">19</span><span class="sxs-lookup"><span data-stu-id="4330a-129">19</span></span>|<span data-ttu-id="4330a-130">Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может.</span><span class="sxs-lookup"><span data-stu-id="4330a-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





