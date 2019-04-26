---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d18d09f2ba37b8b062f3d19ae5cf971d886f278
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563836"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="6c05f-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="6c05f-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="6c05f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c05f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c05f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c05f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c05f-106">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="6c05f-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="6c05f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6c05f-107">Members</span></span>
|<span data-ttu-id="6c05f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6c05f-108">Member</span></span>|<span data-ttu-id="6c05f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6c05f-109">Value</span></span>|<span data-ttu-id="6c05f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c05f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c05f-111">Аллаппс</span><span class="sxs-lookup"><span data-stu-id="6c05f-111">allApps</span></span>|<span data-ttu-id="6c05f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6c05f-112">0</span></span>|<span data-ttu-id="6c05f-113">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="6c05f-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="6c05f-114">Манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="6c05f-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="6c05f-115">1 </span><span class="sxs-lookup"><span data-stu-id="6c05f-115">1</span></span>|<span data-ttu-id="6c05f-116">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="6c05f-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="6c05f-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="6c05f-117">managedApps</span></span>|<span data-ttu-id="6c05f-118">2 </span><span class="sxs-lookup"><span data-stu-id="6c05f-118">2</span></span>|<span data-ttu-id="6c05f-119">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="6c05f-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="6c05f-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="6c05f-120">blocked</span></span>|<span data-ttu-id="6c05f-121">3 </span><span class="sxs-lookup"><span data-stu-id="6c05f-121">3</span></span>|<span data-ttu-id="6c05f-122">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="6c05f-122">Sharing between apps is disabled</span></span>|





