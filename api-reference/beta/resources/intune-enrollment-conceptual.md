---
title: Регистрация корпоративных устройств с помощью Intune-API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые регистрируют устройства для организации клиента.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 506f85ae59330757f4c6f12cf80795c6678b125e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366373"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="62ee2-103">Регистрация корпоративных устройств с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="62ee2-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="62ee2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62ee2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62ee2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ee2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62ee2-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62ee2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62ee2-107">Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство.</span><span class="sxs-lookup"><span data-stu-id="62ee2-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="62ee2-108">Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="62ee2-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="62ee2-109">Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="62ee2-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="62ee2-110">Профиль Windows AutoPilot Deployment для Active Directory</span><span class="sxs-lookup"><span data-stu-id="62ee2-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="62ee2-111">Профиль Windows AutoPilot Deployment для Azure AD</span><span class="sxs-lookup"><span data-stu-id="62ee2-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="62ee2-112">Базовые профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="62ee2-113">Профиль регистрации DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="62ee2-114">Профиль регистрации iOS DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="62ee2-115">Профиль регистрации macOS DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="62ee2-116">Параметр подключения DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="62ee2-117">Тип маркера DEP</span><span class="sxs-lookup"><span data-stu-id="62ee2-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="62ee2-118">Источник обнаружения</span><span class="sxs-lookup"><span data-stu-id="62ee2-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="62ee2-119">Профиль регистрации</span><span class="sxs-lookup"><span data-stu-id="62ee2-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="62ee2-120">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="62ee2-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="62ee2-121">Импортированное удостоверение устройства Apple</span><span class="sxs-lookup"><span data-stu-id="62ee2-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="62ee2-122">Результат импорта удостоверения устройства Apple</span><span class="sxs-lookup"><span data-stu-id="62ee2-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="62ee2-123">Импортированное удостоверение устройства</span><span class="sxs-lookup"><span data-stu-id="62ee2-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="62ee2-124">Результат импорта удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="62ee2-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="62ee2-125">Тип импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="62ee2-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="62ee2-126">Импортированное удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="62ee2-127">Состояние импорта удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="62ee2-128">Состояние импортированного удостоверения устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="62ee2-129">Статус загрузки импортированного удостоверения устройства Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-129">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="62ee2-130">Режим связывания с iTunes</span><span class="sxs-lookup"><span data-stu-id="62ee2-130">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="62ee2-131">Сертификат управления с отпечатком</span><span class="sxs-lookup"><span data-stu-id="62ee2-131">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="62ee2-132">Параметры запуска при первом включении компьютера</span><span class="sxs-lookup"><span data-stu-id="62ee2-132">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="62ee2-133">Платформа</span><span class="sxs-lookup"><span data-stu-id="62ee2-133">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="62ee2-134">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="62ee2-134">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="62ee2-135">Назначение профиля Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="62ee2-135">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="62ee2-136">Удостоверение устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-136">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="62ee2-137">Тип устройства с Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-137">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="62ee2-138">Полное состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="62ee2-139">Состояние назначения профиля Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="62ee2-140">Параметры Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="62ee2-141">Состояние синхронизации Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="62ee2-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="62ee2-142">Тип использования устройства Windows</span><span class="sxs-lookup"><span data-stu-id="62ee2-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="62ee2-143">Параметры экрана состояния регистрации Windows</span><span class="sxs-lookup"><span data-stu-id="62ee2-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="62ee2-144">Тип пользователя Windows</span><span class="sxs-lookup"><span data-stu-id="62ee2-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
