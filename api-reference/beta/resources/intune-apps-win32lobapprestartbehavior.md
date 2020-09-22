---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 61c41f8e2d9d0b787988a10e0562d10567bf1b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071054"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="ebd65-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="ebd65-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="ebd65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebd65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebd65-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebd65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebd65-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebd65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd65-107">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="ebd65-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="ebd65-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ebd65-108">Members</span></span>
|<span data-ttu-id="ebd65-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ebd65-109">Member</span></span>|<span data-ttu-id="ebd65-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ebd65-110">Value</span></span>|<span data-ttu-id="ebd65-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebd65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd65-112">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="ebd65-112">basedOnReturnCode</span></span>|<span data-ttu-id="ebd65-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ebd65-113">0</span></span>|<span data-ttu-id="ebd65-114">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="ebd65-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="ebd65-115">разрешить</span><span class="sxs-lookup"><span data-stu-id="ebd65-115">allow</span></span>|<span data-ttu-id="ebd65-116">1 </span><span class="sxs-lookup"><span data-stu-id="ebd65-116">1</span></span>|<span data-ttu-id="ebd65-117">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ebd65-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="ebd65-118">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="ebd65-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="ebd65-119">подавлять</span><span class="sxs-lookup"><span data-stu-id="ebd65-119">suppress</span></span>|<span data-ttu-id="ebd65-120">2 </span><span class="sxs-lookup"><span data-stu-id="ebd65-120">2</span></span>|<span data-ttu-id="ebd65-121">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="ebd65-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="ebd65-122">включить</span><span class="sxs-lookup"><span data-stu-id="ebd65-122">force</span></span>|<span data-ttu-id="ebd65-123">4</span><span class="sxs-lookup"><span data-stu-id="ebd65-123">3</span></span>|<span data-ttu-id="ebd65-124">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ebd65-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|






