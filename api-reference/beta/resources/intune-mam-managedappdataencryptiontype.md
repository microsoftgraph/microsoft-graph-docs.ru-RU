---
title: Тип перечисления managedAppDataEncryptionType
description: Представляет уровень, на который приложение шифрование для управляемых приложений
author: tfitzmac
ms.openlocfilehash: 6bd23f6cd590724c2c981ddf2c3087ead4c21817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326119"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="a8ff1-103">Тип перечисления managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="a8ff1-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="a8ff1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8ff1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8ff1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ff1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8ff1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8ff1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8ff1-107">Представляет уровень, на который приложение шифрование для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="a8ff1-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="a8ff1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a8ff1-108">Members</span></span>
|<span data-ttu-id="a8ff1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a8ff1-109">Member</span></span>|<span data-ttu-id="a8ff1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a8ff1-110">Value</span></span>|<span data-ttu-id="a8ff1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ff1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8ff1-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="a8ff1-112">useDeviceSettings</span></span>|<span data-ttu-id="a8ff1-113">0</span><span class="sxs-lookup"><span data-stu-id="a8ff1-113">0</span></span>|<span data-ttu-id="a8ff1-114">Приложение шифрование на основе параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a8ff1-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="a8ff1-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="a8ff1-115">afterDeviceRestart</span></span>|<span data-ttu-id="a8ff1-116">1</span><span class="sxs-lookup"><span data-stu-id="a8ff1-116">1</span></span>|<span data-ttu-id="a8ff1-117">Приложение шифрование при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="a8ff1-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="a8ff1-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="a8ff1-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="a8ff1-119">2</span><span class="sxs-lookup"><span data-stu-id="a8ff1-119">2</span></span>|<span data-ttu-id="a8ff1-120">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство, за исключением данных в файлах, открытых</span><span class="sxs-lookup"><span data-stu-id="a8ff1-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="a8ff1-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="a8ff1-121">whenDeviceLocked</span></span>|<span data-ttu-id="a8ff1-122">3</span><span class="sxs-lookup"><span data-stu-id="a8ff1-122">3</span></span>|<span data-ttu-id="a8ff1-123">Данные приложения, связанные с этой политикой шифруются при заблокированном устройство</span><span class="sxs-lookup"><span data-stu-id="a8ff1-123">App data associated with this policy is encrypted when the device is locked</span></span>|





