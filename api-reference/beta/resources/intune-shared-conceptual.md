---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 06be7eefad204f0cef73d8c0d16d70159f9142db
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793761"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ea4ed-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ea4ed-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="ea4ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea4ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea4ed-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea4ed-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea4ed-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea4ed-108">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ea4ed-109">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ea4ed-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ea4ed-111">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="ea4ed-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="ea4ed-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="ea4ed-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="ea4ed-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="ea4ed-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ea4ed-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="ea4ed-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ea4ed-115">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="ea4ed-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="ea4ed-116">Параметры назначения приложений с управляемым хранилищем Android</span><span class="sxs-lookup"><span data-stu-id="ea4ed-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-117">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="ea4ed-117">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="ea4ed-118">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="ea4ed-118">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="ea4ed-119">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="ea4ed-119">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ea4ed-120">Тип фильтра назначения управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ea4ed-120">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="ea4ed-121">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ea4ed-121">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="ea4ed-122">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ea4ed-122">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ea4ed-123">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="ea4ed-123">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ea4ed-124">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="ea4ed-124">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ea4ed-125">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="ea4ed-125">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="ea4ed-126">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="ea4ed-126">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="ea4ed-127">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="ea4ed-127">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="ea4ed-128">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="ea4ed-128">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="ea4ed-129">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="ea4ed-129">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ea4ed-130">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ea4ed-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="ea4ed-131">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ea4ed-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="ea4ed-132">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="ea4ed-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="ea4ed-133">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="ea4ed-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="ea4ed-134">Включение</span><span class="sxs-lookup"><span data-stu-id="ea4ed-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="ea4ed-135">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="ea4ed-135">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="ea4ed-136">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="ea4ed-136">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="ea4ed-137">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-137">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ea4ed-138">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="ea4ed-138">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ea4ed-139">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="ea4ed-139">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ea4ed-140">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="ea4ed-140">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-141">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="ea4ed-141">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="ea4ed-142">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="ea4ed-142">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="ea4ed-143">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="ea4ed-143">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-144">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ea4ed-144">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-145">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="ea4ed-145">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="ea4ed-146">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="ea4ed-146">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="ea4ed-147">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="ea4ed-147">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="ea4ed-148">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ea4ed-148">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="ea4ed-149">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ea4ed-149">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-150">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="ea4ed-150">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="ea4ed-151">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="ea4ed-151">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="ea4ed-152">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="ea4ed-152">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ea4ed-153">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ea4ed-153">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-154">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="ea4ed-154">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ea4ed-155">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="ea4ed-155">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="ea4ed-156">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-156">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-157">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-157">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="ea4ed-158">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="ea4ed-158">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="ea4ed-159">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="ea4ed-159">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="ea4ed-160">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="ea4ed-160">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="ea4ed-161">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ea4ed-161">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="ea4ed-162">Report</span><span class="sxs-lookup"><span data-stu-id="ea4ed-162">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ea4ed-163">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="ea4ed-163">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ea4ed-164">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-164">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="ea4ed-165">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="ea4ed-165">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="ea4ed-166">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="ea4ed-166">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="ea4ed-167">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-167">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="ea4ed-168">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="ea4ed-168">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ea4ed-169">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ea4ed-169">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="ea4ed-170">URI</span><span class="sxs-lookup"><span data-stu-id="ea4ed-170">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ea4ed-171">User</span><span class="sxs-lookup"><span data-stu-id="ea4ed-171">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ea4ed-172">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="ea4ed-172">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="ea4ed-173">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="ea4ed-173">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="ea4ed-174">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ea4ed-174">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-175">Приоритет оптимизации доставки бизнес-приложений Win32</span><span class="sxs-lookup"><span data-stu-id="ea4ed-175">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="ea4ed-176">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ea4ed-176">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="ea4ed-177">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="ea4ed-177">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="ea4ed-178">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ea4ed-178">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-179">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="ea4ed-179">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ea4ed-180">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="ea4ed-180">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="ea4ed-181">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ea4ed-181">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="ea4ed-182">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="ea4ed-182">Windows update state</span></span>](intune-shared-windowsupdatestate.md)