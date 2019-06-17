---
title: Регистрация корпоративных устройств с помощью Intune-API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые регистрируют устройства для организации клиента.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 053ae11623f01dc5287a143f3e9db8a6b12e4120
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978180"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="ebb99-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="ebb99-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="ebb99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebb99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebb99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebb99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebb99-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebb99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb99-107">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="ebb99-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="ebb99-108">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="ebb99-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="ebb99-109">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="ebb99-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="ebb99-110">Профиль Windows AutoPilot Deployment для Active Directory</span><span class="sxs-lookup"><span data-stu-id="ebb99-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ebb99-111">Профиль Windows AutoPilot Deployment для Azure AD</span><span class="sxs-lookup"><span data-stu-id="ebb99-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ebb99-112">Базовые профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="ebb99-113">Профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="ebb99-114">Профиль регистрации iOS DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="ebb99-115">Профиль регистрации macOS DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="ebb99-116">Параметр подключения DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="ebb99-117">Тип маркера DEP</span><span class="sxs-lookup"><span data-stu-id="ebb99-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="ebb99-118">Источник обнаружения</span><span class="sxs-lookup"><span data-stu-id="ebb99-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="ebb99-119">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="ebb99-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="ebb99-120">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="ebb99-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="ebb99-121">Импортированное удостоверение устройства Apple</span><span class="sxs-lookup"><span data-stu-id="ebb99-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="ebb99-122">Результат импорта удостоверения устройства Apple</span><span class="sxs-lookup"><span data-stu-id="ebb99-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="ebb99-123">Импортированное удостоверение устройства</span><span class="sxs-lookup"><span data-stu-id="ebb99-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="ebb99-124">Результат импорта удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="ebb99-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="ebb99-125">Тип импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="ebb99-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="ebb99-126">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ebb99-127">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="ebb99-128">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="ebb99-129">Загрузка импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="ebb99-130">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="ebb99-131">Режим связывания с iTunes</span><span class="sxs-lookup"><span data-stu-id="ebb99-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="ebb99-132">Сертификат управления с отпечатком</span><span class="sxs-lookup"><span data-stu-id="ebb99-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="ebb99-133">Параметры запуска при первом включении компьютера</span><span class="sxs-lookup"><span data-stu-id="ebb99-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="ebb99-134">Платформа</span><span class="sxs-lookup"><span data-stu-id="ebb99-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="ebb99-135">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="ebb99-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ebb99-136">Назначение профиля Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="ebb99-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="ebb99-137">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ebb99-138">Тип устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-138">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="ebb99-139">Полное состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-139">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="ebb99-140">Состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-140">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="ebb99-141">Параметры Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-141">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="ebb99-142">Состояние синхронизации Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ebb99-142">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="ebb99-143">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="ebb99-143">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="ebb99-144">Параметры экрана состояния регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="ebb99-144">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="ebb99-145">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="ebb99-145">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
