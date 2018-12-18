---
title: Регистрация корпоративных устройств с помощью Intune
description: " Сценарий (BYOD)."
author: tfitzmac
ms.openlocfilehash: f3103d2098053a75839b297eb4ef0a656d6d53a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334323"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="13b5e-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="13b5e-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="13b5e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="13b5e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="13b5e-105">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="13b5e-105">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="13b5e-106">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="13b5e-106">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="13b5e-107">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="13b5e-107">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="13b5e-108">Импортированные windows автопилот устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="13b5e-108">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="13b5e-109">Состояние импортированных windows автопилот устройства identity импорта</span><span class="sxs-lookup"><span data-stu-id="13b5e-109">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="13b5e-110">Состояние импортированных windows автопилот устройства удостоверения</span><span class="sxs-lookup"><span data-stu-id="13b5e-110">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="13b5e-111">Отправка identity устройства автопилот импортированных windows</span><span class="sxs-lookup"><span data-stu-id="13b5e-111">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="13b5e-112">Состояние передачи удостоверения устройства автопилот импортированных windows</span><span class="sxs-lookup"><span data-stu-id="13b5e-112">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
