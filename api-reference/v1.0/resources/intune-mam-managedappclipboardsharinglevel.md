---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 349f0ee08b8e3bff4e627c58318e2c21fa00847c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946786"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="8c78c-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="8c78c-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="8c78c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c78c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c78c-105">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="8c78c-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="8c78c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="8c78c-106">Members</span></span>
|<span data-ttu-id="8c78c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="8c78c-107">Member</span></span>|<span data-ttu-id="8c78c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="8c78c-108">Value</span></span>|<span data-ttu-id="8c78c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8c78c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c78c-110">allApps</span><span class="sxs-lookup"><span data-stu-id="8c78c-110">allApps</span></span>|<span data-ttu-id="8c78c-111">0</span><span class="sxs-lookup"><span data-stu-id="8c78c-111">0</span></span>|<span data-ttu-id="8c78c-112">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="8c78c-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="8c78c-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="8c78c-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="8c78c-114">1</span><span class="sxs-lookup"><span data-stu-id="8c78c-114">1</span></span>|<span data-ttu-id="8c78c-115">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="8c78c-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="8c78c-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="8c78c-116">managedApps</span></span>|<span data-ttu-id="8c78c-117">2</span><span class="sxs-lookup"><span data-stu-id="8c78c-117">2</span></span>|<span data-ttu-id="8c78c-118">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="8c78c-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="8c78c-119">заблокировано</span><span class="sxs-lookup"><span data-stu-id="8c78c-119">blocked</span></span>|<span data-ttu-id="8c78c-120">3</span><span class="sxs-lookup"><span data-stu-id="8c78c-120">3</span></span>|<span data-ttu-id="8c78c-121">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="8c78c-121">Sharing between apps is disabled</span></span>|



