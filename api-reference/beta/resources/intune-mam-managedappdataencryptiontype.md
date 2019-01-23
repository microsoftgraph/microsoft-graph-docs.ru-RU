---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413691"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="5743f-103">Тип перечисления managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="5743f-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="5743f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5743f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5743f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5743f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5743f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5743f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5743f-107">Представляет уровень, на который приложение шифрование для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="5743f-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="5743f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5743f-108">Members</span></span>
|<span data-ttu-id="5743f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5743f-109">Member</span></span>|<span data-ttu-id="5743f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5743f-110">Value</span></span>|<span data-ttu-id="5743f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5743f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5743f-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="5743f-112">useDeviceSettings</span></span>|<span data-ttu-id="5743f-113">0</span><span class="sxs-lookup"><span data-stu-id="5743f-113">0</span></span>|<span data-ttu-id="5743f-114">Приложение шифрование на основе параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5743f-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="5743f-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="5743f-115">afterDeviceRestart</span></span>|<span data-ttu-id="5743f-116">1</span><span class="sxs-lookup"><span data-stu-id="5743f-116">1</span></span>|<span data-ttu-id="5743f-117">Приложение шифрование при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="5743f-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="5743f-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="5743f-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="5743f-119">2</span><span class="sxs-lookup"><span data-stu-id="5743f-119">2</span></span>|<span data-ttu-id="5743f-120">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых</span><span class="sxs-lookup"><span data-stu-id="5743f-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="5743f-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="5743f-121">whenDeviceLocked</span></span>|<span data-ttu-id="5743f-122">3</span><span class="sxs-lookup"><span data-stu-id="5743f-122">3</span></span>|<span data-ttu-id="5743f-123">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство</span><span class="sxs-lookup"><span data-stu-id="5743f-123">App data associated with this policy is encrypted when the device is locked</span></span>|




