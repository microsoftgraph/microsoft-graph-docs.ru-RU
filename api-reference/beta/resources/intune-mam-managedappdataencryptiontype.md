---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962e759e83b08baf7fc150e07dc84ed7146feb0b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799533"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="c28b5-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="c28b5-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="c28b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c28b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c28b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c28b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c28b5-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="c28b5-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="c28b5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c28b5-107">Members</span></span>
|<span data-ttu-id="c28b5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c28b5-108">Member</span></span>|<span data-ttu-id="c28b5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c28b5-109">Value</span></span>|<span data-ttu-id="c28b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c28b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c28b5-111">Уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="c28b5-111">useDeviceSettings</span></span>|<span data-ttu-id="c28b5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c28b5-112">0</span></span>|<span data-ttu-id="c28b5-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c28b5-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="c28b5-114">Афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="c28b5-114">afterDeviceRestart</span></span>|<span data-ttu-id="c28b5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c28b5-115">1</span></span>|<span data-ttu-id="c28b5-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="c28b5-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="c28b5-117">Вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="c28b5-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="c28b5-118">2</span><span class="sxs-lookup"><span data-stu-id="c28b5-118">2</span></span>|<span data-ttu-id="c28b5-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="c28b5-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="c28b5-120">Вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="c28b5-120">whenDeviceLocked</span></span>|<span data-ttu-id="c28b5-121">4</span><span class="sxs-lookup"><span data-stu-id="c28b5-121">3</span></span>|<span data-ttu-id="c28b5-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="c28b5-122">App data associated with this policy is encrypted when the device is locked</span></span>|





