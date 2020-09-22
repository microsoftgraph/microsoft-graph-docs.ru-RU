---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a4f9044e90c67afe3ec50ba2349a94d194641dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036778"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="b4729-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="b4729-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="b4729-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4729-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4729-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4729-106">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="b4729-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="b4729-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4729-107">Members</span></span>
|<span data-ttu-id="b4729-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4729-108">Member</span></span>|<span data-ttu-id="b4729-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b4729-109">Value</span></span>|<span data-ttu-id="b4729-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4729-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4729-111">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="b4729-111">basedOnReturnCode</span></span>|<span data-ttu-id="b4729-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b4729-112">0</span></span>|<span data-ttu-id="b4729-113">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="b4729-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="b4729-114">разрешить</span><span class="sxs-lookup"><span data-stu-id="b4729-114">allow</span></span>|<span data-ttu-id="b4729-115">1 </span><span class="sxs-lookup"><span data-stu-id="b4729-115">1</span></span>|<span data-ttu-id="b4729-116">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="b4729-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="b4729-117">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="b4729-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b4729-118">подавлять</span><span class="sxs-lookup"><span data-stu-id="b4729-118">suppress</span></span>|<span data-ttu-id="b4729-119">2 </span><span class="sxs-lookup"><span data-stu-id="b4729-119">2</span></span>|<span data-ttu-id="b4729-120">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="b4729-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="b4729-121">включить</span><span class="sxs-lookup"><span data-stu-id="b4729-121">force</span></span>|<span data-ttu-id="b4729-122">4</span><span class="sxs-lookup"><span data-stu-id="b4729-122">3</span></span>|<span data-ttu-id="b4729-123">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="b4729-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|





