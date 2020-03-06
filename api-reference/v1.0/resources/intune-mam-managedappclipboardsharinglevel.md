---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0457069a3da40b138abbff091fffd6ffca653937
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532155"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="5284c-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="5284c-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="5284c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5284c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5284c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5284c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5284c-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="5284c-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="5284c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5284c-107">Members</span></span>
|<span data-ttu-id="5284c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5284c-108">Member</span></span>|<span data-ttu-id="5284c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5284c-109">Value</span></span>|<span data-ttu-id="5284c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5284c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5284c-111">аллаппс</span><span class="sxs-lookup"><span data-stu-id="5284c-111">allApps</span></span>|<span data-ttu-id="5284c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5284c-112">0</span></span>|<span data-ttu-id="5284c-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="5284c-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="5284c-114">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="5284c-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="5284c-115">1 </span><span class="sxs-lookup"><span data-stu-id="5284c-115">1</span></span>|<span data-ttu-id="5284c-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="5284c-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="5284c-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="5284c-117">managedApps</span></span>|<span data-ttu-id="5284c-118">2 </span><span class="sxs-lookup"><span data-stu-id="5284c-118">2</span></span>|<span data-ttu-id="5284c-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="5284c-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="5284c-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="5284c-120">blocked</span></span>|<span data-ttu-id="5284c-121">3 </span><span class="sxs-lookup"><span data-stu-id="5284c-121">3</span></span>|<span data-ttu-id="5284c-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="5284c-122">Sharing between apps is disabled</span></span>|




