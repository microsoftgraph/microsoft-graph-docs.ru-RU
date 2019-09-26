---
title: Регистрация корпоративных устройств с помощью Intune-API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые регистрируют устройства для организации клиента.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5655bd1733c2383bac562f700be5abc1c57bf43b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196611"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="dbecf-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="dbecf-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="dbecf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbecf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbecf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbecf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbecf-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbecf-107">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="dbecf-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="dbecf-108">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="dbecf-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="dbecf-109">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="dbecf-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="dbecf-110">Профиль Windows AutoPilot Deployment для Active Directory</span><span class="sxs-lookup"><span data-stu-id="dbecf-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="dbecf-111">Назначение профилей регистрации Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-111">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="dbecf-112">Тип регистрации типа владельца Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-112">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="dbecf-113">Профиль регистрации, инициированный пользователем Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-113">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="dbecf-114">Тип регистрации, инициированный пользователем Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-114">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="dbecf-115">Профиль Windows AutoPilot Deployment для Azure AD</span><span class="sxs-lookup"><span data-stu-id="dbecf-115">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="dbecf-116">Базовые профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-116">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="dbecf-117">Профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-117">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="dbecf-118">Профиль регистрации iOS DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-118">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="dbecf-119">Профиль регистрации macOS DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-119">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="dbecf-120">Параметр подключения DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-120">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="dbecf-121">Тип маркера DEP</span><span class="sxs-lookup"><span data-stu-id="dbecf-121">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="dbecf-122">Источник обнаружения</span><span class="sxs-lookup"><span data-stu-id="dbecf-122">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="dbecf-123">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="dbecf-123">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="dbecf-124">Импортированное удостоверение устройства Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-124">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="dbecf-125">Результат импорта удостоверения устройства Apple</span><span class="sxs-lookup"><span data-stu-id="dbecf-125">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="dbecf-126">Импортированное удостоверение устройства</span><span class="sxs-lookup"><span data-stu-id="dbecf-126">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="dbecf-127">Результат импорта удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="dbecf-127">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="dbecf-128">Тип импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="dbecf-128">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="dbecf-129">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-129">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="dbecf-130">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-130">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="dbecf-131">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-131">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="dbecf-132">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-132">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="dbecf-133">Режим связывания с iTunes</span><span class="sxs-lookup"><span data-stu-id="dbecf-133">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="dbecf-134">Сертификат управления с отпечатком</span><span class="sxs-lookup"><span data-stu-id="dbecf-134">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="dbecf-135">Параметры запуска при первом включении компьютера</span><span class="sxs-lookup"><span data-stu-id="dbecf-135">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="dbecf-136">Платформа</span><span class="sxs-lookup"><span data-stu-id="dbecf-136">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="dbecf-137">Назначение профиля Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="dbecf-137">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="dbecf-138">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-138">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="dbecf-139">Тип устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-139">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="dbecf-140">Полное состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-140">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="dbecf-141">Состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-141">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="dbecf-142">Параметры Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-142">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="dbecf-143">Состояние синхронизации Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="dbecf-143">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="dbecf-144">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="dbecf-144">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="dbecf-145">Параметры экрана состояния регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="dbecf-145">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="dbecf-146">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="dbecf-146">Windows user type</span></span>](intune-enrollment-windowsusertype.md)

