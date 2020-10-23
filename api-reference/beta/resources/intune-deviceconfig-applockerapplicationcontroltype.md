---
title: тип перечисления Апплоккераппликатионконтролтипе
description: Возможные значения типов элементов управления приложения AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: efdb7913d5b813ec528969520e2e7d64da1d3002
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708818"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c368e-103">тип перечисления Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="c368e-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="c368e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c368e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c368e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c368e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c368e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c368e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c368e-107">Возможные значения типов элементов управления приложения AppLocker</span><span class="sxs-lookup"><span data-stu-id="c368e-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="c368e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c368e-108">Members</span></span>
|<span data-ttu-id="c368e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c368e-109">Member</span></span>|<span data-ttu-id="c368e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c368e-110">Value</span></span>|<span data-ttu-id="c368e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c368e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c368e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c368e-112">notConfigured</span></span>|<span data-ttu-id="c368e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c368e-113">0</span></span>|<span data-ttu-id="c368e-114">Значение по умолчанию для устройства, тип элемента управления приложения не выбран.</span><span class="sxs-lookup"><span data-stu-id="c368e-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c368e-115">енфорцекомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="c368e-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c368e-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c368e-116">1</span></span>|<span data-ttu-id="c368e-117">Принудительное применение компонентов Windows и сохранение приложений.</span><span class="sxs-lookup"><span data-stu-id="c368e-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c368e-118">аудиткомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="c368e-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c368e-119">2</span><span class="sxs-lookup"><span data-stu-id="c368e-119">2</span></span>|<span data-ttu-id="c368e-120">Аудит компонентов Windows и хранение приложений.</span><span class="sxs-lookup"><span data-stu-id="c368e-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c368e-121">енфорцекомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="c368e-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c368e-122">4</span><span class="sxs-lookup"><span data-stu-id="c368e-122">3</span></span>|<span data-ttu-id="c368e-123">Принудительное применение компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="c368e-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c368e-124">аудиткомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="c368e-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c368e-125">4 </span><span class="sxs-lookup"><span data-stu-id="c368e-125">4</span></span>|<span data-ttu-id="c368e-126">Аудит компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="c368e-126">Audit Windows components, store apps and smart locker.</span></span>|





