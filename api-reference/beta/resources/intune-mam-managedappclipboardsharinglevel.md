---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410989"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="ce2fb-103">Тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="ce2fb-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="ce2fb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce2fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce2fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce2fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce2fb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce2fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2fb-107">Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений</span><span class="sxs-lookup"><span data-stu-id="ce2fb-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="ce2fb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce2fb-108">Members</span></span>
|<span data-ttu-id="ce2fb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ce2fb-109">Member</span></span>|<span data-ttu-id="ce2fb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ce2fb-110">Value</span></span>|<span data-ttu-id="ce2fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ce2fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2fb-112">allApps</span><span class="sxs-lookup"><span data-stu-id="ce2fb-112">allApps</span></span>|<span data-ttu-id="ce2fb-113">0</span><span class="sxs-lookup"><span data-stu-id="ce2fb-113">0</span></span>|<span data-ttu-id="ce2fb-114">Общий доступ к может между всем приложениям, управляемых или нет</span><span class="sxs-lookup"><span data-stu-id="ce2fb-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="ce2fb-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="ce2fb-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="ce2fb-116">1</span><span class="sxs-lookup"><span data-stu-id="ce2fb-116">1</span></span>|<span data-ttu-id="ce2fb-117">Общий доступ к может между все управляемые приложения с помощью вставки в включено</span><span class="sxs-lookup"><span data-stu-id="ce2fb-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="ce2fb-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="ce2fb-118">managedApps</span></span>|<span data-ttu-id="ce2fb-119">2</span><span class="sxs-lookup"><span data-stu-id="ce2fb-119">2</span></span>|<span data-ttu-id="ce2fb-120">Общий доступ к может между все управляемые приложения</span><span class="sxs-lookup"><span data-stu-id="ce2fb-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="ce2fb-121">заблокировано</span><span class="sxs-lookup"><span data-stu-id="ce2fb-121">blocked</span></span>|<span data-ttu-id="ce2fb-122">3</span><span class="sxs-lookup"><span data-stu-id="ce2fb-122">3</span></span>|<span data-ttu-id="ce2fb-123">Совместное использование приложений отключена</span><span class="sxs-lookup"><span data-stu-id="ce2fb-123">Sharing between apps is disabled</span></span>|




