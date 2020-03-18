---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7f6975710f13816a64b01f7bcabbc1677810bb87
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782155"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="5d5ef-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="5d5ef-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="5d5ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d5ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d5ef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d5ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d5ef-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="5d5ef-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="5d5ef-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5d5ef-107">Members</span></span>
|<span data-ttu-id="5d5ef-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5d5ef-108">Member</span></span>|<span data-ttu-id="5d5ef-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5d5ef-109">Value</span></span>|<span data-ttu-id="5d5ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d5ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d5ef-111">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="5d5ef-111">useDeviceSettings</span></span>|<span data-ttu-id="5d5ef-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5d5ef-112">0</span></span>|<span data-ttu-id="5d5ef-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5d5ef-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="5d5ef-114">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="5d5ef-114">afterDeviceRestart</span></span>|<span data-ttu-id="5d5ef-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5d5ef-115">1</span></span>|<span data-ttu-id="5d5ef-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="5d5ef-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="5d5ef-117">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="5d5ef-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="5d5ef-118">2</span><span class="sxs-lookup"><span data-stu-id="5d5ef-118">2</span></span>|<span data-ttu-id="5d5ef-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="5d5ef-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="5d5ef-120">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="5d5ef-120">whenDeviceLocked</span></span>|<span data-ttu-id="5d5ef-121">4</span><span class="sxs-lookup"><span data-stu-id="5d5ef-121">3</span></span>|<span data-ttu-id="5d5ef-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="5d5ef-122">App data associated with this policy is encrypted when the device is locked</span></span>|



