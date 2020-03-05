---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 62e329c2fa400689c708b4155ea5145bc8eaed34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527951"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="c61ee-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="c61ee-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="c61ee-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c61ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c61ee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c61ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c61ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c61ee-107">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="c61ee-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="c61ee-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c61ee-108">Members</span></span>
|<span data-ttu-id="c61ee-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c61ee-109">Member</span></span>|<span data-ttu-id="c61ee-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c61ee-110">Value</span></span>|<span data-ttu-id="c61ee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c61ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c61ee-112">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="c61ee-112">useDeviceSettings</span></span>|<span data-ttu-id="c61ee-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c61ee-113">0</span></span>|<span data-ttu-id="c61ee-114">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c61ee-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="c61ee-115">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="c61ee-115">afterDeviceRestart</span></span>|<span data-ttu-id="c61ee-116">1 </span><span class="sxs-lookup"><span data-stu-id="c61ee-116">1</span></span>|<span data-ttu-id="c61ee-117">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="c61ee-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="c61ee-118">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="c61ee-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="c61ee-119">2 </span><span class="sxs-lookup"><span data-stu-id="c61ee-119">2</span></span>|<span data-ttu-id="c61ee-120">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="c61ee-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="c61ee-121">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="c61ee-121">whenDeviceLocked</span></span>|<span data-ttu-id="c61ee-122">3 </span><span class="sxs-lookup"><span data-stu-id="c61ee-122">3</span></span>|<span data-ttu-id="c61ee-123">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="c61ee-123">App data associated with this policy is encrypted when the device is locked</span></span>|



