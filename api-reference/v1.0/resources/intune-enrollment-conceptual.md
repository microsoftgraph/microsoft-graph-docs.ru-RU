---
title: Регистрация корпоративных устройств с помощью Intune
description: " Сценарий (BYOD)."
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 840fec00f32cd33093bc965157b35af16bb43248
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530266"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="2d54a-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="2d54a-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="2d54a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d54a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d54a-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d54a-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="2d54a-106">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="2d54a-106">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="2d54a-107">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="2d54a-107">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="2d54a-108">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="2d54a-108">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="2d54a-109">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2d54a-109">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="2d54a-110">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2d54a-110">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="2d54a-111">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2d54a-111">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="2d54a-112">Загрузка импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="2d54a-112">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="2d54a-113">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="2d54a-113">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)

