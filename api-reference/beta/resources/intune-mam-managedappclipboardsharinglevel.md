---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5f6153eeb4b76af9d8974b715b7c6342c646ba6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782246"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="ec0bf-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="ec0bf-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="ec0bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec0bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec0bf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec0bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec0bf-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="ec0bf-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="ec0bf-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ec0bf-107">Members</span></span>
|<span data-ttu-id="ec0bf-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ec0bf-108">Member</span></span>|<span data-ttu-id="ec0bf-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ec0bf-109">Value</span></span>|<span data-ttu-id="ec0bf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ec0bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec0bf-111">аллаппс</span><span class="sxs-lookup"><span data-stu-id="ec0bf-111">allApps</span></span>|<span data-ttu-id="ec0bf-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ec0bf-112">0</span></span>|<span data-ttu-id="ec0bf-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="ec0bf-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="ec0bf-114">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="ec0bf-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="ec0bf-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ec0bf-115">1</span></span>|<span data-ttu-id="ec0bf-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="ec0bf-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="ec0bf-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="ec0bf-117">managedApps</span></span>|<span data-ttu-id="ec0bf-118">2</span><span class="sxs-lookup"><span data-stu-id="ec0bf-118">2</span></span>|<span data-ttu-id="ec0bf-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ec0bf-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="ec0bf-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="ec0bf-120">blocked</span></span>|<span data-ttu-id="ec0bf-121">4</span><span class="sxs-lookup"><span data-stu-id="ec0bf-121">3</span></span>|<span data-ttu-id="ec0bf-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="ec0bf-122">Sharing between apps is disabled</span></span>|



