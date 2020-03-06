---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: db7746504a7bd31df99941ffc7bc85065eb5d56a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527479"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ca091-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ca091-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="ca091-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca091-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca091-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca091-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca091-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca091-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca091-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca091-108">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="ca091-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ca091-109">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="ca091-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ca091-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="ca091-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ca091-111">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="ca091-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="ca091-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="ca091-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="ca091-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="ca091-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ca091-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="ca091-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ca091-115">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="ca091-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="ca091-116">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="ca091-116">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="ca091-117">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="ca091-117">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="ca091-118">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="ca091-118">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ca091-119">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ca091-119">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="ca091-120">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ca091-120">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ca091-121">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="ca091-121">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ca091-122">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="ca091-122">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ca091-123">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="ca091-123">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="ca091-124">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="ca091-124">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="ca091-125">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="ca091-125">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="ca091-126">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="ca091-126">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="ca091-127">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="ca091-127">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ca091-128">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ca091-128">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="ca091-129">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ca091-129">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="ca091-130">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="ca091-130">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="ca091-131">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="ca091-131">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="ca091-132">Включение</span><span class="sxs-lookup"><span data-stu-id="ca091-132">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="ca091-133">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="ca091-133">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="ca091-134">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="ca091-134">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="ca091-135">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="ca091-135">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ca091-136">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="ca091-136">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ca091-137">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="ca091-137">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ca091-138">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="ca091-138">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="ca091-139">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="ca091-139">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="ca091-140">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="ca091-140">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="ca091-141">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="ca091-141">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="ca091-142">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ca091-142">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="ca091-143">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="ca091-143">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="ca091-144">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="ca091-144">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="ca091-145">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="ca091-145">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="ca091-146">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ca091-146">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="ca091-147">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ca091-147">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="ca091-148">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="ca091-148">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="ca091-149">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="ca091-149">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="ca091-150">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="ca091-150">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ca091-151">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ca091-151">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="ca091-152">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="ca091-152">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ca091-153">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="ca091-153">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="ca091-154">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ca091-154">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="ca091-155">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ca091-155">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="ca091-156">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="ca091-156">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="ca091-157">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="ca091-157">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="ca091-158">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="ca091-158">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="ca091-159">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ca091-159">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="ca091-160">Report</span><span class="sxs-lookup"><span data-stu-id="ca091-160">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ca091-161">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="ca091-161">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ca091-162">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="ca091-162">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="ca091-163">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="ca091-163">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="ca091-164">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="ca091-164">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="ca091-165">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="ca091-165">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="ca091-166">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="ca091-166">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ca091-167">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ca091-167">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="ca091-168">URI</span><span class="sxs-lookup"><span data-stu-id="ca091-168">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ca091-169">User</span><span class="sxs-lookup"><span data-stu-id="ca091-169">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ca091-170">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="ca091-170">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="ca091-171">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="ca091-171">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="ca091-172">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ca091-172">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="ca091-173">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ca091-173">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="ca091-174">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="ca091-174">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="ca091-175">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ca091-175">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="ca091-176">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="ca091-176">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ca091-177">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="ca091-177">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="ca091-178">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ca091-178">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="ca091-179">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="ca091-179">Windows update state</span></span>](intune-shared-windowsupdatestate.md)

