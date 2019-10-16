---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 1420f751866224905f1636205de173e3bd117451
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539171"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="adbf7-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="adbf7-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="adbf7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adbf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adbf7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbf7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adbf7-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adbf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adbf7-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="adbf7-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="adbf7-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="adbf7-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="adbf7-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="adbf7-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="adbf7-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="adbf7-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="adbf7-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="adbf7-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="adbf7-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="adbf7-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="adbf7-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="adbf7-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="adbf7-114">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="adbf7-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="adbf7-115">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="adbf7-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="adbf7-116">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="adbf7-116">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="adbf7-117">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="adbf7-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="adbf7-118">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="adbf7-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="adbf7-119">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="adbf7-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="adbf7-120">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="adbf7-120">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="adbf7-121">Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="adbf7-121">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="adbf7-122">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="adbf7-122">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="adbf7-123">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="adbf7-123">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="adbf7-124">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="adbf7-124">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="adbf7-125">Производный поставщик учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="adbf7-125">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="adbf7-126">Тип уведомления о получении учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="adbf7-126">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="adbf7-127">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="adbf7-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="adbf7-128">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="adbf7-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="adbf7-129">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="adbf7-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="adbf7-130">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="adbf7-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="adbf7-131">Включение</span><span class="sxs-lookup"><span data-stu-id="adbf7-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="adbf7-132">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="adbf7-132">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="adbf7-133">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="adbf7-133">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="adbf7-134">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="adbf7-134">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="adbf7-135">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="adbf7-135">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="adbf7-136">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="adbf7-136">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="adbf7-137">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="adbf7-137">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="adbf7-138">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="adbf7-138">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="adbf7-139">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="adbf7-139">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="adbf7-140">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="adbf7-140">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="adbf7-141">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="adbf7-141">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="adbf7-142">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="adbf7-142">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="adbf7-143">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="adbf7-143">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="adbf7-144">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="adbf7-144">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="adbf7-145">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="adbf7-145">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="adbf7-146">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="adbf7-146">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="adbf7-147">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="adbf7-147">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="adbf7-148">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="adbf7-148">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="adbf7-149">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="adbf7-149">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="adbf7-150">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="adbf7-150">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="adbf7-151">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="adbf7-151">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="adbf7-152">Параметры времени установки мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="adbf7-152">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="adbf7-153">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="adbf7-153">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="adbf7-154">Тип платформы политики</span><span class="sxs-lookup"><span data-stu-id="adbf7-154">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="adbf7-155">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="adbf7-155">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="adbf7-156">Report</span><span class="sxs-lookup"><span data-stu-id="adbf7-156">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="adbf7-157">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="adbf7-157">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="adbf7-158">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="adbf7-158">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="adbf7-159">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="adbf7-159">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="adbf7-160">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="adbf7-160">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="adbf7-161">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="adbf7-161">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="adbf7-162">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="adbf7-162">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="adbf7-163">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="adbf7-163">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="adbf7-164">URI</span><span class="sxs-lookup"><span data-stu-id="adbf7-164">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="adbf7-165">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="adbf7-165">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="adbf7-166">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="adbf7-166">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="adbf7-167">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="adbf7-167">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="adbf7-168">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="adbf7-168">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="adbf7-169">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="adbf7-169">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="adbf7-170">Параметры перезапуска приложения Win32 LOB</span><span class="sxs-lookup"><span data-stu-id="adbf7-170">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="adbf7-171">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="adbf7-171">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="adbf7-172">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="adbf7-172">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="adbf7-173">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="adbf7-173">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="adbf7-174">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="adbf7-174">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="adbf7-175">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="adbf7-175">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="adbf7-176">Статус обновления Windows</span><span class="sxs-lookup"><span data-stu-id="adbf7-176">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

