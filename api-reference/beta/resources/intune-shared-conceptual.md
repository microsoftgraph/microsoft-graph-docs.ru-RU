---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 2d138f4c92999477054e8fe154c426fd18181037
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178096"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="64467-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="64467-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="64467-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64467-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64467-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64467-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64467-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64467-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64467-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64467-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64467-108">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="64467-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="64467-109">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="64467-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="64467-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="64467-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="64467-111">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="64467-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="64467-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="64467-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="64467-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="64467-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="64467-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="64467-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="64467-115">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="64467-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="64467-116">Параметры назначения приложений с управляемым хранилищем Android</span><span class="sxs-lookup"><span data-stu-id="64467-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="64467-117">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="64467-117">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="64467-118">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="64467-118">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="64467-119">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="64467-119">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="64467-120">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="64467-120">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="64467-121">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="64467-121">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="64467-122">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="64467-122">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="64467-123">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="64467-123">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="64467-124">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="64467-124">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="64467-125">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="64467-125">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="64467-126">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="64467-126">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="64467-127">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="64467-127">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="64467-128">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="64467-128">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="64467-129">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="64467-129">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="64467-130">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="64467-130">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="64467-131">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="64467-131">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="64467-132">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="64467-132">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="64467-133">Включение</span><span class="sxs-lookup"><span data-stu-id="64467-133">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="64467-134">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="64467-134">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="64467-135">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="64467-135">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="64467-136">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="64467-136">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="64467-137">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="64467-137">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="64467-138">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="64467-138">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="64467-139">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="64467-139">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="64467-140">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="64467-140">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="64467-141">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="64467-141">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="64467-142">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="64467-142">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="64467-143">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="64467-143">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="64467-144">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="64467-144">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="64467-145">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="64467-145">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="64467-146">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="64467-146">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="64467-147">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="64467-147">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="64467-148">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="64467-148">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="64467-149">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="64467-149">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="64467-150">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="64467-150">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="64467-151">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="64467-151">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="64467-152">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="64467-152">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="64467-153">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="64467-153">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="64467-154">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="64467-154">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="64467-155">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="64467-155">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="64467-156">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="64467-156">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="64467-157">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="64467-157">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="64467-158">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="64467-158">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="64467-159">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="64467-159">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="64467-160">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="64467-160">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="64467-161">Report</span><span class="sxs-lookup"><span data-stu-id="64467-161">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="64467-162">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="64467-162">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="64467-163">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="64467-163">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="64467-164">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="64467-164">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="64467-165">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="64467-165">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="64467-166">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="64467-166">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="64467-167">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="64467-167">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="64467-168">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="64467-168">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="64467-169">URI</span><span class="sxs-lookup"><span data-stu-id="64467-169">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="64467-170">Пользователь</span><span class="sxs-lookup"><span data-stu-id="64467-170">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="64467-171">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="64467-171">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="64467-172">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="64467-172">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="64467-173">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="64467-173">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="64467-174">Приоритет оптимизации доставки бизнес-приложений Win32</span><span class="sxs-lookup"><span data-stu-id="64467-174">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="64467-175">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="64467-175">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="64467-176">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="64467-176">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="64467-177">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="64467-177">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="64467-178">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="64467-178">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="64467-179">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="64467-179">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="64467-180">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="64467-180">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="64467-181">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="64467-181">Windows update state</span></span>](intune-shared-windowsupdatestate.md)