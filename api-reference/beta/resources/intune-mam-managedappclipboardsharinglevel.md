---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 29c5fee1a6873e331a9adc927f1a92cf60a8c9e8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267077"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="8dbbe-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="8dbbe-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="8dbbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dbbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dbbe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dbbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dbbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dbbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dbbe-107">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="8dbbe-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="8dbbe-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8dbbe-108">Members</span></span>
|<span data-ttu-id="8dbbe-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8dbbe-109">Member</span></span>|<span data-ttu-id="8dbbe-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8dbbe-110">Value</span></span>|<span data-ttu-id="8dbbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8dbbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dbbe-112">аллаппс</span><span class="sxs-lookup"><span data-stu-id="8dbbe-112">allApps</span></span>|<span data-ttu-id="8dbbe-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8dbbe-113">0</span></span>|<span data-ttu-id="8dbbe-114">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="8dbbe-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="8dbbe-115">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="8dbbe-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="8dbbe-116">1,1</span><span class="sxs-lookup"><span data-stu-id="8dbbe-116">1</span></span>|<span data-ttu-id="8dbbe-117">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="8dbbe-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="8dbbe-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="8dbbe-118">managedApps</span></span>|<span data-ttu-id="8dbbe-119">2</span><span class="sxs-lookup"><span data-stu-id="8dbbe-119">2</span></span>|<span data-ttu-id="8dbbe-120">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="8dbbe-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="8dbbe-121">заблокированных</span><span class="sxs-lookup"><span data-stu-id="8dbbe-121">blocked</span></span>|<span data-ttu-id="8dbbe-122">4</span><span class="sxs-lookup"><span data-stu-id="8dbbe-122">3</span></span>|<span data-ttu-id="8dbbe-123">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="8dbbe-123">Sharing between apps is disabled</span></span>|




