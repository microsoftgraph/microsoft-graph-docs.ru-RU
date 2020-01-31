---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: e1b613dc9140e597dc9eb0c74448f227cf940ba5
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636828"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="d2d87-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d2d87-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="d2d87-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2d87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2d87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2d87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d87-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="d2d87-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="d2d87-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="d2d87-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="d2d87-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="d2d87-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="d2d87-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="d2d87-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="d2d87-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="d2d87-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="d2d87-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="d2d87-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="d2d87-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="d2d87-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d2d87-114">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="d2d87-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="d2d87-115">Тип вращения пароля восстановления BitLocker</span><span class="sxs-lookup"><span data-stu-id="d2d87-115">BitLocker recovery password rotation type</span></span>](intune-shared-bitlockerrecoverypasswordrotationtype.md)
- [<span data-ttu-id="d2d87-116">Действие портала компании</span><span class="sxs-lookup"><span data-stu-id="d2d87-116">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="d2d87-117">Действие блокирования портала компании</span><span class="sxs-lookup"><span data-stu-id="d2d87-117">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="d2d87-118">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="d2d87-118">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="d2d87-119">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="d2d87-119">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="d2d87-120">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="d2d87-120">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d2d87-121">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="d2d87-121">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="d2d87-122">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="d2d87-122">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="d2d87-123">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="d2d87-123">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="d2d87-124">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="d2d87-124">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="d2d87-125">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d2d87-125">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="d2d87-126">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="d2d87-126">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="d2d87-127">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="d2d87-127">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="d2d87-128">Производный поставщик учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="d2d87-128">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="d2d87-129">Тип уведомления о получении учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="d2d87-129">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="d2d87-130">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="d2d87-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="d2d87-131">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="d2d87-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="d2d87-132">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="d2d87-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="d2d87-133">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="d2d87-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="d2d87-134">Включение</span><span class="sxs-lookup"><span data-stu-id="d2d87-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="d2d87-135">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="d2d87-135">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="d2d87-136">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="d2d87-136">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d2d87-137">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="d2d87-137">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="d2d87-138">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="d2d87-138">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="d2d87-139">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="d2d87-139">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="d2d87-140">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="d2d87-140">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="d2d87-141">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="d2d87-141">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="d2d87-142">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="d2d87-142">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="d2d87-143">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="d2d87-143">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="d2d87-144">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="d2d87-144">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="d2d87-145">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="d2d87-145">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="d2d87-146">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="d2d87-146">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="d2d87-147">Ключевая логическая переменная значения</span><span class="sxs-lookup"><span data-stu-id="d2d87-147">Key boolean value pair</span></span>](intune-shared-keybooleanvaluepair.md)
- [<span data-ttu-id="d2d87-148">Ключевое целое значение</span><span class="sxs-lookup"><span data-stu-id="d2d87-148">Key integer value pair</span></span>](intune-shared-keyintegervaluepair.md)
- [<span data-ttu-id="d2d87-149">Ключевое значение "ключевое значение"</span><span class="sxs-lookup"><span data-stu-id="d2d87-149">Key real value pair</span></span>](intune-shared-keyrealvaluepair.md)
- [<span data-ttu-id="d2d87-150">Ключевая строка значений ключа</span><span class="sxs-lookup"><span data-stu-id="d2d87-150">Key string value pair</span></span>](intune-shared-keystringvaluepair.md)
- [<span data-ttu-id="d2d87-151">Комбинация типизированных типизированных значений</span><span class="sxs-lookup"><span data-stu-id="d2d87-151">Key typed value pair</span></span>](intune-shared-keytypedvaluepair.md)
- [<span data-ttu-id="d2d87-152">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="d2d87-152">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="d2d87-153">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="d2d87-153">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="d2d87-154">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="d2d87-154">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="d2d87-155">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="d2d87-155">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="d2d87-156">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="d2d87-156">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="d2d87-157">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="d2d87-157">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="d2d87-158">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="d2d87-158">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="d2d87-159">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="d2d87-159">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="d2d87-160">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="d2d87-160">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="d2d87-161">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="d2d87-161">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="d2d87-162">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="d2d87-162">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="d2d87-163">Тип владельца</span><span class="sxs-lookup"><span data-stu-id="d2d87-163">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="d2d87-164">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="d2d87-164">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="d2d87-165">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="d2d87-165">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="d2d87-166">Report</span><span class="sxs-lookup"><span data-stu-id="d2d87-166">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="d2d87-167">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="d2d87-167">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="d2d87-168">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="d2d87-168">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="d2d87-169">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="d2d87-169">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="d2d87-170">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="d2d87-170">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="d2d87-171">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="d2d87-171">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="d2d87-172">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="d2d87-172">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="d2d87-173">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="d2d87-173">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="d2d87-174">URI</span><span class="sxs-lookup"><span data-stu-id="d2d87-174">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="d2d87-175">User</span><span class="sxs-lookup"><span data-stu-id="d2d87-175">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="d2d87-176">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="d2d87-176">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="d2d87-177">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="d2d87-177">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="d2d87-178">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d2d87-178">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="d2d87-179">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d2d87-179">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="d2d87-180">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="d2d87-180">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="d2d87-181">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="d2d87-181">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="d2d87-182">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="d2d87-182">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="d2d87-183">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="d2d87-183">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="d2d87-184">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="d2d87-184">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="d2d87-185">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="d2d87-185">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="d2d87-186">Статус обновления Windows</span><span class="sxs-lookup"><span data-stu-id="d2d87-186">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

