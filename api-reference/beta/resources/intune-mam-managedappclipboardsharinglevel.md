---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
ms.openlocfilehash: 71c4ab2d629fdfee3ded68612d7060a0fa069809
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082278"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="499f8-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="499f8-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="499f8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="499f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="499f8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="499f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="499f8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="499f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="499f8-107">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="499f8-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="499f8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="499f8-108">Members</span></span>
|<span data-ttu-id="499f8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="499f8-109">Member</span></span>|<span data-ttu-id="499f8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="499f8-110">Value</span></span>|<span data-ttu-id="499f8-111">Description</span><span class="sxs-lookup"><span data-stu-id="499f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499f8-112">allApps</span><span class="sxs-lookup"><span data-stu-id="499f8-112">allApps</span></span>|<span data-ttu-id="499f8-113">0</span><span class="sxs-lookup"><span data-stu-id="499f8-113">0</span></span>|<span data-ttu-id="499f8-114">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="499f8-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="499f8-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="499f8-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="499f8-116">1</span><span class="sxs-lookup"><span data-stu-id="499f8-116">1</span></span>|<span data-ttu-id="499f8-117">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="499f8-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="499f8-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="499f8-118">managedApps</span></span>|<span data-ttu-id="499f8-119">2</span><span class="sxs-lookup"><span data-stu-id="499f8-119">2</span></span>|<span data-ttu-id="499f8-120">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="499f8-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="499f8-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="499f8-121">blocked</span></span>|<span data-ttu-id="499f8-122">3</span><span class="sxs-lookup"><span data-stu-id="499f8-122">3</span></span>|<span data-ttu-id="499f8-123">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="499f8-123">Sharing between apps is disabled</span></span>|





