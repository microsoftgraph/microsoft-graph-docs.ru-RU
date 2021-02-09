---
title: 'Общие ресурсы в Microsoft Intune : API Microsoft Graph'
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые поддерживают несколько процессов для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 07f408cfc4157dd4ad415a71b19367ce0ce6ddfa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156737"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="4860d-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4860d-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="4860d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4860d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4860d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4860d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4860d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4860d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4860d-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4860d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4860d-108">Эти конечные точки используются в нескольких API Microsoft Graph для рабочего процесса Intune.</span><span class="sxs-lookup"><span data-stu-id="4860d-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="4860d-109">Цель, цель и разрешения, необходимые для использования заданного ресурса, зависят от конкретного рабочего процесса и контекста вызова.</span><span class="sxs-lookup"><span data-stu-id="4860d-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="4860d-110">Кроме того, определенные методы, свойства и действия поддерживаются только для определенных процессов.</span><span class="sxs-lookup"><span data-stu-id="4860d-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="4860d-111">Между процессами Intune совместно работают следующие ресурсы Graph:</span><span class="sxs-lookup"><span data-stu-id="4860d-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="4860d-112">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="4860d-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="4860d-113">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="4860d-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="4860d-114">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="4860d-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="4860d-115">Корпоративный Android всегда имеет тип пакета VPN</span><span class="sxs-lookup"><span data-stu-id="4860d-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="4860d-116">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="4860d-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="4860d-117">Параметры назначения приложений управляемого магазина Android</span><span class="sxs-lookup"><span data-stu-id="4860d-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="4860d-118">Целевое хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="4860d-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="4860d-119">Хранилище сертификатов</span><span class="sxs-lookup"><span data-stu-id="4860d-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="4860d-120">Шкала срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="4860d-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="4860d-121">Действие на портале компании</span><span class="sxs-lookup"><span data-stu-id="4860d-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="4860d-122">Действия, заблокированные на портале компании</span><span class="sxs-lookup"><span data-stu-id="4860d-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="4860d-123">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="4860d-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="4860d-124">Цель назначения коллекции Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="4860d-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="4860d-125">Тип фильтра назначений для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="4860d-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="4860d-126">Источник назначения управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="4860d-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="4860d-127">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="4860d-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="4860d-128">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="4860d-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="4860d-129">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="4860d-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="4860d-130">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="4860d-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="4860d-131">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="4860d-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="4860d-132">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="4860d-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="4860d-133">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4860d-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="4860d-134">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="4860d-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="4860d-135">Параметры учетных данных, производных от управления устройствами</span><span class="sxs-lookup"><span data-stu-id="4860d-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="4860d-136">Отчеты службы управления устройствами</span><span class="sxs-lookup"><span data-stu-id="4860d-136">Device management reports</span></span>](intune-shared-devicemanagementreports.md)
- [<span data-ttu-id="4860d-137">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="4860d-137">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="4860d-138">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="4860d-138">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="4860d-139">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="4860d-139">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="4860d-140">Включение</span><span class="sxs-lookup"><span data-stu-id="4860d-140">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="4860d-141">Параметры доступности регистрации</span><span class="sxs-lookup"><span data-stu-id="4860d-141">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="4860d-142">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="4860d-142">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="4860d-143">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="4860d-143">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="4860d-144">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="4860d-144">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="4860d-145">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="4860d-145">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="4860d-146">Хэш-алгоритмы</span><span class="sxs-lookup"><span data-stu-id="4860d-146">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="4860d-147">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="4860d-147">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="4860d-148">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="4860d-148">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="4860d-149">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="4860d-149">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="4860d-150">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="4860d-150">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="4860d-151">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="4860d-151">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="4860d-152">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="4860d-152">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="4860d-153">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="4860d-153">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="4860d-154">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="4860d-154">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="4860d-155">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="4860d-155">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="4860d-156">Размер ключа</span><span class="sxs-lookup"><span data-stu-id="4860d-156">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="4860d-157">Параметр поставщика хранилища ключей</span><span class="sxs-lookup"><span data-stu-id="4860d-157">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="4860d-158">Использование ключей</span><span class="sxs-lookup"><span data-stu-id="4860d-158">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="4860d-159">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="4860d-159">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="4860d-160">Параметры назначения приложений для macOS LOB</span><span class="sxs-lookup"><span data-stu-id="4860d-160">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="4860d-161">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="4860d-161">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="4860d-162">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="4860d-162">Managed device</span></span>](intune-shared-manageddevice.md)
- [<span data-ttu-id="4860d-163">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="4860d-163">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="4860d-164">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="4860d-164">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="4860d-165">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="4860d-165">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="4860d-166">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="4860d-166">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="4860d-167">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="4860d-167">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="4860d-168">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="4860d-168">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="4860d-169">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="4860d-169">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="4860d-170">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="4860d-170">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="4860d-171">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="4860d-171">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="4860d-172">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="4860d-172">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="4860d-173">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="4860d-173">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="4860d-174">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="4860d-174">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="4860d-175">Report</span><span class="sxs-lookup"><span data-stu-id="4860d-175">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="4860d-176">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="4860d-176">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="4860d-177">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="4860d-177">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="4860d-178">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="4860d-178">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="4860d-179">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="4860d-179">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="4860d-180">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="4860d-180">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="4860d-181">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="4860d-181">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="4860d-182">Установка типа источника</span><span class="sxs-lookup"><span data-stu-id="4860d-182">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="4860d-183">Тип альтернативного имени субъекта</span><span class="sxs-lookup"><span data-stu-id="4860d-183">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="4860d-184">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="4860d-184">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="4860d-185">URI</span><span class="sxs-lookup"><span data-stu-id="4860d-185">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="4860d-186">Пользователь</span><span class="sxs-lookup"><span data-stu-id="4860d-186">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="4860d-187">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="4860d-187">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="4860d-188">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="4860d-188">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="4860d-189">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="4860d-189">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="4860d-190">Приоритет оптимизации доставки для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="4860d-190">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="4860d-191">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="4860d-191">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="4860d-192">Параметры перезапуска LOB-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="4860d-192">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="4860d-193">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="4860d-193">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="4860d-194">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="4860d-194">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="4860d-195">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="4860d-195">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="4860d-196">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="4860d-196">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="4860d-197">Состояние обновления Windows</span><span class="sxs-lookup"><span data-stu-id="4860d-197">Windows update state</span></span>](intune-shared-windowsupdatestate.md)