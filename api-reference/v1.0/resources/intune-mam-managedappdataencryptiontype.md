---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e4540826254967be7ed16e3feeb08dd38db4e48e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445786"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="91e98-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="91e98-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="91e98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91e98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91e98-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91e98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e98-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="91e98-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="91e98-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="91e98-107">Members</span></span>
|<span data-ttu-id="91e98-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="91e98-108">Member</span></span>|<span data-ttu-id="91e98-109">Значение</span><span class="sxs-lookup"><span data-stu-id="91e98-109">Value</span></span>|<span data-ttu-id="91e98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91e98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e98-111">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="91e98-111">useDeviceSettings</span></span>|<span data-ttu-id="91e98-112">нуль</span><span class="sxs-lookup"><span data-stu-id="91e98-112">0</span></span>|<span data-ttu-id="91e98-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="91e98-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="91e98-114">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="91e98-114">afterDeviceRestart</span></span>|<span data-ttu-id="91e98-115">1,1</span><span class="sxs-lookup"><span data-stu-id="91e98-115">1</span></span>|<span data-ttu-id="91e98-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="91e98-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="91e98-117">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="91e98-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="91e98-118">2</span><span class="sxs-lookup"><span data-stu-id="91e98-118">2</span></span>|<span data-ttu-id="91e98-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="91e98-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="91e98-120">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="91e98-120">whenDeviceLocked</span></span>|<span data-ttu-id="91e98-121">4</span><span class="sxs-lookup"><span data-stu-id="91e98-121">3</span></span>|<span data-ttu-id="91e98-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="91e98-122">App data associated with this policy is encrypted when the device is locked</span></span>|







