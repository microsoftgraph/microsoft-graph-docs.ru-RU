---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e99dde25fb1b57e06cddddc9610a6860a193059
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490317"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="a9a92-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="a9a92-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="a9a92-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9a92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9a92-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9a92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9a92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9a92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9a92-107">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="a9a92-107">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="a9a92-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a9a92-108">Members</span></span>
|<span data-ttu-id="a9a92-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a9a92-109">Member</span></span>|<span data-ttu-id="a9a92-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a9a92-110">Value</span></span>|<span data-ttu-id="a9a92-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a9a92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9a92-112">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="a9a92-112">basedOnReturnCode</span></span>|<span data-ttu-id="a9a92-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a9a92-113">0</span></span>|<span data-ttu-id="a9a92-114">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="a9a92-114">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="a9a92-115">разрешить</span><span class="sxs-lookup"><span data-stu-id="a9a92-115">allow</span></span>|<span data-ttu-id="a9a92-116">1 </span><span class="sxs-lookup"><span data-stu-id="a9a92-116">1</span></span>|<span data-ttu-id="a9a92-117">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="a9a92-117">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="a9a92-118">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="a9a92-118">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="a9a92-119">подавлять</span><span class="sxs-lookup"><span data-stu-id="a9a92-119">suppress</span></span>|<span data-ttu-id="a9a92-120">2 </span><span class="sxs-lookup"><span data-stu-id="a9a92-120">2</span></span>|<span data-ttu-id="a9a92-121">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="a9a92-121">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="a9a92-122">включить</span><span class="sxs-lookup"><span data-stu-id="a9a92-122">force</span></span>|<span data-ttu-id="a9a92-123">3 </span><span class="sxs-lookup"><span data-stu-id="a9a92-123">3</span></span>|<span data-ttu-id="a9a92-124">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="a9a92-124">Intune will force the device to restart immediately after the app installation operation.</span></span>|



