---
title: тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе
description: Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7eb22977f571d0e15e8d9cd20f3ee02e52faff7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216742"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="c5f1a-103">тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="c5f1a-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="c5f1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5f1a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f1a-107">Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="c5f1a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5f1a-108">Members</span></span>
|<span data-ttu-id="c5f1a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5f1a-109">Member</span></span>|<span data-ttu-id="c5f1a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f1a-110">Value</span></span>|<span data-ttu-id="c5f1a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f1a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c5f1a-112">notConfigured</span></span>|<span data-ttu-id="c5f1a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c5f1a-113">0</span></span>|<span data-ttu-id="c5f1a-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="c5f1a-115">усерчоице</span><span class="sxs-lookup"><span data-stu-id="c5f1a-115">userChoice</span></span>|<span data-ttu-id="c5f1a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c5f1a-116">1</span></span>|<span data-ttu-id="c5f1a-117">Пользователь может управлять автоматическим обновлением.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="c5f1a-118">ключа</span><span class="sxs-lookup"><span data-stu-id="c5f1a-118">never</span></span>|<span data-ttu-id="c5f1a-119">2</span><span class="sxs-lookup"><span data-stu-id="c5f1a-119">2</span></span>|<span data-ttu-id="c5f1a-120">Приложения никогда не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="c5f1a-121">вифионли</span><span class="sxs-lookup"><span data-stu-id="c5f1a-121">wiFiOnly</span></span>|<span data-ttu-id="c5f1a-122">4</span><span class="sxs-lookup"><span data-stu-id="c5f1a-122">3</span></span>|<span data-ttu-id="c5f1a-123">Приложения автоматически обновляются только на Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="c5f1a-124">Постоянное</span><span class="sxs-lookup"><span data-stu-id="c5f1a-124">always</span></span>|<span data-ttu-id="c5f1a-125">4 </span><span class="sxs-lookup"><span data-stu-id="c5f1a-125">4</span></span>|<span data-ttu-id="c5f1a-126">Приложения автоматически обновляются в любое время.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="c5f1a-127">Может взиматься плата за передачу данных.</span><span class="sxs-lookup"><span data-stu-id="c5f1a-127">Data charges may apply.</span></span>|




