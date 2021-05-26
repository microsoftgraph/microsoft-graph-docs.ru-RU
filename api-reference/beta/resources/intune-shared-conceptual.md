---
title: Общие ресурсы в Microsoft Intune - API Graph Microsoft
description: Перечислены API Graph Microsoft для конечных точек Intune (REST), которые поддерживают несколько процессов для организации-клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 77500484aaafd5d9101e66789966b4861b61e511
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664904"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="bea7b-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bea7b-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="bea7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bea7b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bea7b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bea7b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea7b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bea7b-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bea7b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea7b-108">Эти конечные точки используются в нескольких API Graph Microsoft для рабочего процесса Intune.</span><span class="sxs-lookup"><span data-stu-id="bea7b-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="bea7b-109">Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.</span><span class="sxs-lookup"><span data-stu-id="bea7b-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="bea7b-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.</span><span class="sxs-lookup"><span data-stu-id="bea7b-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="bea7b-111">Между Graph intune общие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="bea7b-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="bea7b-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="bea7b-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="bea7b-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="bea7b-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="bea7b-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="bea7b-115">Android-предприятие всегда на типе пакета VPN</span><span class="sxs-lookup"><span data-stu-id="bea7b-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="bea7b-116">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="bea7b-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="bea7b-117">Параметры назначения приложений для управляемого магазина Android</span><span class="sxs-lookup"><span data-stu-id="bea7b-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="bea7b-118">Целевое хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="bea7b-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="bea7b-119">Хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="bea7b-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="bea7b-120">Шкала срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="bea7b-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="bea7b-121">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="bea7b-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="bea7b-122">Портал компании заблокировал действие</span><span class="sxs-lookup"><span data-stu-id="bea7b-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="bea7b-123">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="bea7b-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="bea7b-124">Цель назначения коллекции диспетчера конфигурации</span><span class="sxs-lookup"><span data-stu-id="bea7b-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="bea7b-125">Тип фильтра назначения для устройств и приложений</span><span class="sxs-lookup"><span data-stu-id="bea7b-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="bea7b-126">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="bea7b-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="bea7b-127">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="bea7b-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="bea7b-128">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="bea7b-129">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="bea7b-130">Политика соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="bea7b-131">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="bea7b-132">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="bea7b-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="bea7b-133">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="bea7b-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="bea7b-134">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="bea7b-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="bea7b-135">Параметры учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="bea7b-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="bea7b-136">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="bea7b-136">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="bea7b-137">Включение</span><span class="sxs-lookup"><span data-stu-id="bea7b-137">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="bea7b-138">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="bea7b-138">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="bea7b-139">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="bea7b-139">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="bea7b-140">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="bea7b-140">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="bea7b-141">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="bea7b-141">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="bea7b-142">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="bea7b-142">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="bea7b-143">Хэш-алгоритмы</span><span class="sxs-lookup"><span data-stu-id="bea7b-143">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="bea7b-144">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="bea7b-144">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="bea7b-145">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="bea7b-145">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="bea7b-146">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="bea7b-146">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="bea7b-147">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="bea7b-147">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="bea7b-148">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="bea7b-148">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="bea7b-149">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="bea7b-149">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="bea7b-150">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="bea7b-150">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="bea7b-151">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="bea7b-151">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="bea7b-152">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="bea7b-152">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="bea7b-153">Размер ключа</span><span class="sxs-lookup"><span data-stu-id="bea7b-153">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="bea7b-154">Параметр поставщика хранилища ключей</span><span class="sxs-lookup"><span data-stu-id="bea7b-154">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="bea7b-155">Использование ключей</span><span class="sxs-lookup"><span data-stu-id="bea7b-155">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="bea7b-156">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="bea7b-156">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="bea7b-157">Параметры назначения приложений macOS LOB</span><span class="sxs-lookup"><span data-stu-id="bea7b-157">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="bea7b-158">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="bea7b-158">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="bea7b-159">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="bea7b-159">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="bea7b-160">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="bea7b-160">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="bea7b-161">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="bea7b-161">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="bea7b-162">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="bea7b-162">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="bea7b-163">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="bea7b-163">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="bea7b-164">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="bea7b-164">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="bea7b-165">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="bea7b-165">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="bea7b-166">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="bea7b-166">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="bea7b-167">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="bea7b-167">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="bea7b-168">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="bea7b-168">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="bea7b-169">Отчет</span><span class="sxs-lookup"><span data-stu-id="bea7b-169">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="bea7b-170">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="bea7b-170">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="bea7b-171">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="bea7b-171">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="bea7b-172">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="bea7b-172">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="bea7b-173">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="bea7b-173">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="bea7b-174">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="bea7b-174">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="bea7b-175">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="bea7b-175">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="bea7b-176">Настройка типа источника</span><span class="sxs-lookup"><span data-stu-id="bea7b-176">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="bea7b-177">Тип альтернативного имени субъекта</span><span class="sxs-lookup"><span data-stu-id="bea7b-177">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="bea7b-178">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="bea7b-178">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="bea7b-179">URI</span><span class="sxs-lookup"><span data-stu-id="bea7b-179">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="bea7b-180">Пользователь</span><span class="sxs-lookup"><span data-stu-id="bea7b-180">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="bea7b-181">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="bea7b-181">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="bea7b-182">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="bea7b-182">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="bea7b-183">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="bea7b-183">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="bea7b-184">Приоритет оптимизации доставки приложений Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="bea7b-184">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="bea7b-185">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="bea7b-185">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="bea7b-186">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="bea7b-186">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="bea7b-187">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="bea7b-187">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="bea7b-188">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="bea7b-188">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="bea7b-189">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="bea7b-189">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="bea7b-190">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="bea7b-190">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="bea7b-191">Windows состояние обновления</span><span class="sxs-lookup"><span data-stu-id="bea7b-191">Windows update state</span></span>](intune-shared-windowsupdatestate.md)