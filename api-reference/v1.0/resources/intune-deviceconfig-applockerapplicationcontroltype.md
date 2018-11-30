---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
ms.openlocfilehash: 703cc18dfee49a01adb3cd4f61c5d7e99e30fb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024946"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="586c6-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="586c6-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="586c6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="586c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="586c6-105">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="586c6-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="586c6-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="586c6-106">Members</span></span>
|<span data-ttu-id="586c6-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="586c6-107">Member</span></span>|<span data-ttu-id="586c6-108">Значение</span><span class="sxs-lookup"><span data-stu-id="586c6-108">Value</span></span>|<span data-ttu-id="586c6-109">Description</span><span class="sxs-lookup"><span data-stu-id="586c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="586c6-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="586c6-110">notConfigured</span></span>|<span data-ttu-id="586c6-111">0</span><span class="sxs-lookup"><span data-stu-id="586c6-111">0</span></span>|<span data-ttu-id="586c6-112">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="586c6-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="586c6-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="586c6-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="586c6-114">1</span><span class="sxs-lookup"><span data-stu-id="586c6-114">1</span></span>|<span data-ttu-id="586c6-115">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="586c6-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="586c6-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="586c6-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="586c6-117">2</span><span class="sxs-lookup"><span data-stu-id="586c6-117">2</span></span>|<span data-ttu-id="586c6-118">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="586c6-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="586c6-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="586c6-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="586c6-120">3</span><span class="sxs-lookup"><span data-stu-id="586c6-120">3</span></span>|<span data-ttu-id="586c6-121">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="586c6-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="586c6-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="586c6-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="586c6-123">4</span><span class="sxs-lookup"><span data-stu-id="586c6-123">4</span></span>|<span data-ttu-id="586c6-124">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="586c6-124">Audit Windows components, store apps and smart locker.</span></span>|



