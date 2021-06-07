---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 28a5d906342cc240d2382ed18c6de572e316f886
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754506"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="2afd9-103">тип enum managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2afd9-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="2afd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2afd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2afd9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2afd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2afd9-106">Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями</span><span class="sxs-lookup"><span data-stu-id="2afd9-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="2afd9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2afd9-107">Members</span></span>
|<span data-ttu-id="2afd9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2afd9-108">Member</span></span>|<span data-ttu-id="2afd9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2afd9-109">Value</span></span>|<span data-ttu-id="2afd9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2afd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2afd9-111">allApps</span><span class="sxs-lookup"><span data-stu-id="2afd9-111">allApps</span></span>|<span data-ttu-id="2afd9-112">0</span><span class="sxs-lookup"><span data-stu-id="2afd9-112">0</span></span>|<span data-ttu-id="2afd9-113">Разрешено совместное использование между всеми приложениями, управляемыми или не управляемыми</span><span class="sxs-lookup"><span data-stu-id="2afd9-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="2afd9-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="2afd9-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="2afd9-115">1</span><span class="sxs-lookup"><span data-stu-id="2afd9-115">1</span></span>|<span data-ttu-id="2afd9-116">Разрешен общий доступ между всеми управляемыми приложениями с включенной вклейки</span><span class="sxs-lookup"><span data-stu-id="2afd9-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="2afd9-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="2afd9-117">managedApps</span></span>|<span data-ttu-id="2afd9-118">2</span><span class="sxs-lookup"><span data-stu-id="2afd9-118">2</span></span>|<span data-ttu-id="2afd9-119">Разрешен общий доступ между всеми управляемыми приложениями</span><span class="sxs-lookup"><span data-stu-id="2afd9-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="2afd9-120">заблокировано</span><span class="sxs-lookup"><span data-stu-id="2afd9-120">blocked</span></span>|<span data-ttu-id="2afd9-121">3</span><span class="sxs-lookup"><span data-stu-id="2afd9-121">3</span></span>|<span data-ttu-id="2afd9-122">Совместное использование между приложениями отключено</span><span class="sxs-lookup"><span data-stu-id="2afd9-122">Sharing between apps is disabled</span></span>|




