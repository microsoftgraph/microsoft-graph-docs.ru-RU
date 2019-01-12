---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968419"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="98748-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="98748-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="98748-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98748-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98748-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98748-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98748-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98748-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98748-107">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="98748-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="98748-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="98748-108">Members</span></span>
|<span data-ttu-id="98748-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="98748-109">Member</span></span>|<span data-ttu-id="98748-110">Значение</span><span class="sxs-lookup"><span data-stu-id="98748-110">Value</span></span>|<span data-ttu-id="98748-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98748-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98748-112">allApps</span><span class="sxs-lookup"><span data-stu-id="98748-112">allApps</span></span>|<span data-ttu-id="98748-113">0</span><span class="sxs-lookup"><span data-stu-id="98748-113">0</span></span>|<span data-ttu-id="98748-114">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="98748-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="98748-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="98748-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="98748-116">1</span><span class="sxs-lookup"><span data-stu-id="98748-116">1</span></span>|<span data-ttu-id="98748-117">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="98748-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="98748-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="98748-118">managedApps</span></span>|<span data-ttu-id="98748-119">2</span><span class="sxs-lookup"><span data-stu-id="98748-119">2</span></span>|<span data-ttu-id="98748-120">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="98748-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="98748-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="98748-121">blocked</span></span>|<span data-ttu-id="98748-122">3</span><span class="sxs-lookup"><span data-stu-id="98748-122">3</span></span>|<span data-ttu-id="98748-123">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="98748-123">Sharing between apps is disabled</span></span>|





