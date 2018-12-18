---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
ms.openlocfilehash: d53c2d0f7996edfab610e4206f4d2815ba4000b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310264"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c28b5-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="c28b5-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="c28b5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c28b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c28b5-105">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="c28b5-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="c28b5-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c28b5-106">Members</span></span>
|<span data-ttu-id="c28b5-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c28b5-107">Member</span></span>|<span data-ttu-id="c28b5-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c28b5-108">Value</span></span>|<span data-ttu-id="c28b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c28b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c28b5-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c28b5-110">notConfigured</span></span>|<span data-ttu-id="c28b5-111">0</span><span class="sxs-lookup"><span data-stu-id="c28b5-111">0</span></span>|<span data-ttu-id="c28b5-112">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="c28b5-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c28b5-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c28b5-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c28b5-114">1</span><span class="sxs-lookup"><span data-stu-id="c28b5-114">1</span></span>|<span data-ttu-id="c28b5-115">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="c28b5-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c28b5-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c28b5-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c28b5-117">2</span><span class="sxs-lookup"><span data-stu-id="c28b5-117">2</span></span>|<span data-ttu-id="c28b5-118">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="c28b5-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c28b5-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c28b5-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c28b5-120">3</span><span class="sxs-lookup"><span data-stu-id="c28b5-120">3</span></span>|<span data-ttu-id="c28b5-121">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="c28b5-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c28b5-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c28b5-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c28b5-123">4</span><span class="sxs-lookup"><span data-stu-id="c28b5-123">4</span></span>|<span data-ttu-id="c28b5-124">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="c28b5-124">Audit Windows components, store apps and smart locker.</span></span>|



