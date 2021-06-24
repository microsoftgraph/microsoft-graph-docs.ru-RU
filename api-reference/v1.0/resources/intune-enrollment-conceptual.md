---
title: Регистрация корпоративных устройств с помощью Intune - Microsoft Graph API
description: Перечисляет API Graph Microsoft для конечных точек Intune (REST), которые регистрировать устройства для организации-клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daefbf23d8aa70cdd3f81fdcb4afb69dd2590ba7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108941"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="4d68a-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="4d68a-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="4d68a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d68a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d68a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d68a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d68a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d68a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d68a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d68a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d68a-108">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="4d68a-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="4d68a-109">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="4d68a-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="4d68a-110">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="4d68a-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="4d68a-111">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="4d68a-111">Device management</span></span>](intune-enrollment-devicemanagement.md)
- [<span data-ttu-id="4d68a-112">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="4d68a-112">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="4d68a-113">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="4d68a-113">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="4d68a-114">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="4d68a-114">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="4d68a-115">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="4d68a-115">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="4d68a-116">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4d68a-116">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="4d68a-117">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="4d68a-117">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)