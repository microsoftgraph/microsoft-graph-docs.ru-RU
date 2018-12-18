---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330207"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="1f8c1-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1f8c1-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="1f8c1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f8c1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f8c1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f8c1-107">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="1f8c1-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="1f8c1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1f8c1-108">Members</span></span>
|<span data-ttu-id="1f8c1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1f8c1-109">Member</span></span>|<span data-ttu-id="1f8c1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1f8c1-110">Value</span></span>|<span data-ttu-id="1f8c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f8c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f8c1-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1f8c1-112">notConfigured</span></span>|<span data-ttu-id="1f8c1-113">0</span><span class="sxs-lookup"><span data-stu-id="1f8c1-113">0</span></span>|<span data-ttu-id="1f8c1-114">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="1f8c1-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1f8c1-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="1f8c1-116">1</span><span class="sxs-lookup"><span data-stu-id="1f8c1-116">1</span></span>|<span data-ttu-id="1f8c1-117">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="1f8c1-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1f8c1-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="1f8c1-119">2</span><span class="sxs-lookup"><span data-stu-id="1f8c1-119">2</span></span>|<span data-ttu-id="1f8c1-120">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="1f8c1-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1f8c1-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1f8c1-122">3</span><span class="sxs-lookup"><span data-stu-id="1f8c1-122">3</span></span>|<span data-ttu-id="1f8c1-123">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="1f8c1-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1f8c1-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1f8c1-125">4</span><span class="sxs-lookup"><span data-stu-id="1f8c1-125">4</span></span>|<span data-ttu-id="1f8c1-126">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="1f8c1-126">Audit Windows components, store apps and smart locker.</span></span>|





