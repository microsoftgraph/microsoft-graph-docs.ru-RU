---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 56950c21527c4bf72dd57e71d27f0b1be2e47046
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196345"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="f661c-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f661c-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="f661c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f661c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f661c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f661c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f661c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f661c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f661c-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="f661c-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="f661c-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="f661c-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="f661c-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="f661c-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="f661c-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="f661c-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="f661c-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="f661c-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="f661c-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="f661c-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="f661c-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="f661c-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="f661c-114">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="f661c-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="f661c-115">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="f661c-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="f661c-116">Источник назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="f661c-116">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="f661c-117">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="f661c-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="f661c-118">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="f661c-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="f661c-119">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="f661c-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="f661c-120">Политика соответствия устройств требованиям</span><span class="sxs-lookup"><span data-stu-id="f661c-120">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="f661c-121">Настройка устройства</span><span class="sxs-lookup"><span data-stu-id="f661c-121">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="f661c-122">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="f661c-122">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="f661c-123">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="f661c-123">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="f661c-124">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="f661c-124">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="f661c-125">Производный поставщик учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="f661c-125">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="f661c-126">Тип уведомления о получении учетных данных для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="f661c-126">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="f661c-127">Параметры производных учетных данных управления устройствами</span><span class="sxs-lookup"><span data-stu-id="f661c-127">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="f661c-128">Сценарий управления устройствами</span><span class="sxs-lookup"><span data-stu-id="f661c-128">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="f661c-129">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="f661c-129">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="f661c-130">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="f661c-130">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="f661c-131">Включение</span><span class="sxs-lookup"><span data-stu-id="f661c-131">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="f661c-132">Состояние регистрации</span><span class="sxs-lookup"><span data-stu-id="f661c-132">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="f661c-133">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="f661c-133">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="f661c-134">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="f661c-134">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="f661c-135">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="f661c-135">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="f661c-136">Настройки назначения бизнес-приложения iOS</span><span class="sxs-lookup"><span data-stu-id="f661c-136">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="f661c-137">Конфигурация подготовки бизнес-приложений iOS</span><span class="sxs-lookup"><span data-stu-id="f661c-137">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="f661c-138">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="f661c-138">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="f661c-139">Настройки назначения приложения из магазина iOS</span><span class="sxs-lookup"><span data-stu-id="f661c-139">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="f661c-140">Настройки назначения приложения iOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="f661c-140">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="f661c-141">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="f661c-141">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="f661c-142">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="f661c-142">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="f661c-143">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="f661c-143">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="f661c-144">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="f661c-144">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="f661c-145">Настройки назначения приложения macOS, приобретенного по программе VPP</span><span class="sxs-lookup"><span data-stu-id="f661c-145">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="f661c-146">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="f661c-146">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="f661c-147">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="f661c-147">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="f661c-148">Настройки назначения приложения из Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f661c-148">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="f661c-149">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="f661c-149">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="f661c-150">Мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="f661c-150">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="f661c-151">Настройки назначения мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="f661c-151">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="f661c-152">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="f661c-152">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="f661c-153">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="f661c-153">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="f661c-154">Report</span><span class="sxs-lookup"><span data-stu-id="f661c-154">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="f661c-155">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="f661c-155">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="f661c-156">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="f661c-156">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="f661c-157">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="f661c-157">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="f661c-158">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="f661c-158">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="f661c-159">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="f661c-159">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="f661c-160">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="f661c-160">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="f661c-161">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="f661c-161">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="f661c-162">URI</span><span class="sxs-lookup"><span data-stu-id="f661c-162">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="f661c-163">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="f661c-163">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="f661c-164">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="f661c-164">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="f661c-165">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="f661c-165">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="f661c-166">Настройки назначения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="f661c-166">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="f661c-167">Уведомление бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="f661c-167">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="f661c-168">Настройки назначения приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="f661c-168">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="f661c-169">Профиль Windows AutoPilot Deployment</span><span class="sxs-lookup"><span data-stu-id="f661c-169">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="f661c-170">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="f661c-170">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="f661c-171">Настройки назначения универсального приложения Windows AppX</span><span class="sxs-lookup"><span data-stu-id="f661c-171">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="f661c-172">Состояние центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="f661c-172">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="f661c-173">Статус обновления Windows</span><span class="sxs-lookup"><span data-stu-id="f661c-173">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

