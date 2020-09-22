---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8372d7a959a54a91d13aec91d2b27829fcf3a30c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074974"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="41d62-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="41d62-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="41d62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41d62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41d62-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41d62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d62-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="41d62-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="41d62-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="41d62-107">Members</span></span>
|<span data-ttu-id="41d62-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="41d62-108">Member</span></span>|<span data-ttu-id="41d62-109">Значение</span><span class="sxs-lookup"><span data-stu-id="41d62-109">Value</span></span>|<span data-ttu-id="41d62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41d62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d62-111">аллаппс</span><span class="sxs-lookup"><span data-stu-id="41d62-111">allApps</span></span>|<span data-ttu-id="41d62-112">нуль</span><span class="sxs-lookup"><span data-stu-id="41d62-112">0</span></span>|<span data-ttu-id="41d62-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="41d62-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="41d62-114">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="41d62-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="41d62-115">1 </span><span class="sxs-lookup"><span data-stu-id="41d62-115">1</span></span>|<span data-ttu-id="41d62-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="41d62-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="41d62-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="41d62-117">managedApps</span></span>|<span data-ttu-id="41d62-118">2 </span><span class="sxs-lookup"><span data-stu-id="41d62-118">2</span></span>|<span data-ttu-id="41d62-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="41d62-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="41d62-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="41d62-120">blocked</span></span>|<span data-ttu-id="41d62-121">4</span><span class="sxs-lookup"><span data-stu-id="41d62-121">3</span></span>|<span data-ttu-id="41d62-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="41d62-122">Sharing between apps is disabled</span></span>|









