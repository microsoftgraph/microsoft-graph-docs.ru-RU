---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f57904d45b24f6aaae9d67394facb07692add67e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834148"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="ee8e7-103">Тип перечисления managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="ee8e7-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="ee8e7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee8e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee8e7-105">Представляет уровень, на который приложение шифрование для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ee8e7-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="ee8e7-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ee8e7-106">Members</span></span>
|<span data-ttu-id="ee8e7-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ee8e7-107">Member</span></span>|<span data-ttu-id="ee8e7-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ee8e7-108">Value</span></span>|<span data-ttu-id="ee8e7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ee8e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8e7-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="ee8e7-110">useDeviceSettings</span></span>|<span data-ttu-id="ee8e7-111">0</span><span class="sxs-lookup"><span data-stu-id="ee8e7-111">0</span></span>|<span data-ttu-id="ee8e7-112">Приложение шифрование на основе параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ee8e7-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="ee8e7-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="ee8e7-113">afterDeviceRestart</span></span>|<span data-ttu-id="ee8e7-114">1</span><span class="sxs-lookup"><span data-stu-id="ee8e7-114">1</span></span>|<span data-ttu-id="ee8e7-115">Приложение шифрование при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="ee8e7-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="ee8e7-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="ee8e7-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="ee8e7-117">2</span><span class="sxs-lookup"><span data-stu-id="ee8e7-117">2</span></span>|<span data-ttu-id="ee8e7-118">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых</span><span class="sxs-lookup"><span data-stu-id="ee8e7-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="ee8e7-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="ee8e7-119">whenDeviceLocked</span></span>|<span data-ttu-id="ee8e7-120">3</span><span class="sxs-lookup"><span data-stu-id="ee8e7-120">3</span></span>|<span data-ttu-id="ee8e7-121">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство</span><span class="sxs-lookup"><span data-stu-id="ee8e7-121">App data associated with this policy is encrypted when the device is locked</span></span>|



