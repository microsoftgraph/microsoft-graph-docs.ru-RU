---
title: Регистрация корпоративных устройств с помощью Intune-API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые регистрируют устройства для организации клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5611e7819756803bceb079d9ef1d324ec39a7d0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179202"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="50dbf-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="50dbf-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="50dbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50dbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50dbf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50dbf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50dbf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50dbf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50dbf-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50dbf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50dbf-108">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="50dbf-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="50dbf-109">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="50dbf-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="50dbf-110">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="50dbf-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="50dbf-111">Профиль Windows AutoPilot Deployment для Active Directory</span><span class="sxs-lookup"><span data-stu-id="50dbf-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="50dbf-112">Назначение профилей регистрации Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="50dbf-113">Тип регистрации типа владельца Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="50dbf-114">Профиль регистрации, инициированный пользователем Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="50dbf-115">Тип регистрации, инициированный пользователем Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="50dbf-116">Профиль Windows AutoPilot Deployment для Azure AD</span><span class="sxs-lookup"><span data-stu-id="50dbf-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="50dbf-117">Базовые профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-117">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="50dbf-118">Профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-118">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="50dbf-119">Профиль регистрации iOS DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-119">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="50dbf-120">Профиль регистрации macOS DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-120">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="50dbf-121">Параметр подключения DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-121">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="50dbf-122">Тип маркера DEP</span><span class="sxs-lookup"><span data-stu-id="50dbf-122">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="50dbf-123">Источник обнаружения</span><span class="sxs-lookup"><span data-stu-id="50dbf-123">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="50dbf-124">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="50dbf-124">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="50dbf-125">Импортированное удостоверение устройства Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-125">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="50dbf-126">Результат импорта удостоверения устройства Apple</span><span class="sxs-lookup"><span data-stu-id="50dbf-126">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="50dbf-127">Импортированное удостоверение устройства</span><span class="sxs-lookup"><span data-stu-id="50dbf-127">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="50dbf-128">Результат импорта удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="50dbf-128">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="50dbf-129">Тип импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="50dbf-129">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="50dbf-130">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-130">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="50dbf-131">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-131">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="50dbf-132">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-132">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="50dbf-133">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-133">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="50dbf-134">Режим связывания с iTunes</span><span class="sxs-lookup"><span data-stu-id="50dbf-134">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="50dbf-135">Сертификат управления с отпечатком</span><span class="sxs-lookup"><span data-stu-id="50dbf-135">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="50dbf-136">Параметры запуска при первом включении компьютера</span><span class="sxs-lookup"><span data-stu-id="50dbf-136">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="50dbf-137">Платформа</span><span class="sxs-lookup"><span data-stu-id="50dbf-137">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="50dbf-138">Назначение профиля Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="50dbf-138">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="50dbf-139">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-139">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="50dbf-140">Тип устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-140">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="50dbf-141">Полное состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-141">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="50dbf-142">Состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-142">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="50dbf-143">Параметры Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-143">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="50dbf-144">Состояние синхронизации Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="50dbf-144">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="50dbf-145">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="50dbf-145">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="50dbf-146">Параметры экрана состояния регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="50dbf-146">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="50dbf-147">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="50dbf-147">Windows user type</span></span>](intune-enrollment-windowsusertype.md)