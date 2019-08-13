---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba7de7ee3612c4d1e8e419522e8d18587339343c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370286"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="0e65e-103">тип перечисления Конфигуратионманажерклиентстате</span><span class="sxs-lookup"><span data-stu-id="0e65e-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="0e65e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e65e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e65e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e65e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e65e-106">Состояние клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="0e65e-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="0e65e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0e65e-107">Members</span></span>
|<span data-ttu-id="0e65e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0e65e-108">Member</span></span>|<span data-ttu-id="0e65e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0e65e-109">Value</span></span>|<span data-ttu-id="0e65e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e65e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e65e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="0e65e-111">unknown</span></span>|<span data-ttu-id="0e65e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0e65e-112">0</span></span>|<span data-ttu-id="0e65e-113">Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0e65e-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="0e65e-114">устанавлива</span><span class="sxs-lookup"><span data-stu-id="0e65e-114">installed</span></span>|<span data-ttu-id="0e65e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0e65e-115">1</span></span>|<span data-ttu-id="0e65e-116">Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="0e65e-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="0e65e-117">Подождите несколько часов, пока оно не будет обновлено.</span><span class="sxs-lookup"><span data-stu-id="0e65e-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="0e65e-118">рабочее</span><span class="sxs-lookup"><span data-stu-id="0e65e-118">healthy</span></span>|<span data-ttu-id="0e65e-119">7 </span><span class="sxs-lookup"><span data-stu-id="0e65e-119">7</span></span>|<span data-ttu-id="0e65e-120">Этому устройству удалось успешно вернуть службу Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="0e65e-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="0e65e-121">инсталлфаилед</span><span class="sxs-lookup"><span data-stu-id="0e65e-121">installFailed</span></span>|<span data-ttu-id="0e65e-122">8 </span><span class="sxs-lookup"><span data-stu-id="0e65e-122">8</span></span>|<span data-ttu-id="0e65e-123">Не удалось установить агент диспетчера конфигураций.</span><span class="sxs-lookup"><span data-stu-id="0e65e-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="0e65e-124">упдатефаилед</span><span class="sxs-lookup"><span data-stu-id="0e65e-124">updateFailed</span></span>|<span data-ttu-id="0e65e-125">-11:00</span><span class="sxs-lookup"><span data-stu-id="0e65e-125">11</span></span>|<span data-ttu-id="0e65e-126">Ошибка обновления от версии x до версии y агента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="0e65e-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="0e65e-127">коммуникатионеррор</span><span class="sxs-lookup"><span data-stu-id="0e65e-127">communicationError</span></span>|<span data-ttu-id="0e65e-128">19</span><span class="sxs-lookup"><span data-stu-id="0e65e-128">19</span></span>|<span data-ttu-id="0e65e-129">Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может.</span><span class="sxs-lookup"><span data-stu-id="0e65e-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |



