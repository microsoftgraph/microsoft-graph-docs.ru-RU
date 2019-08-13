---
title: тип перечисления Манажедаппдатаенкриптионтипе
description: Представляет уровень, на который данные приложения шифруются для управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 273303044af0ed6b5a13c1221e99e00ccd57026e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332178"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="abfdf-103">тип перечисления Манажедаппдатаенкриптионтипе</span><span class="sxs-lookup"><span data-stu-id="abfdf-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="abfdf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abfdf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abfdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abfdf-106">Представляет уровень, на который данные приложения шифруются для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="abfdf-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="abfdf-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="abfdf-107">Members</span></span>
|<span data-ttu-id="abfdf-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="abfdf-108">Member</span></span>|<span data-ttu-id="abfdf-109">Значение</span><span class="sxs-lookup"><span data-stu-id="abfdf-109">Value</span></span>|<span data-ttu-id="abfdf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="abfdf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abfdf-111">уседевицесеттингс</span><span class="sxs-lookup"><span data-stu-id="abfdf-111">useDeviceSettings</span></span>|<span data-ttu-id="abfdf-112">нуль</span><span class="sxs-lookup"><span data-stu-id="abfdf-112">0</span></span>|<span data-ttu-id="abfdf-113">Данные приложений шифруются на основе параметров, используемых по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="abfdf-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="abfdf-114">афтердевицерестарт</span><span class="sxs-lookup"><span data-stu-id="abfdf-114">afterDeviceRestart</span></span>|<span data-ttu-id="abfdf-115">1,1</span><span class="sxs-lookup"><span data-stu-id="abfdf-115">1</span></span>|<span data-ttu-id="abfdf-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="abfdf-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="abfdf-117">вхендевицелоккедексцептопенфилес</span><span class="sxs-lookup"><span data-stu-id="abfdf-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="abfdf-118">2</span><span class="sxs-lookup"><span data-stu-id="abfdf-118">2</span></span>|<span data-ttu-id="abfdf-119">Данные приложения, связанные с этой политикой, шифруются, если устройство заблокировано, за исключением данных в открытых файлах.</span><span class="sxs-lookup"><span data-stu-id="abfdf-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="abfdf-120">вхендевицелоккед</span><span class="sxs-lookup"><span data-stu-id="abfdf-120">whenDeviceLocked</span></span>|<span data-ttu-id="abfdf-121">4</span><span class="sxs-lookup"><span data-stu-id="abfdf-121">3</span></span>|<span data-ttu-id="abfdf-122">Данные о приложении, связанные с этой политикой, шифруются, когда устройство заблокировано</span><span class="sxs-lookup"><span data-stu-id="abfdf-122">App data associated with this policy is encrypted when the device is locked</span></span>|



