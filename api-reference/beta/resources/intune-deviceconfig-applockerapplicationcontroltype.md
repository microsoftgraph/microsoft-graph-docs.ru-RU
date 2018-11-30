---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
ms.openlocfilehash: 150e3daa6b8deb2d1e17c3ea7caf345ba39446f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077227"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="74e29-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="74e29-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="74e29-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74e29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74e29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74e29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74e29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74e29-107">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="74e29-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="74e29-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="74e29-108">Members</span></span>
|<span data-ttu-id="74e29-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="74e29-109">Member</span></span>|<span data-ttu-id="74e29-110">Значение</span><span class="sxs-lookup"><span data-stu-id="74e29-110">Value</span></span>|<span data-ttu-id="74e29-111">Description</span><span class="sxs-lookup"><span data-stu-id="74e29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e29-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="74e29-112">notConfigured</span></span>|<span data-ttu-id="74e29-113">0</span><span class="sxs-lookup"><span data-stu-id="74e29-113">0</span></span>|<span data-ttu-id="74e29-114">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="74e29-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="74e29-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="74e29-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="74e29-116">1</span><span class="sxs-lookup"><span data-stu-id="74e29-116">1</span></span>|<span data-ttu-id="74e29-117">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="74e29-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="74e29-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="74e29-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="74e29-119">2</span><span class="sxs-lookup"><span data-stu-id="74e29-119">2</span></span>|<span data-ttu-id="74e29-120">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="74e29-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="74e29-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="74e29-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="74e29-122">3</span><span class="sxs-lookup"><span data-stu-id="74e29-122">3</span></span>|<span data-ttu-id="74e29-123">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="74e29-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="74e29-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="74e29-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="74e29-125">4</span><span class="sxs-lookup"><span data-stu-id="74e29-125">4</span></span>|<span data-ttu-id="74e29-126">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="74e29-126">Audit Windows components, store apps and smart locker.</span></span>|





