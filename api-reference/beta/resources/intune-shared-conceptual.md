---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 9a5a6ee1a9111f85d041821e8e5917c0b007698d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160342"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="62ce8-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62ce8-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="62ce8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62ce8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62ce8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ce8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62ce8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62ce8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62ce8-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="62ce8-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="62ce8-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="62ce8-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="62ce8-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="62ce8-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="62ce8-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="62ce8-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="62ce8-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="62ce8-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="62ce8-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="62ce8-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="62ce8-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="62ce8-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="62ce8-114">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="62ce8-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="62ce8-115">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="62ce8-115">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="62ce8-116">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="62ce8-116">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="62ce8-117">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="62ce8-117">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="62ce8-118">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="62ce8-118">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="62ce8-119">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="62ce8-119">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="62ce8-120">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="62ce8-120">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="62ce8-121">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="62ce8-121">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="62ce8-122">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="62ce8-122">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="62ce8-123">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="62ce8-123">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="62ce8-124">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="62ce8-124">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="62ce8-125">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="62ce8-125">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="62ce8-126">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="62ce8-126">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="62ce8-127">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="62ce8-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="62ce8-128">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="62ce8-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="62ce8-129">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="62ce8-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="62ce8-130">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="62ce8-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="62ce8-131">Включение</span><span class="sxs-lookup"><span data-stu-id="62ce8-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="62ce8-132">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="62ce8-132">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="62ce8-133">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="62ce8-133">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="62ce8-134">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="62ce8-134">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="62ce8-135">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="62ce8-135">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="62ce8-136">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="62ce8-136">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="62ce8-137">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="62ce8-137">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="62ce8-138">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="62ce8-138">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="62ce8-139">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="62ce8-139">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="62ce8-140">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="62ce8-140">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="62ce8-141">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="62ce8-141">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="62ce8-142">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="62ce8-142">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="62ce8-143">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="62ce8-143">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="62ce8-144">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="62ce8-144">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="62ce8-145">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="62ce8-145">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="62ce8-146">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="62ce8-146">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="62ce8-147">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="62ce8-147">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="62ce8-148">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="62ce8-148">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="62ce8-149">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="62ce8-149">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="62ce8-150">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="62ce8-150">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="62ce8-151">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="62ce8-151">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="62ce8-152">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="62ce8-152">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="62ce8-153">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="62ce8-153">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="62ce8-154">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="62ce8-154">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="62ce8-155">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="62ce8-155">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="62ce8-156">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="62ce8-156">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="62ce8-157">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="62ce8-157">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="62ce8-158">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="62ce8-158">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="62ce8-159">Report</span><span class="sxs-lookup"><span data-stu-id="62ce8-159">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="62ce8-160">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="62ce8-160">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="62ce8-161">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="62ce8-161">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="62ce8-162">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="62ce8-162">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="62ce8-163">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="62ce8-163">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="62ce8-164">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="62ce8-164">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="62ce8-165">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="62ce8-165">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="62ce8-166">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="62ce8-166">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="62ce8-167">URI</span><span class="sxs-lookup"><span data-stu-id="62ce8-167">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="62ce8-168">User</span><span class="sxs-lookup"><span data-stu-id="62ce8-168">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="62ce8-169">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="62ce8-169">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="62ce8-170">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="62ce8-170">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="62ce8-171">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="62ce8-171">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="62ce8-172">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="62ce8-172">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="62ce8-173">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="62ce8-173">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="62ce8-174">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="62ce8-174">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="62ce8-175">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="62ce8-175">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="62ce8-176">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="62ce8-176">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="62ce8-177">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="62ce8-177">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="62ce8-178">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="62ce8-178">Windows update state</span></span>](intune-shared-windowsupdatestate.md)

