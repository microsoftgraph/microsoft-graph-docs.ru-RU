---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
ms.openlocfilehash: 363e80b2242f5ac4d481389633aaa72fcc27894a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808178"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="0897d-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="0897d-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="0897d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0897d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0897d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0897d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0897d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0897d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0897d-107">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="0897d-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="0897d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0897d-108">Members</span></span>
|<span data-ttu-id="0897d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0897d-109">Member</span></span>|<span data-ttu-id="0897d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0897d-110">Value</span></span>|<span data-ttu-id="0897d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0897d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0897d-112">allApps</span><span class="sxs-lookup"><span data-stu-id="0897d-112">allApps</span></span>|<span data-ttu-id="0897d-113">0</span><span class="sxs-lookup"><span data-stu-id="0897d-113">0</span></span>|<span data-ttu-id="0897d-114">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="0897d-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="0897d-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="0897d-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="0897d-116">1</span><span class="sxs-lookup"><span data-stu-id="0897d-116">1</span></span>|<span data-ttu-id="0897d-117">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="0897d-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="0897d-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="0897d-118">managedApps</span></span>|<span data-ttu-id="0897d-119">2</span><span class="sxs-lookup"><span data-stu-id="0897d-119">2</span></span>|<span data-ttu-id="0897d-120">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="0897d-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="0897d-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="0897d-121">blocked</span></span>|<span data-ttu-id="0897d-122">3</span><span class="sxs-lookup"><span data-stu-id="0897d-122">3</span></span>|<span data-ttu-id="0897d-123">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="0897d-123">Sharing between apps is disabled</span></span>|





