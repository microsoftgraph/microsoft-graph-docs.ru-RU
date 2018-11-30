---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027237"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="0da61-103">Тип перечисления managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="0da61-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="0da61-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0da61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0da61-105">Представляет уровень, на который приложение шифрование для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="0da61-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="0da61-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="0da61-106">Members</span></span>
|<span data-ttu-id="0da61-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="0da61-107">Member</span></span>|<span data-ttu-id="0da61-108">Значение</span><span class="sxs-lookup"><span data-stu-id="0da61-108">Value</span></span>|<span data-ttu-id="0da61-109">Description</span><span class="sxs-lookup"><span data-stu-id="0da61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da61-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="0da61-110">useDeviceSettings</span></span>|<span data-ttu-id="0da61-111">0</span><span class="sxs-lookup"><span data-stu-id="0da61-111">0</span></span>|<span data-ttu-id="0da61-112">Приложение шифрование на основе параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0da61-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="0da61-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="0da61-113">afterDeviceRestart</span></span>|<span data-ttu-id="0da61-114">1</span><span class="sxs-lookup"><span data-stu-id="0da61-114">1</span></span>|<span data-ttu-id="0da61-115">Приложение шифрование при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="0da61-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="0da61-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="0da61-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="0da61-117">2</span><span class="sxs-lookup"><span data-stu-id="0da61-117">2</span></span>|<span data-ttu-id="0da61-118">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых</span><span class="sxs-lookup"><span data-stu-id="0da61-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="0da61-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="0da61-119">whenDeviceLocked</span></span>|<span data-ttu-id="0da61-120">3</span><span class="sxs-lookup"><span data-stu-id="0da61-120">3</span></span>|<span data-ttu-id="0da61-121">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство</span><span class="sxs-lookup"><span data-stu-id="0da61-121">App data associated with this policy is encrypted when the device is locked</span></span>|



