---
title: Регистрация корпоративных устройств с помощью Intune
description: " Сценарий (BYOD)."
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9671eb7f66be78075209906a4f6f923256afef36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928026"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="9d4ea-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="9d4ea-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="9d4ea-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d4ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d4ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d4ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d4ea-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d4ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="9d4ea-107">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="9d4ea-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="9d4ea-108">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="9d4ea-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="9d4ea-109">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="9d4ea-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="9d4ea-110">Профиль развертывания автопилот windows Active directory</span><span class="sxs-lookup"><span data-stu-id="9d4ea-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="9d4ea-111">Azure AD windows автопилот развертывания профилей</span><span class="sxs-lookup"><span data-stu-id="9d4ea-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="9d4ea-112">Предотвращение выполнения данных регистрации основного профиля</span><span class="sxs-lookup"><span data-stu-id="9d4ea-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="9d4ea-113">Предотвращение выполнения данных регистрации профилей</span><span class="sxs-lookup"><span data-stu-id="9d4ea-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="9d4ea-114">Предотвращение выполнения данных профилей регистрации операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="9d4ea-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="9d4ea-115">Предотвращение выполнения данных macOS регистрации профилей</span><span class="sxs-lookup"><span data-stu-id="9d4ea-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="9d4ea-116">Параметр DEP на использование доски</span><span class="sxs-lookup"><span data-stu-id="9d4ea-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="9d4ea-117">Тип токена DEP</span><span class="sxs-lookup"><span data-stu-id="9d4ea-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="9d4ea-118">Обнаружение источника</span><span class="sxs-lookup"><span data-stu-id="9d4ea-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="9d4ea-119">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="9d4ea-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="9d4ea-120">State подачи заявок</span><span class="sxs-lookup"><span data-stu-id="9d4ea-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="9d4ea-121">Импортированные идентификатор устройства Apple</span><span class="sxs-lookup"><span data-stu-id="9d4ea-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="9d4ea-122">Импортировать идентификатор устройства Apple результатов</span><span class="sxs-lookup"><span data-stu-id="9d4ea-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="9d4ea-123">Импортированные устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="9d4ea-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="9d4ea-124">Импортированные результатов идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="9d4ea-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="9d4ea-125">Импортировать тип удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="9d4ea-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="9d4ea-126">Импортированные windows автопилот устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="9d4ea-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="9d4ea-127">Состояние импортированных windows автопилот устройства identity импорта</span><span class="sxs-lookup"><span data-stu-id="9d4ea-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="9d4ea-128">Состояние импортированных windows автопилот устройства удостоверения</span><span class="sxs-lookup"><span data-stu-id="9d4ea-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="9d4ea-129">Отправка identity устройства автопилот импортированных windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="9d4ea-130">Состояние передачи удостоверения устройства автопилот импортированных windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="9d4ea-131">режим связывания iTunes</span><span class="sxs-lookup"><span data-stu-id="9d4ea-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="9d4ea-132">Управление сертификат с отпечатком</span><span class="sxs-lookup"><span data-stu-id="9d4ea-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="9d4ea-133">Параметров качества</span><span class="sxs-lookup"><span data-stu-id="9d4ea-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="9d4ea-134">Платформа</span><span class="sxs-lookup"><span data-stu-id="9d4ea-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="9d4ea-135">Windows автопилот развертывания профилей</span><span class="sxs-lookup"><span data-stu-id="9d4ea-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="9d4ea-136">Назначение профиля развертывания автопилот Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="9d4ea-137">Удостоверения автопилот устройства Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="9d4ea-138">Назначение профиля Windows автопилот подробное описание состояния</span><span class="sxs-lookup"><span data-stu-id="9d4ea-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="9d4ea-139">Состояние назначения профиля автопилот Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="9d4ea-140">Параметры автопилот Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="9d4ea-141">Состояние синхронизации автопилот Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="9d4ea-142">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="9d4ea-143">Параметры экрана состояние регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="9d4ea-144">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="9d4ea-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
