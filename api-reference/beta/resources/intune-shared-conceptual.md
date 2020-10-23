---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 0d5dd4150260ac61b9a49c231127107ea91fb758
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697198"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ef583-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ef583-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="ef583-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef583-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef583-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef583-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef583-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef583-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef583-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef583-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef583-108">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="ef583-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ef583-109">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="ef583-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ef583-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="ef583-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ef583-111">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="ef583-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="ef583-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="ef583-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="ef583-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="ef583-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ef583-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="ef583-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ef583-115">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="ef583-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="ef583-116">Параметры назначения приложений с управляемым хранилищем Android</span><span class="sxs-lookup"><span data-stu-id="ef583-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="ef583-117">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="ef583-117">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="ef583-118">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="ef583-118">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="ef583-119">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="ef583-119">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ef583-120">Тип фильтра назначения управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ef583-120">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="ef583-121">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ef583-121">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="ef583-122">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="ef583-122">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ef583-123">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="ef583-123">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ef583-124">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="ef583-124">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ef583-125">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="ef583-125">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="ef583-126">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="ef583-126">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="ef583-127">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="ef583-127">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="ef583-128">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="ef583-128">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="ef583-129">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="ef583-129">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ef583-130">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ef583-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="ef583-131">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="ef583-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="ef583-132">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="ef583-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="ef583-133">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="ef583-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="ef583-134">Включение</span><span class="sxs-lookup"><span data-stu-id="ef583-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="ef583-135">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="ef583-135">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="ef583-136">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="ef583-136">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="ef583-137">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="ef583-137">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ef583-138">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="ef583-138">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ef583-139">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="ef583-139">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ef583-140">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="ef583-140">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="ef583-141">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="ef583-141">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="ef583-142">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="ef583-142">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="ef583-143">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="ef583-143">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="ef583-144">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ef583-144">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="ef583-145">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="ef583-145">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="ef583-146">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="ef583-146">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="ef583-147">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="ef583-147">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="ef583-148">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ef583-148">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="ef583-149">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="ef583-149">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="ef583-150">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="ef583-150">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="ef583-151">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="ef583-151">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="ef583-152">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="ef583-152">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ef583-153">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ef583-153">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="ef583-154">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="ef583-154">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ef583-155">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="ef583-155">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="ef583-156">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ef583-156">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="ef583-157">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="ef583-157">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="ef583-158">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="ef583-158">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="ef583-159">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="ef583-159">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="ef583-160">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="ef583-160">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="ef583-161">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ef583-161">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="ef583-162">Report</span><span class="sxs-lookup"><span data-stu-id="ef583-162">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ef583-163">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="ef583-163">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ef583-164">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="ef583-164">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="ef583-165">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="ef583-165">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="ef583-166">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="ef583-166">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="ef583-167">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="ef583-167">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="ef583-168">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="ef583-168">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ef583-169">Настройка типа источника</span><span class="sxs-lookup"><span data-stu-id="ef583-169">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="ef583-170">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ef583-170">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="ef583-171">URI</span><span class="sxs-lookup"><span data-stu-id="ef583-171">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ef583-172">Пользователь</span><span class="sxs-lookup"><span data-stu-id="ef583-172">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ef583-173">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="ef583-173">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="ef583-174">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="ef583-174">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="ef583-175">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ef583-175">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="ef583-176">Приоритет оптимизации доставки бизнес-приложений Win32</span><span class="sxs-lookup"><span data-stu-id="ef583-176">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="ef583-177">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ef583-177">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="ef583-178">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="ef583-178">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="ef583-179">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ef583-179">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="ef583-180">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="ef583-180">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ef583-181">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="ef583-181">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="ef583-182">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="ef583-182">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="ef583-183">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="ef583-183">Windows update state</span></span>](intune-shared-windowsupdatestate.md)