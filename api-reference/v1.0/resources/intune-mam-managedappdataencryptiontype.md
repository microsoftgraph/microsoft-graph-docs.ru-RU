---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b3e2cc44e1d548a1abe2a4d34c02fef9db7750a1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356389"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="93a9f-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="93a9f-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="93a9f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93a9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93a9f-105">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="93a9f-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="93a9f-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="93a9f-106">Members</span></span>
|<span data-ttu-id="93a9f-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="93a9f-107">Member</span></span>|<span data-ttu-id="93a9f-108">Значение</span><span class="sxs-lookup"><span data-stu-id="93a9f-108">Value</span></span>|<span data-ttu-id="93a9f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="93a9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93a9f-110">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="93a9f-110">useDeviceSettings</span></span>|<span data-ttu-id="93a9f-111">нуль</span><span class="sxs-lookup"><span data-stu-id="93a9f-111">0</span></span>|<span data-ttu-id="93a9f-112">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="93a9f-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="93a9f-113">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="93a9f-113">afterDeviceRestart</span></span>|<span data-ttu-id="93a9f-114">1,1</span><span class="sxs-lookup"><span data-stu-id="93a9f-114">1</span></span>|<span data-ttu-id="93a9f-115">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="93a9f-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="93a9f-116">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="93a9f-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="93a9f-117">2</span><span class="sxs-lookup"><span data-stu-id="93a9f-117">2</span></span>|<span data-ttu-id="93a9f-118">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="93a9f-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="93a9f-119">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="93a9f-119">whenDeviceLocked</span></span>|<span data-ttu-id="93a9f-120">4</span><span class="sxs-lookup"><span data-stu-id="93a9f-120">3</span></span>|<span data-ttu-id="93a9f-121">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="93a9f-121">App data associated with this policy is encrypted when the device is locked</span></span>|




