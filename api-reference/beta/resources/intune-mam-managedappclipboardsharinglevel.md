---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7daab906ab376aea8b7540b88c6922a37ec23bd2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684647"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="65446-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="65446-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="65446-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65446-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65446-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65446-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65446-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65446-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65446-107">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="65446-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="65446-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="65446-108">Members</span></span>
|<span data-ttu-id="65446-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="65446-109">Member</span></span>|<span data-ttu-id="65446-110">Значение</span><span class="sxs-lookup"><span data-stu-id="65446-110">Value</span></span>|<span data-ttu-id="65446-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65446-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65446-112">аллаппс</span><span class="sxs-lookup"><span data-stu-id="65446-112">allApps</span></span>|<span data-ttu-id="65446-113">нуль</span><span class="sxs-lookup"><span data-stu-id="65446-113">0</span></span>|<span data-ttu-id="65446-114">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="65446-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="65446-115">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="65446-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="65446-116">1,1</span><span class="sxs-lookup"><span data-stu-id="65446-116">1</span></span>|<span data-ttu-id="65446-117">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="65446-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="65446-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="65446-118">managedApps</span></span>|<span data-ttu-id="65446-119">2</span><span class="sxs-lookup"><span data-stu-id="65446-119">2</span></span>|<span data-ttu-id="65446-120">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="65446-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="65446-121">заблокированных</span><span class="sxs-lookup"><span data-stu-id="65446-121">blocked</span></span>|<span data-ttu-id="65446-122">4</span><span class="sxs-lookup"><span data-stu-id="65446-122">3</span></span>|<span data-ttu-id="65446-123">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="65446-123">Sharing between apps is disabled</span></span>|





