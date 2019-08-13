---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1e479f925e8b52ae746180851ce52ad116774367
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332213"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="b1c8a-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="b1c8a-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="b1c8a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c8a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1c8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c8a-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="b1c8a-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="b1c8a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b1c8a-107">Members</span></span>
|<span data-ttu-id="b1c8a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b1c8a-108">Member</span></span>|<span data-ttu-id="b1c8a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b1c8a-109">Value</span></span>|<span data-ttu-id="b1c8a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1c8a-111">аллаппс</span><span class="sxs-lookup"><span data-stu-id="b1c8a-111">allApps</span></span>|<span data-ttu-id="b1c8a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b1c8a-112">0</span></span>|<span data-ttu-id="b1c8a-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="b1c8a-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="b1c8a-114">манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="b1c8a-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="b1c8a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b1c8a-115">1</span></span>|<span data-ttu-id="b1c8a-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="b1c8a-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="b1c8a-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="b1c8a-117">managedApps</span></span>|<span data-ttu-id="b1c8a-118">2</span><span class="sxs-lookup"><span data-stu-id="b1c8a-118">2</span></span>|<span data-ttu-id="b1c8a-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="b1c8a-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="b1c8a-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="b1c8a-120">blocked</span></span>|<span data-ttu-id="b1c8a-121">4</span><span class="sxs-lookup"><span data-stu-id="b1c8a-121">3</span></span>|<span data-ttu-id="b1c8a-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="b1c8a-122">Sharing between apps is disabled</span></span>|



