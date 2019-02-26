---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256772"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="82a39-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="82a39-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="82a39-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82a39-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a39-105">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="82a39-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="82a39-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="82a39-106">Members</span></span>
|<span data-ttu-id="82a39-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="82a39-107">Member</span></span>|<span data-ttu-id="82a39-108">Значение</span><span class="sxs-lookup"><span data-stu-id="82a39-108">Value</span></span>|<span data-ttu-id="82a39-109">Описание</span><span class="sxs-lookup"><span data-stu-id="82a39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82a39-110">Уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="82a39-110">useDeviceSettings</span></span>|<span data-ttu-id="82a39-111">нуль</span><span class="sxs-lookup"><span data-stu-id="82a39-111">0</span></span>|<span data-ttu-id="82a39-112">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82a39-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="82a39-113">Афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="82a39-113">afterDeviceRestart</span></span>|<span data-ttu-id="82a39-114">1,1</span><span class="sxs-lookup"><span data-stu-id="82a39-114">1</span></span>|<span data-ttu-id="82a39-115">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="82a39-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="82a39-116">Вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="82a39-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="82a39-117">2</span><span class="sxs-lookup"><span data-stu-id="82a39-117">2</span></span>|<span data-ttu-id="82a39-118">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="82a39-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="82a39-119">Вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="82a39-119">whenDeviceLocked</span></span>|<span data-ttu-id="82a39-120">4</span><span class="sxs-lookup"><span data-stu-id="82a39-120">3</span></span>|<span data-ttu-id="82a39-121">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="82a39-121">App data associated with this policy is encrypted when the device is locked</span></span>|



