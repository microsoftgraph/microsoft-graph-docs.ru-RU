---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
ms.openlocfilehash: 7cf7b4a2f6ea6dc129a21167a2d75ba215ff29fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028427"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="ff838-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="ff838-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="ff838-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff838-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff838-105">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="ff838-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="ff838-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ff838-106">Members</span></span>
|<span data-ttu-id="ff838-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ff838-107">Member</span></span>|<span data-ttu-id="ff838-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ff838-108">Value</span></span>|<span data-ttu-id="ff838-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ff838-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff838-110">allApps</span><span class="sxs-lookup"><span data-stu-id="ff838-110">allApps</span></span>|<span data-ttu-id="ff838-111">0</span><span class="sxs-lookup"><span data-stu-id="ff838-111">0</span></span>|<span data-ttu-id="ff838-112">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="ff838-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="ff838-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="ff838-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="ff838-114">1</span><span class="sxs-lookup"><span data-stu-id="ff838-114">1</span></span>|<span data-ttu-id="ff838-115">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="ff838-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="ff838-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="ff838-116">managedApps</span></span>|<span data-ttu-id="ff838-117">2</span><span class="sxs-lookup"><span data-stu-id="ff838-117">2</span></span>|<span data-ttu-id="ff838-118">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="ff838-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="ff838-119">заблокировано</span><span class="sxs-lookup"><span data-stu-id="ff838-119">blocked</span></span>|<span data-ttu-id="ff838-120">3</span><span class="sxs-lookup"><span data-stu-id="ff838-120">3</span></span>|<span data-ttu-id="ff838-121">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="ff838-121">Sharing between apps is disabled</span></span>|



