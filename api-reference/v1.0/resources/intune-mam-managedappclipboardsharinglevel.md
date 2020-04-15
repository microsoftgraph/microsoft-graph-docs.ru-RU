---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55a9608144e31d9e11f1a435e9220934ee3cb792
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445824"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="3f4f2-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="3f4f2-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="3f4f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f4f2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f4f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4f2-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="3f4f2-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="3f4f2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3f4f2-107">Members</span></span>
|<span data-ttu-id="3f4f2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3f4f2-108">Member</span></span>|<span data-ttu-id="3f4f2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3f4f2-109">Value</span></span>|<span data-ttu-id="3f4f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4f2-111">аллаппс</span><span class="sxs-lookup"><span data-stu-id="3f4f2-111">allApps</span></span>|<span data-ttu-id="3f4f2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3f4f2-112">0</span></span>|<span data-ttu-id="3f4f2-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="3f4f2-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="3f4f2-114">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="3f4f2-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="3f4f2-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3f4f2-115">1</span></span>|<span data-ttu-id="3f4f2-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="3f4f2-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="3f4f2-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="3f4f2-117">managedApps</span></span>|<span data-ttu-id="3f4f2-118">2</span><span class="sxs-lookup"><span data-stu-id="3f4f2-118">2</span></span>|<span data-ttu-id="3f4f2-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="3f4f2-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="3f4f2-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="3f4f2-120">blocked</span></span>|<span data-ttu-id="3f4f2-121">4</span><span class="sxs-lookup"><span data-stu-id="3f4f2-121">3</span></span>|<span data-ttu-id="3f4f2-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="3f4f2-122">Sharing between apps is disabled</span></span>|







