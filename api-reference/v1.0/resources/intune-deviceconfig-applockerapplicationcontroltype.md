---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937959"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="6cdbe-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="6cdbe-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="6cdbe-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cdbe-105">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="6cdbe-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="6cdbe-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6cdbe-106">Members</span></span>
|<span data-ttu-id="6cdbe-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6cdbe-107">Member</span></span>|<span data-ttu-id="6cdbe-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6cdbe-108">Value</span></span>|<span data-ttu-id="6cdbe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6cdbe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cdbe-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6cdbe-110">notConfigured</span></span>|<span data-ttu-id="6cdbe-111">0</span><span class="sxs-lookup"><span data-stu-id="6cdbe-111">0</span></span>|<span data-ttu-id="6cdbe-112">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="6cdbe-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6cdbe-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="6cdbe-114">1</span><span class="sxs-lookup"><span data-stu-id="6cdbe-114">1</span></span>|<span data-ttu-id="6cdbe-115">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="6cdbe-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6cdbe-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="6cdbe-117">2</span><span class="sxs-lookup"><span data-stu-id="6cdbe-117">2</span></span>|<span data-ttu-id="6cdbe-118">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="6cdbe-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6cdbe-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6cdbe-120">3</span><span class="sxs-lookup"><span data-stu-id="6cdbe-120">3</span></span>|<span data-ttu-id="6cdbe-121">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="6cdbe-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6cdbe-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6cdbe-123">4</span><span class="sxs-lookup"><span data-stu-id="6cdbe-123">4</span></span>|<span data-ttu-id="6cdbe-124">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="6cdbe-124">Audit Windows components, store apps and smart locker.</span></span>|



