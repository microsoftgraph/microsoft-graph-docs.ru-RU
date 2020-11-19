---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6cda29552c3ae0253ac1200d7a15ec394005ede5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293194"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="3d482-103">тип перечисления Конфигуратионманажерклиентстате</span><span class="sxs-lookup"><span data-stu-id="3d482-103">configurationManagerClientState enum type</span></span>

<span data-ttu-id="3d482-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d482-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d482-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d482-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d482-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d482-107">Состояние клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="3d482-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="3d482-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3d482-108">Members</span></span>
|<span data-ttu-id="3d482-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3d482-109">Member</span></span>|<span data-ttu-id="3d482-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3d482-110">Value</span></span>|<span data-ttu-id="3d482-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d482-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d482-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3d482-112">unknown</span></span>|<span data-ttu-id="3d482-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3d482-113">0</span></span>|<span data-ttu-id="3d482-114">Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.</span><span class="sxs-lookup"><span data-stu-id="3d482-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="3d482-115">устанавлива</span><span class="sxs-lookup"><span data-stu-id="3d482-115">installed</span></span>|<span data-ttu-id="3d482-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3d482-116">1</span></span>|<span data-ttu-id="3d482-117">Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="3d482-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="3d482-118">Подождите несколько часов, пока оно не будет обновлено.</span><span class="sxs-lookup"><span data-stu-id="3d482-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="3d482-119">рабочее</span><span class="sxs-lookup"><span data-stu-id="3d482-119">healthy</span></span>|<span data-ttu-id="3d482-120">7 </span><span class="sxs-lookup"><span data-stu-id="3d482-120">7</span></span>|<span data-ttu-id="3d482-121">Этому устройству удалось успешно вернуть службу Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="3d482-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="3d482-122">инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="3d482-122">installFailed</span></span>|<span data-ttu-id="3d482-123">8 </span><span class="sxs-lookup"><span data-stu-id="3d482-123">8</span></span>|<span data-ttu-id="3d482-124">Не удалось установить агент диспетчера конфигураций.</span><span class="sxs-lookup"><span data-stu-id="3d482-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="3d482-125">упдатефаилед</span><span class="sxs-lookup"><span data-stu-id="3d482-125">updateFailed</span></span>|<span data-ttu-id="3d482-126">11 </span><span class="sxs-lookup"><span data-stu-id="3d482-126">11</span></span>|<span data-ttu-id="3d482-127">Ошибка обновления от версии x до версии y агента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="3d482-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="3d482-128">коммуникатионеррор</span><span class="sxs-lookup"><span data-stu-id="3d482-128">communicationError</span></span>|<span data-ttu-id="3d482-129">19</span><span class="sxs-lookup"><span data-stu-id="3d482-129">19</span></span>|<span data-ttu-id="3d482-130">Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может.</span><span class="sxs-lookup"><span data-stu-id="3d482-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




