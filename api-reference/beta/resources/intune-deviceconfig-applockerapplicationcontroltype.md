---
title: тип перечисления Апплоккераппликатионконтролтипе
description: Возможные значения типов элементов управления приложения AppLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e645f0ee8201ee0e66fe21ce80cc237f52faa3a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260826"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c7d05-103">тип перечисления Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="c7d05-103">appLockerApplicationControlType enum type</span></span>

<span data-ttu-id="c7d05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7d05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7d05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7d05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d05-107">Возможные значения типов элементов управления приложения AppLocker</span><span class="sxs-lookup"><span data-stu-id="c7d05-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="c7d05-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c7d05-108">Members</span></span>
|<span data-ttu-id="c7d05-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c7d05-109">Member</span></span>|<span data-ttu-id="c7d05-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c7d05-110">Value</span></span>|<span data-ttu-id="c7d05-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d05-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d05-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c7d05-112">notConfigured</span></span>|<span data-ttu-id="c7d05-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c7d05-113">0</span></span>|<span data-ttu-id="c7d05-114">Значение по умолчанию для устройства, тип элемента управления приложения не выбран.</span><span class="sxs-lookup"><span data-stu-id="c7d05-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c7d05-115">енфорцекомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="c7d05-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c7d05-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c7d05-116">1</span></span>|<span data-ttu-id="c7d05-117">Принудительное применение компонентов Windows и сохранение приложений.</span><span class="sxs-lookup"><span data-stu-id="c7d05-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c7d05-118">аудиткомпонентсандстореаппс</span><span class="sxs-lookup"><span data-stu-id="c7d05-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c7d05-119">2</span><span class="sxs-lookup"><span data-stu-id="c7d05-119">2</span></span>|<span data-ttu-id="c7d05-120">Аудит компонентов Windows и хранение приложений.</span><span class="sxs-lookup"><span data-stu-id="c7d05-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c7d05-121">енфорцекомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="c7d05-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c7d05-122">4</span><span class="sxs-lookup"><span data-stu-id="c7d05-122">3</span></span>|<span data-ttu-id="c7d05-123">Принудительное применение компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="c7d05-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c7d05-124">аудиткомпонентсстореаппсандсмартлоккер</span><span class="sxs-lookup"><span data-stu-id="c7d05-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c7d05-125">4 </span><span class="sxs-lookup"><span data-stu-id="c7d05-125">4</span></span>|<span data-ttu-id="c7d05-126">Аудит компонентов Windows, хранение приложений и интеллектуальных блокировок.</span><span class="sxs-lookup"><span data-stu-id="c7d05-126">Audit Windows components, store apps and smart locker.</span></span>|




