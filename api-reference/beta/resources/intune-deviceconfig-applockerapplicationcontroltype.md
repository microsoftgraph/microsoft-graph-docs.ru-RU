---
title: тип перечисления Апплоккераппликатионконтролтипе
description: Возможные значения типов элементов управления приложения AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22d108dd3bad90341031d1e965948a9daa59efa1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141358"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="27d93-103">тип перечисления Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="27d93-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="27d93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27d93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27d93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27d93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27d93-106">Возможные значения типов элементов управления приложения AppLocker</span><span class="sxs-lookup"><span data-stu-id="27d93-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="27d93-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="27d93-107">Members</span></span>
|<span data-ttu-id="27d93-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="27d93-108">Member</span></span>|<span data-ttu-id="27d93-109">Значение</span><span class="sxs-lookup"><span data-stu-id="27d93-109">Value</span></span>|<span data-ttu-id="27d93-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27d93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d93-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="27d93-111">notConfigured</span></span>|<span data-ttu-id="27d93-112">нуль</span><span class="sxs-lookup"><span data-stu-id="27d93-112">0</span></span>|<span data-ttu-id="27d93-113">Значение по умолчанию для устройства, тип элемента управления приложения не выбран.</span><span class="sxs-lookup"><span data-stu-id="27d93-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="27d93-114">Енфорцекомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="27d93-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="27d93-115">1,1</span><span class="sxs-lookup"><span data-stu-id="27d93-115">1</span></span>|<span data-ttu-id="27d93-116">Принудительное применение компонентов Windows и сохранение приложений.</span><span class="sxs-lookup"><span data-stu-id="27d93-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="27d93-117">Аудиткомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="27d93-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="27d93-118">2</span><span class="sxs-lookup"><span data-stu-id="27d93-118">2</span></span>|<span data-ttu-id="27d93-119">Аудит компонентов Windows и хранение приложений.</span><span class="sxs-lookup"><span data-stu-id="27d93-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="27d93-120">Енфорцекомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="27d93-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="27d93-121">4</span><span class="sxs-lookup"><span data-stu-id="27d93-121">3</span></span>|<span data-ttu-id="27d93-122">Принудительное применение компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="27d93-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="27d93-123">Аудиткомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="27d93-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="27d93-124">4</span><span class="sxs-lookup"><span data-stu-id="27d93-124">4</span></span>|<span data-ttu-id="27d93-125">Аудит компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="27d93-125">Audit Windows components, store apps and smart locker.</span></span>|




