---
title: тип enum win32LobAppRestartBehavior
description: Указывает тип действия перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc6ff030c2228ae108e034eea312c57d40b9006f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758969"
---
# <a name="win32lobapprestartbehavior-enum-type"></a><span data-ttu-id="1df1e-103">тип enum win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="1df1e-103">win32LobAppRestartBehavior enum type</span></span>

<span data-ttu-id="1df1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1df1e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1df1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1df1e-106">Указывает тип действия перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="1df1e-106">Indicates the type of restart action.</span></span>

## <a name="members"></a><span data-ttu-id="1df1e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1df1e-107">Members</span></span>
|<span data-ttu-id="1df1e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1df1e-108">Member</span></span>|<span data-ttu-id="1df1e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1df1e-109">Value</span></span>|<span data-ttu-id="1df1e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1df1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df1e-111">basedOnReturnCode</span><span class="sxs-lookup"><span data-stu-id="1df1e-111">basedOnReturnCode</span></span>|<span data-ttu-id="1df1e-112">0</span><span class="sxs-lookup"><span data-stu-id="1df1e-112">0</span></span>|<span data-ttu-id="1df1e-113">Intune перезапустит устройство после запуска установки приложения, если операция возвращает код перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="1df1e-113">Intune will restart the device after running the app installation if the operation returns a reboot code.</span></span>|
|<span data-ttu-id="1df1e-114">разрешить</span><span class="sxs-lookup"><span data-stu-id="1df1e-114">allow</span></span>|<span data-ttu-id="1df1e-115">1</span><span class="sxs-lookup"><span data-stu-id="1df1e-115">1</span></span>|<span data-ttu-id="1df1e-116">Intune не будет принимать каких-либо конкретных действий по перезагрузке кодов в результате установки приложений.</span><span class="sxs-lookup"><span data-stu-id="1df1e-116">Intune will not take any specific action on reboot codes resulting from app installations.</span></span> <span data-ttu-id="1df1e-117">Intune не будет пытаться подавить перезапуски для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="1df1e-117">Intune will not attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="1df1e-118">подавление</span><span class="sxs-lookup"><span data-stu-id="1df1e-118">suppress</span></span>|<span data-ttu-id="1df1e-119">2</span><span class="sxs-lookup"><span data-stu-id="1df1e-119">2</span></span>|<span data-ttu-id="1df1e-120">Intune будет пытаться подавить перезапуски для приложений MSI.</span><span class="sxs-lookup"><span data-stu-id="1df1e-120">Intune will attempt to suppress restarts for MSI apps.</span></span>|
|<span data-ttu-id="1df1e-121">force</span><span class="sxs-lookup"><span data-stu-id="1df1e-121">force</span></span>|<span data-ttu-id="1df1e-122">3</span><span class="sxs-lookup"><span data-stu-id="1df1e-122">3</span></span>|<span data-ttu-id="1df1e-123">Intune заставит устройство перезапуститься сразу после операции установки приложения.</span><span class="sxs-lookup"><span data-stu-id="1df1e-123">Intune will force the device to restart immediately after the app installation operation.</span></span>|




