---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4ce16d0c064fb182352fa0a0061fb2296fd44d7a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706186"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="c00bb-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="c00bb-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="c00bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c00bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c00bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c00bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c00bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c00bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c00bb-107">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="c00bb-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="c00bb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c00bb-108">Members</span></span>
|<span data-ttu-id="c00bb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c00bb-109">Member</span></span>|<span data-ttu-id="c00bb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c00bb-110">Value</span></span>|<span data-ttu-id="c00bb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c00bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c00bb-112">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="c00bb-112">basedOnReturnCode</span></span>|<span data-ttu-id="c00bb-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c00bb-113">0</span></span>|<span data-ttu-id="c00bb-114">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="c00bb-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="c00bb-115">разрешить</span><span class="sxs-lookup"><span data-stu-id="c00bb-115">allow</span></span>|<span data-ttu-id="c00bb-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c00bb-116">1</span></span>|<span data-ttu-id="c00bb-117">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c00bb-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="c00bb-118">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="c00bb-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="c00bb-119">подавлять</span><span class="sxs-lookup"><span data-stu-id="c00bb-119">suppress</span></span>|<span data-ttu-id="c00bb-120">2</span><span class="sxs-lookup"><span data-stu-id="c00bb-120">2</span></span>|<span data-ttu-id="c00bb-121">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="c00bb-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="c00bb-122">включить</span><span class="sxs-lookup"><span data-stu-id="c00bb-122">force</span></span>|<span data-ttu-id="c00bb-123">4</span><span class="sxs-lookup"><span data-stu-id="c00bb-123">3</span></span>|<span data-ttu-id="c00bb-124">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c00bb-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|





