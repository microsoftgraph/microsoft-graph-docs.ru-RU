---
title: Тип перечисления configurationManagerClientState
description: Состояние клиента диспетчер конфигурации
ms.openlocfilehash: c76fc33fee0fd5f6f5782f77d988535ec851cc86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080500"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="6fb1c-103">Тип перечисления configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="6fb1c-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="6fb1c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fb1c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fb1c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fb1c-107">Состояние клиента диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="6fb1c-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="6fb1c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6fb1c-108">Members</span></span>
|<span data-ttu-id="6fb1c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6fb1c-109">Member</span></span>|<span data-ttu-id="6fb1c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6fb1c-110">Value</span></span>|<span data-ttu-id="6fb1c-111">Description</span><span class="sxs-lookup"><span data-stu-id="6fb1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb1c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="6fb1c-112">unknown</span></span>|<span data-ttu-id="6fb1c-113">0</span><span class="sxs-lookup"><span data-stu-id="6fb1c-113">0</span></span>|<span data-ttu-id="6fb1c-114">Диспетчер конфигурации агента старше 1806 или не установлена или это устройство не возвращенных в Intune старше 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="6fb1c-115">установлен</span><span class="sxs-lookup"><span data-stu-id="6fb1c-115">installed</span></span>|<span data-ttu-id="6fb1c-116">1</span><span class="sxs-lookup"><span data-stu-id="6fb1c-116">1</span></span>|<span data-ttu-id="6fb1c-117">Агент диспетчера конфигурации установлен, но может быть отображаются в консоли диспетчера конфигурации еще.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="6fb1c-118">Подождите несколько часов для ее обновление.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="6fb1c-119">работоспособны</span><span class="sxs-lookup"><span data-stu-id="6fb1c-119">healthy</span></span>|<span data-ttu-id="6fb1c-120">7</span><span class="sxs-lookup"><span data-stu-id="6fb1c-120">7</span></span>|<span data-ttu-id="6fb1c-121">Это устройство удалось успешно проверить с помощью службы диспетчера конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="6fb1c-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="6fb1c-122">installFailed</span></span>|<span data-ttu-id="6fb1c-123">8</span><span class="sxs-lookup"><span data-stu-id="6fb1c-123">8</span></span>|<span data-ttu-id="6fb1c-124">Не удается установить агент диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="6fb1c-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="6fb1c-125">updateFailed</span></span>|<span data-ttu-id="6fb1c-126">11</span><span class="sxs-lookup"><span data-stu-id="6fb1c-126">11</span></span>|<span data-ttu-id="6fb1c-127">Не удалось обновить версии x в y версия агента диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="6fb1c-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="6fb1c-128">communicationError</span></span>|<span data-ttu-id="6fb1c-129">19</span><span class="sxs-lookup"><span data-stu-id="6fb1c-129">19</span></span>|<span data-ttu-id="6fb1c-130">Агент диспетчера конфигурации удалось для доступа к службе Диспетчер конфигурации в прошлом, но теперь больше не является возможность.</span><span class="sxs-lookup"><span data-stu-id="6fb1c-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





