---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c219f9a6235bff7c406294630faa1d1bc50ec7ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030460"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="7eee3-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="7eee3-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="7eee3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eee3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7eee3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eee3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7eee3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7eee3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eee3-107">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="7eee3-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="7eee3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7eee3-108">Members</span></span>
|<span data-ttu-id="7eee3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7eee3-109">Member</span></span>|<span data-ttu-id="7eee3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7eee3-110">Value</span></span>|<span data-ttu-id="7eee3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7eee3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eee3-112">аллаппс</span><span class="sxs-lookup"><span data-stu-id="7eee3-112">allApps</span></span>|<span data-ttu-id="7eee3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7eee3-113">0</span></span>|<span data-ttu-id="7eee3-114">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="7eee3-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="7eee3-115">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="7eee3-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="7eee3-116">1 </span><span class="sxs-lookup"><span data-stu-id="7eee3-116">1</span></span>|<span data-ttu-id="7eee3-117">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="7eee3-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="7eee3-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="7eee3-118">managedApps</span></span>|<span data-ttu-id="7eee3-119">2 </span><span class="sxs-lookup"><span data-stu-id="7eee3-119">2</span></span>|<span data-ttu-id="7eee3-120">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="7eee3-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="7eee3-121">заблокированных</span><span class="sxs-lookup"><span data-stu-id="7eee3-121">blocked</span></span>|<span data-ttu-id="7eee3-122">4</span><span class="sxs-lookup"><span data-stu-id="7eee3-122">3</span></span>|<span data-ttu-id="7eee3-123">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="7eee3-123">Sharing between apps is disabled</span></span>|






