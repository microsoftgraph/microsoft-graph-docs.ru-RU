---
title: Тип перечисления configurationManagerClientState
description: Состояние клиента диспетчер конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425787"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="81b3e-103">Тип перечисления configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="81b3e-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="81b3e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81b3e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81b3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81b3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81b3e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81b3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b3e-107">Состояние клиента диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="81b3e-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="81b3e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="81b3e-108">Members</span></span>
|<span data-ttu-id="81b3e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="81b3e-109">Member</span></span>|<span data-ttu-id="81b3e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="81b3e-110">Value</span></span>|<span data-ttu-id="81b3e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81b3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b3e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="81b3e-112">unknown</span></span>|<span data-ttu-id="81b3e-113">0</span><span class="sxs-lookup"><span data-stu-id="81b3e-113">0</span></span>|<span data-ttu-id="81b3e-114">Диспетчер конфигурации агента старше 1806 или не установлена или это устройство не возвращенных в Intune старше 30 дней.</span><span class="sxs-lookup"><span data-stu-id="81b3e-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="81b3e-115">установлен</span><span class="sxs-lookup"><span data-stu-id="81b3e-115">installed</span></span>|<span data-ttu-id="81b3e-116">1</span><span class="sxs-lookup"><span data-stu-id="81b3e-116">1</span></span>|<span data-ttu-id="81b3e-117">Агент диспетчера конфигурации установлен, но может быть отображаются в консоли диспетчера конфигурации еще.</span><span class="sxs-lookup"><span data-stu-id="81b3e-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="81b3e-118">Подождите несколько часов для ее обновление.</span><span class="sxs-lookup"><span data-stu-id="81b3e-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="81b3e-119">работоспособны</span><span class="sxs-lookup"><span data-stu-id="81b3e-119">healthy</span></span>|<span data-ttu-id="81b3e-120">7</span><span class="sxs-lookup"><span data-stu-id="81b3e-120">7</span></span>|<span data-ttu-id="81b3e-121">Это устройство удалось успешно проверить с помощью службы диспетчера конфигурации.</span><span class="sxs-lookup"><span data-stu-id="81b3e-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="81b3e-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="81b3e-122">installFailed</span></span>|<span data-ttu-id="81b3e-123">8</span><span class="sxs-lookup"><span data-stu-id="81b3e-123">8</span></span>|<span data-ttu-id="81b3e-124">Не удается установить агент диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="81b3e-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="81b3e-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="81b3e-125">updateFailed</span></span>|<span data-ttu-id="81b3e-126">11</span><span class="sxs-lookup"><span data-stu-id="81b3e-126">11</span></span>|<span data-ttu-id="81b3e-127">Не удалось обновить версии x в y версия агента диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="81b3e-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="81b3e-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="81b3e-128">communicationError</span></span>|<span data-ttu-id="81b3e-129">19</span><span class="sxs-lookup"><span data-stu-id="81b3e-129">19</span></span>|<span data-ttu-id="81b3e-130">Агент диспетчера конфигурации удалось для доступа к службе Диспетчер конфигурации в прошлом, но теперь больше не является возможность.</span><span class="sxs-lookup"><span data-stu-id="81b3e-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




