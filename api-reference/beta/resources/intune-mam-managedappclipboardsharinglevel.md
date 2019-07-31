---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 339dc8a824073f609ee580042895bd3a59f58e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998438"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="db6e0-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="db6e0-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="db6e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db6e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db6e0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db6e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db6e0-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="db6e0-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="db6e0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="db6e0-107">Members</span></span>
|<span data-ttu-id="db6e0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="db6e0-108">Member</span></span>|<span data-ttu-id="db6e0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="db6e0-109">Value</span></span>|<span data-ttu-id="db6e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db6e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db6e0-111">Аллаппс</span><span class="sxs-lookup"><span data-stu-id="db6e0-111">allApps</span></span>|<span data-ttu-id="db6e0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="db6e0-112">0</span></span>|<span data-ttu-id="db6e0-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="db6e0-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="db6e0-114">Манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="db6e0-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="db6e0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="db6e0-115">1</span></span>|<span data-ttu-id="db6e0-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="db6e0-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="db6e0-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="db6e0-117">managedApps</span></span>|<span data-ttu-id="db6e0-118">2</span><span class="sxs-lookup"><span data-stu-id="db6e0-118">2</span></span>|<span data-ttu-id="db6e0-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="db6e0-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="db6e0-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="db6e0-120">blocked</span></span>|<span data-ttu-id="db6e0-121">4</span><span class="sxs-lookup"><span data-stu-id="db6e0-121">3</span></span>|<span data-ttu-id="db6e0-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="db6e0-122">Sharing between apps is disabled</span></span>|





