---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
ms.openlocfilehash: 16d6e9154b3d6e683d9ddce0efd70a40c01c8994
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814317"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="4932a-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="4932a-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="4932a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4932a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4932a-105">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="4932a-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="4932a-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="4932a-106">Members</span></span>
|<span data-ttu-id="4932a-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="4932a-107">Member</span></span>|<span data-ttu-id="4932a-108">Значение</span><span class="sxs-lookup"><span data-stu-id="4932a-108">Value</span></span>|<span data-ttu-id="4932a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4932a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4932a-110">allApps</span><span class="sxs-lookup"><span data-stu-id="4932a-110">allApps</span></span>|<span data-ttu-id="4932a-111">0</span><span class="sxs-lookup"><span data-stu-id="4932a-111">0</span></span>|<span data-ttu-id="4932a-112">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="4932a-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="4932a-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="4932a-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="4932a-114">1</span><span class="sxs-lookup"><span data-stu-id="4932a-114">1</span></span>|<span data-ttu-id="4932a-115">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="4932a-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="4932a-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="4932a-116">managedApps</span></span>|<span data-ttu-id="4932a-117">2</span><span class="sxs-lookup"><span data-stu-id="4932a-117">2</span></span>|<span data-ttu-id="4932a-118">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="4932a-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="4932a-119">заблокировано</span><span class="sxs-lookup"><span data-stu-id="4932a-119">blocked</span></span>|<span data-ttu-id="4932a-120">3</span><span class="sxs-lookup"><span data-stu-id="4932a-120">3</span></span>|<span data-ttu-id="4932a-121">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="4932a-121">Sharing between apps is disabled</span></span>|



