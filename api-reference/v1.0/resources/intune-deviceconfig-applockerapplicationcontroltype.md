---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871983"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="2d839-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="2d839-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="2d839-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d839-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d839-105">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="2d839-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="2d839-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d839-106">Members</span></span>
|<span data-ttu-id="2d839-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d839-107">Member</span></span>|<span data-ttu-id="2d839-108">Значение</span><span class="sxs-lookup"><span data-stu-id="2d839-108">Value</span></span>|<span data-ttu-id="2d839-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2d839-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d839-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2d839-110">notConfigured</span></span>|<span data-ttu-id="2d839-111">0</span><span class="sxs-lookup"><span data-stu-id="2d839-111">0</span></span>|<span data-ttu-id="2d839-112">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="2d839-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="2d839-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="2d839-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="2d839-114">1</span><span class="sxs-lookup"><span data-stu-id="2d839-114">1</span></span>|<span data-ttu-id="2d839-115">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="2d839-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="2d839-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="2d839-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="2d839-117">2</span><span class="sxs-lookup"><span data-stu-id="2d839-117">2</span></span>|<span data-ttu-id="2d839-118">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="2d839-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="2d839-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="2d839-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="2d839-120">3</span><span class="sxs-lookup"><span data-stu-id="2d839-120">3</span></span>|<span data-ttu-id="2d839-121">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="2d839-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="2d839-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="2d839-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="2d839-123">4</span><span class="sxs-lookup"><span data-stu-id="2d839-123">4</span></span>|<span data-ttu-id="2d839-124">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="2d839-124">Audit Windows components, store apps and smart locker.</span></span>|



