---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечислены API Microsoft Graph для конечных точек Intune (REST), которые поддерживают несколько процессов для организации-клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 6c0b11847ff5ec0f4431a20e4ffa197ddd21dbcf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440180"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="5f538-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5f538-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="5f538-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f538-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f538-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f538-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f538-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f538-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f538-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f538-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f538-108">Эти конечные точки используются в нескольких API Microsoft Graph для процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="5f538-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="5f538-109">Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.</span><span class="sxs-lookup"><span data-stu-id="5f538-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="5f538-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.</span><span class="sxs-lookup"><span data-stu-id="5f538-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="5f538-111">Между рабочего процессами Intune делятся следующие ресурсы Graph:</span><span class="sxs-lookup"><span data-stu-id="5f538-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="5f538-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="5f538-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="5f538-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="5f538-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="5f538-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="5f538-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="5f538-115">Android-предприятие всегда на типе пакета VPN</span><span class="sxs-lookup"><span data-stu-id="5f538-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="5f538-116">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="5f538-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="5f538-117">Параметры назначения приложений для управляемого магазина Android</span><span class="sxs-lookup"><span data-stu-id="5f538-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="5f538-118">Целевое хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="5f538-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="5f538-119">Хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="5f538-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="5f538-120">Шкала срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="5f538-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="5f538-121">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="5f538-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="5f538-122">Портал компании заблокировал действие</span><span class="sxs-lookup"><span data-stu-id="5f538-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="5f538-123">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="5f538-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="5f538-124">Цель назначения коллекции диспетчера конфигурации</span><span class="sxs-lookup"><span data-stu-id="5f538-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="5f538-125">Тип фильтра назначения для устройств и приложений</span><span class="sxs-lookup"><span data-stu-id="5f538-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="5f538-126">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5f538-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="5f538-127">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5f538-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="5f538-128">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="5f538-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="5f538-129">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="5f538-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="5f538-130">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="5f538-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="5f538-131">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="5f538-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="5f538-132">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="5f538-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="5f538-133">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="5f538-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="5f538-134">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="5f538-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="5f538-135">Параметры учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="5f538-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="5f538-136">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="5f538-136">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="5f538-137">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="5f538-137">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="5f538-138">Включение</span><span class="sxs-lookup"><span data-stu-id="5f538-138">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="5f538-139">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="5f538-139">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="5f538-140">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="5f538-140">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="5f538-141">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="5f538-141">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="5f538-142">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="5f538-142">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="5f538-143">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="5f538-143">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="5f538-144">Хэш-алгоритмы</span><span class="sxs-lookup"><span data-stu-id="5f538-144">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="5f538-145">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="5f538-145">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="5f538-146">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="5f538-146">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="5f538-147">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="5f538-147">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="5f538-148">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="5f538-148">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="5f538-149">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="5f538-149">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="5f538-150">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="5f538-150">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="5f538-151">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="5f538-151">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="5f538-152">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="5f538-152">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="5f538-153">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="5f538-153">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="5f538-154">Размер ключа</span><span class="sxs-lookup"><span data-stu-id="5f538-154">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="5f538-155">Параметр поставщика хранилища ключей</span><span class="sxs-lookup"><span data-stu-id="5f538-155">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="5f538-156">Использование ключей</span><span class="sxs-lookup"><span data-stu-id="5f538-156">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="5f538-157">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="5f538-157">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="5f538-158">Параметры назначения приложений macOS LOB</span><span class="sxs-lookup"><span data-stu-id="5f538-158">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="5f538-159">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="5f538-159">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="5f538-160">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="5f538-160">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="5f538-161">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="5f538-161">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="5f538-162">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="5f538-162">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="5f538-163">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="5f538-163">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="5f538-164">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="5f538-164">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="5f538-165">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="5f538-165">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="5f538-166">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="5f538-166">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="5f538-167">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="5f538-167">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="5f538-168">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="5f538-168">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="5f538-169">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="5f538-169">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="5f538-170">Report</span><span class="sxs-lookup"><span data-stu-id="5f538-170">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="5f538-171">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="5f538-171">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="5f538-172">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="5f538-172">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="5f538-173">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="5f538-173">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="5f538-174">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="5f538-174">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="5f538-175">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="5f538-175">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="5f538-176">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="5f538-176">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="5f538-177">Настройка типа источника</span><span class="sxs-lookup"><span data-stu-id="5f538-177">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="5f538-178">Тип альтернативного имени субъекта</span><span class="sxs-lookup"><span data-stu-id="5f538-178">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="5f538-179">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="5f538-179">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="5f538-180">URI</span><span class="sxs-lookup"><span data-stu-id="5f538-180">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="5f538-181">Пользователь</span><span class="sxs-lookup"><span data-stu-id="5f538-181">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="5f538-182">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="5f538-182">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="5f538-183">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="5f538-183">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="5f538-184">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5f538-184">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="5f538-185">Приоритет оптимизации доставки приложений Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="5f538-185">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="5f538-186">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5f538-186">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="5f538-187">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="5f538-187">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="5f538-188">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="5f538-188">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="5f538-189">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="5f538-189">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="5f538-190">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="5f538-190">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="5f538-191">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="5f538-191">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="5f538-192">Состояние обновления Windows</span><span class="sxs-lookup"><span data-stu-id="5f538-192">Windows update state</span></span>](intune-shared-windowsupdatestate.md)