---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 16fda1d530614ea138ecc575930b4800b5f143c4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797558"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="e2794-103">тип перечисления win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="e2794-103">win32LobAppRestartBehavior enum type</span></span>

> <span data-ttu-id="e2794-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2794-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2794-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2794-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2794-106">Указывает тип действия перезапуска.</span><span class="sxs-lookup"><span data-stu-id="e2794-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="e2794-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e2794-107">Members</span></span>
|<span data-ttu-id="e2794-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e2794-108">Member</span></span>|<span data-ttu-id="e2794-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e2794-109">Value</span></span>|<span data-ttu-id="e2794-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e2794-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2794-111">баседонретурнкоде</span><span class="sxs-lookup"><span data-stu-id="e2794-111">basedOnReturnCode</span></span>|<span data-ttu-id="e2794-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e2794-112">0</span></span>|<span data-ttu-id="e2794-113">Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="e2794-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="e2794-114">разрешить</span><span class="sxs-lookup"><span data-stu-id="e2794-114">allow</span></span>|<span data-ttu-id="e2794-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e2794-115">1</span></span>|<span data-ttu-id="e2794-116">Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e2794-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="e2794-117">Intune не будет пытаться отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="e2794-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="e2794-118">подавлять</span><span class="sxs-lookup"><span data-stu-id="e2794-118">suppress</span></span>|<span data-ttu-id="e2794-119">2</span><span class="sxs-lookup"><span data-stu-id="e2794-119">2</span></span>|<span data-ttu-id="e2794-120">Intune попытается отключить перезапуск для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="e2794-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="e2794-121">включить</span><span class="sxs-lookup"><span data-stu-id="e2794-121">force</span></span>|<span data-ttu-id="e2794-122">4</span><span class="sxs-lookup"><span data-stu-id="e2794-122">3</span></span>|<span data-ttu-id="e2794-123">Intune вынуждает устройство перезапускать сразу после завершения установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e2794-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|



