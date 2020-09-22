---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e02d2dd993a31056a19d4c54155b1195e93ab58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074960"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="fd2ee-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="fd2ee-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="fd2ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd2ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd2ee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd2ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd2ee-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fd2ee-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="fd2ee-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="fd2ee-107">Members</span></span>
|<span data-ttu-id="fd2ee-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="fd2ee-108">Member</span></span>|<span data-ttu-id="fd2ee-109">Значение</span><span class="sxs-lookup"><span data-stu-id="fd2ee-109">Value</span></span>|<span data-ttu-id="fd2ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fd2ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd2ee-111">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="fd2ee-111">useDeviceSettings</span></span>|<span data-ttu-id="fd2ee-112">нуль</span><span class="sxs-lookup"><span data-stu-id="fd2ee-112">0</span></span>|<span data-ttu-id="fd2ee-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fd2ee-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="fd2ee-114">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="fd2ee-114">afterDeviceRestart</span></span>|<span data-ttu-id="fd2ee-115">1 </span><span class="sxs-lookup"><span data-stu-id="fd2ee-115">1</span></span>|<span data-ttu-id="fd2ee-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="fd2ee-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="fd2ee-117">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="fd2ee-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="fd2ee-118">2 </span><span class="sxs-lookup"><span data-stu-id="fd2ee-118">2</span></span>|<span data-ttu-id="fd2ee-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="fd2ee-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="fd2ee-120">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="fd2ee-120">whenDeviceLocked</span></span>|<span data-ttu-id="fd2ee-121">4</span><span class="sxs-lookup"><span data-stu-id="fd2ee-121">3</span></span>|<span data-ttu-id="fd2ee-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="fd2ee-122">App data associated with this policy is encrypted when the device is locked</span></span>|









