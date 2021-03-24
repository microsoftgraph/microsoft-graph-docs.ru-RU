---
title: Регистрация корпоративных устройств с помощью Intune - API Microsoft Graph
description: Перечислены API Microsoft Graph для конечных точек Intune (REST), которые регистрировать устройства для организации-клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a85db8c4397659789feafa395195a39542928f01
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131955"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="aa0e8-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="aa0e8-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="aa0e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa0e8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa0e8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa0e8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa0e8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa0e8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa0e8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa0e8-108">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="aa0e8-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="aa0e8-109">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="aa0e8-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="aa0e8-110">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="aa0e8-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="aa0e8-111">Профиль Windows AutoPilot Deployment для Active Directory</span><span class="sxs-lookup"><span data-stu-id="aa0e8-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="aa0e8-112">Назначение профиля регистрации Apple</span><span class="sxs-lookup"><span data-stu-id="aa0e8-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="aa0e8-113">Тип регистрации владельца Apple</span><span class="sxs-lookup"><span data-stu-id="aa0e8-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="aa0e8-114">Пользователь Apple инициировал регистрацию профиля</span><span class="sxs-lookup"><span data-stu-id="aa0e8-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="aa0e8-115">Тип регистрации, инициированный пользователем Apple</span><span class="sxs-lookup"><span data-stu-id="aa0e8-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="aa0e8-116">Профиль Windows AutoPilot Deployment для Azure AD</span><span class="sxs-lookup"><span data-stu-id="aa0e8-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="aa0e8-117">Удаленное состояние устройства автопилота Windows</span><span class="sxs-lookup"><span data-stu-id="aa0e8-117">Deleted windows autopilot device state</span></span>](intune-enrollment-deletedwindowsautopilotdevicestate.md)
- [<span data-ttu-id="aa0e8-118">Базовые профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-118">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="aa0e8-119">Профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-119">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="aa0e8-120">Профиль регистрации iOS DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-120">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="aa0e8-121">Профиль регистрации macOS DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-121">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="aa0e8-122">Параметр подключения DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-122">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="aa0e8-123">Тип маркера DEP</span><span class="sxs-lookup"><span data-stu-id="aa0e8-123">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="aa0e8-124">Источник обнаружения</span><span class="sxs-lookup"><span data-stu-id="aa0e8-124">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="aa0e8-125">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="aa0e8-125">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="aa0e8-126">Импортированное удостоверение устройства Apple</span><span class="sxs-lookup"><span data-stu-id="aa0e8-126">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="aa0e8-127">Результат импорта удостоверения устройства Apple</span><span class="sxs-lookup"><span data-stu-id="aa0e8-127">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="aa0e8-128">Импортированное удостоверение устройства</span><span class="sxs-lookup"><span data-stu-id="aa0e8-128">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="aa0e8-129">Результат импорта удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="aa0e8-129">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="aa0e8-130">Тип импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="aa0e8-130">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="aa0e8-131">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-131">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="aa0e8-132">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-132">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="aa0e8-133">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-133">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="aa0e8-134">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-134">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="aa0e8-135">Режим связывания с iTunes</span><span class="sxs-lookup"><span data-stu-id="aa0e8-135">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="aa0e8-136">Сертификат управления с отпечатком</span><span class="sxs-lookup"><span data-stu-id="aa0e8-136">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="aa0e8-137">Параметры запуска при первом включении компьютера</span><span class="sxs-lookup"><span data-stu-id="aa0e8-137">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="aa0e8-138">Платформа</span><span class="sxs-lookup"><span data-stu-id="aa0e8-138">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="aa0e8-139">Рекомендуемый предел регистрации</span><span class="sxs-lookup"><span data-stu-id="aa0e8-139">Suggested enrollment limit</span></span>](intune-enrollment-suggestedenrollmentlimit.md)
- [<span data-ttu-id="aa0e8-140">Назначение профиля Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="aa0e8-140">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="aa0e8-141">Состояние удаления устройства автопилота Windows</span><span class="sxs-lookup"><span data-stu-id="aa0e8-141">Windows autopilot device deletion state</span></span>](intune-enrollment-windowsautopilotdevicedeletionstate.md)
- [<span data-ttu-id="aa0e8-142">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-142">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="aa0e8-143">Тип устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-143">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="aa0e8-144">Полное состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-144">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="aa0e8-145">Состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-145">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="aa0e8-146">Параметры Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-146">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="aa0e8-147">Состояние синхронизации Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="aa0e8-147">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="aa0e8-148">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="aa0e8-148">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="aa0e8-149">Параметры экрана состояния регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="aa0e8-149">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="aa0e8-150">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="aa0e8-150">Windows user type</span></span>](intune-enrollment-windowsusertype.md)