---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2902f3808ea1ebcc1442b0675c89da51b059f2c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422641"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="e2d6a-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="e2d6a-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="e2d6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2d6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2d6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2d6a-107">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="e2d6a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e2d6a-108">Members</span></span>
|<span data-ttu-id="e2d6a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e2d6a-109">Member</span></span>|<span data-ttu-id="e2d6a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e2d6a-110">Value</span></span>|<span data-ttu-id="e2d6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2d6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d6a-112">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="e2d6a-112">basedOnReturnCode</span></span>|<span data-ttu-id="e2d6a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e2d6a-113">0</span></span>|<span data-ttu-id="e2d6a-114">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="e2d6a-115">разрешить</span><span class="sxs-lookup"><span data-stu-id="e2d6a-115">allow</span></span>|<span data-ttu-id="e2d6a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e2d6a-116">1</span></span>|<span data-ttu-id="e2d6a-117">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="e2d6a-118">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="e2d6a-119">подавлять</span><span class="sxs-lookup"><span data-stu-id="e2d6a-119">suppress</span></span>|<span data-ttu-id="e2d6a-120">2</span><span class="sxs-lookup"><span data-stu-id="e2d6a-120">2</span></span>|<span data-ttu-id="e2d6a-121">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="e2d6a-122">включить</span><span class="sxs-lookup"><span data-stu-id="e2d6a-122">force</span></span>|<span data-ttu-id="e2d6a-123">4</span><span class="sxs-lookup"><span data-stu-id="e2d6a-123">3</span></span>|<span data-ttu-id="e2d6a-124">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e2d6a-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|



