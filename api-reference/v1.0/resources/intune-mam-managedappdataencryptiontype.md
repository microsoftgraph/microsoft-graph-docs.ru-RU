---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c2a4c9b713d2b91645cf210df60ec8d3ba642a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533345"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="f1d6f-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="f1d6f-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="f1d6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1d6f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1d6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d6f-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="f1d6f-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="f1d6f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f1d6f-107">Members</span></span>
|<span data-ttu-id="f1d6f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1d6f-108">Member</span></span>|<span data-ttu-id="f1d6f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f1d6f-109">Value</span></span>|<span data-ttu-id="f1d6f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d6f-111">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="f1d6f-111">useDeviceSettings</span></span>|<span data-ttu-id="f1d6f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f1d6f-112">0</span></span>|<span data-ttu-id="f1d6f-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f1d6f-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="f1d6f-114">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="f1d6f-114">afterDeviceRestart</span></span>|<span data-ttu-id="f1d6f-115">1 </span><span class="sxs-lookup"><span data-stu-id="f1d6f-115">1</span></span>|<span data-ttu-id="f1d6f-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="f1d6f-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="f1d6f-117">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="f1d6f-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="f1d6f-118">2 </span><span class="sxs-lookup"><span data-stu-id="f1d6f-118">2</span></span>|<span data-ttu-id="f1d6f-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="f1d6f-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="f1d6f-120">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="f1d6f-120">whenDeviceLocked</span></span>|<span data-ttu-id="f1d6f-121">3 </span><span class="sxs-lookup"><span data-stu-id="f1d6f-121">3</span></span>|<span data-ttu-id="f1d6f-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="f1d6f-122">App data associated with this policy is encrypted when the device is locked</span></span>|




