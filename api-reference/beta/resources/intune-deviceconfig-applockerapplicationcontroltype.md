---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425724"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="56f0b-103">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="56f0b-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="56f0b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56f0b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56f0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56f0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56f0b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56f0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56f0b-107">Возможные значения элемента управления типов AppLocker приложений</span><span class="sxs-lookup"><span data-stu-id="56f0b-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="56f0b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="56f0b-108">Members</span></span>
|<span data-ttu-id="56f0b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="56f0b-109">Member</span></span>|<span data-ttu-id="56f0b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="56f0b-110">Value</span></span>|<span data-ttu-id="56f0b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56f0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f0b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="56f0b-112">notConfigured</span></span>|<span data-ttu-id="56f0b-113">0</span><span class="sxs-lookup"><span data-stu-id="56f0b-113">0</span></span>|<span data-ttu-id="56f0b-114">Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.</span><span class="sxs-lookup"><span data-stu-id="56f0b-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="56f0b-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="56f0b-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="56f0b-116">1</span><span class="sxs-lookup"><span data-stu-id="56f0b-116">1</span></span>|<span data-ttu-id="56f0b-117">Принудительное применение компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="56f0b-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="56f0b-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="56f0b-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="56f0b-119">2</span><span class="sxs-lookup"><span data-stu-id="56f0b-119">2</span></span>|<span data-ttu-id="56f0b-120">Аудит компонента и хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="56f0b-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="56f0b-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="56f0b-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="56f0b-122">3</span><span class="sxs-lookup"><span data-stu-id="56f0b-122">3</span></span>|<span data-ttu-id="56f0b-123">Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="56f0b-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="56f0b-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="56f0b-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="56f0b-125">4</span><span class="sxs-lookup"><span data-stu-id="56f0b-125">4</span></span>|<span data-ttu-id="56f0b-126">Аудит компонентов Windows, хранилища приложений и смарт-корзины.</span><span class="sxs-lookup"><span data-stu-id="56f0b-126">Audit Windows components, store apps and smart locker.</span></span>|




