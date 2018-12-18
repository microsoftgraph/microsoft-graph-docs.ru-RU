---
title: Тип ресурса windowsInformationProtection
description: Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.
author: tfitzmac
ms.openlocfilehash: 86c1202636046320312cd12fb5d97b98937a2cec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349226"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="11d4f-103">Тип ресурса windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="11d4f-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="11d4f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11d4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11d4f-105">Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.</span><span class="sxs-lookup"><span data-stu-id="11d4f-105">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="11d4f-106">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="11d4f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11d4f-107">Methods</span></span>
|<span data-ttu-id="11d4f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11d4f-108">Method</span></span>|<span data-ttu-id="11d4f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11d4f-109">Return Type</span></span>|<span data-ttu-id="11d4f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11d4f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11d4f-111">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="11d4f-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="11d4f-112">Коллекция объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="11d4f-113">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="11d4f-114">Получение объекта windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="11d4f-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="11d4f-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="11d4f-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="11d4f-116">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="11d4f-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="11d4f-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="11d4f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="11d4f-118">None</span></span>|<span data-ttu-id="11d4f-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11d4f-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="11d4f-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="11d4f-120">Properties</span></span>
|<span data-ttu-id="11d4f-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="11d4f-121">Property</span></span>|<span data-ttu-id="11d4f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="11d4f-122">Type</span></span>|<span data-ttu-id="11d4f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="11d4f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11d4f-124">displayName</span><span class="sxs-lookup"><span data-stu-id="11d4f-124">displayName</span></span>|<span data-ttu-id="11d4f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="11d4f-125">String</span></span>|<span data-ttu-id="11d4f-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="11d4f-126">Policy display name.</span></span> <span data-ttu-id="11d4f-127">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-128">описание</span><span class="sxs-lookup"><span data-stu-id="11d4f-128">description</span></span>|<span data-ttu-id="11d4f-129">Строка</span><span class="sxs-lookup"><span data-stu-id="11d4f-129">String</span></span>|<span data-ttu-id="11d4f-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="11d4f-130">The policy's description.</span></span> <span data-ttu-id="11d4f-131">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11d4f-132">createdDateTime</span></span>|<span data-ttu-id="11d4f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11d4f-133">DateTimeOffset</span></span>|<span data-ttu-id="11d4f-134">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="11d4f-134">The date and time the policy was created.</span></span> <span data-ttu-id="11d4f-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11d4f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="11d4f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11d4f-137">DateTimeOffset</span></span>|<span data-ttu-id="11d4f-138">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="11d4f-138">Last time the policy was modified.</span></span> <span data-ttu-id="11d4f-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-140">id</span><span class="sxs-lookup"><span data-stu-id="11d4f-140">id</span></span>|<span data-ttu-id="11d4f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="11d4f-141">String</span></span>|<span data-ttu-id="11d4f-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11d4f-142">Key of the entity.</span></span> <span data-ttu-id="11d4f-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-144">version</span><span class="sxs-lookup"><span data-stu-id="11d4f-144">version</span></span>|<span data-ttu-id="11d4f-145">Строка</span><span class="sxs-lookup"><span data-stu-id="11d4f-145">String</span></span>|<span data-ttu-id="11d4f-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="11d4f-146">Version of the entity.</span></span> <span data-ttu-id="11d4f-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="11d4f-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="11d4f-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="11d4f-148">enforcementLevel</span></span>|[<span data-ttu-id="11d4f-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="11d4f-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="11d4f-150">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений.</span><span class="sxs-lookup"><span data-stu-id="11d4f-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="11d4f-151">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="11d4f-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="11d4f-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="11d4f-152">enterpriseDomain</span></span>|<span data-ttu-id="11d4f-153">String</span><span class="sxs-lookup"><span data-stu-id="11d4f-153">String</span></span>|<span data-ttu-id="11d4f-154">Основной корпоративный домен.</span><span class="sxs-lookup"><span data-stu-id="11d4f-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="11d4f-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="11d4f-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="11d4f-156">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-157">Список корпоративных доменов, которые необходимо защитить.</span><span class="sxs-lookup"><span data-stu-id="11d4f-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="11d4f-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="11d4f-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="11d4f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-159">Boolean</span></span>|<span data-ttu-id="11d4f-160">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом).</span><span class="sxs-lookup"><span data-stu-id="11d4f-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="11d4f-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="11d4f-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="11d4f-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="11d4f-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="11d4f-163">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="11d4f-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="11d4f-164">То же, что сертификат DRA для шифрованной файловой системы (EFS).</span><span class="sxs-lookup"><span data-stu-id="11d4f-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="11d4f-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="11d4f-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="11d4f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-166">Boolean</span></span>|<span data-ttu-id="11d4f-167">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="11d4f-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="11d4f-168">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="11d4f-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="11d4f-169">Если ключи не отзываются, файлы не очищаются.</span><span class="sxs-lookup"><span data-stu-id="11d4f-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="11d4f-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="11d4f-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="11d4f-171">Guid</span><span class="sxs-lookup"><span data-stu-id="11d4f-171">Guid</span></span>|<span data-ttu-id="11d4f-172">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="11d4f-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="11d4f-173">Шаблон RMS позволяет ИТ-администратору настроить доступ (и его длительность) к защищенному RMS файлу для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="11d4f-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="11d4f-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="11d4f-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="11d4f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-175">Boolean</span></span>|<span data-ttu-id="11d4f-176">Указывает, разрешать ли шифрование Azure RMS для WIP.</span><span class="sxs-lookup"><span data-stu-id="11d4f-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="11d4f-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="11d4f-177">iconsVisible</span></span>|<span data-ttu-id="11d4f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-178">Boolean</span></span>|<span data-ttu-id="11d4f-179">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов WIP в Проводнике и плиток приложений только для предприятий в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="11d4f-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="11d4f-180">Начиная с Windows 10 версии 1703, этот параметр также определяет, отображается ли значок WIP в заголовке окна защищенного приложения.</span><span class="sxs-lookup"><span data-stu-id="11d4f-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="11d4f-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="11d4f-181">protectedApps</span></span>|<span data-ttu-id="11d4f-182">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="11d4f-183">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются.</span><span class="sxs-lookup"><span data-stu-id="11d4f-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="11d4f-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="11d4f-184">exemptApps</span></span>|<span data-ttu-id="11d4f-185">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="11d4f-186">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="11d4f-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="11d4f-187">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="11d4f-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="11d4f-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="11d4f-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="11d4f-189">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-190">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="11d4f-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="11d4f-191">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно.</span><span class="sxs-lookup"><span data-stu-id="11d4f-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="11d4f-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="11d4f-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="11d4f-193">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="11d4f-194">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="11d4f-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="11d4f-195">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="11d4f-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="11d4f-196">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="11d4f-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="11d4f-197">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="11d4f-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="11d4f-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="11d4f-198">enterpriseIPRanges</span></span>|<span data-ttu-id="11d4f-199">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="11d4f-200">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="11d4f-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="11d4f-201">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="11d4f-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="11d4f-202">Считается, что отправлять корпоративные данные на эти компьютеры безопасно.</span><span class="sxs-lookup"><span data-stu-id="11d4f-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="11d4f-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="11d4f-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="11d4f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-204">Boolean</span></span>|<span data-ttu-id="11d4f-205">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="11d4f-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="11d4f-206">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="11d4f-206">Default is false</span></span>|
|<span data-ttu-id="11d4f-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="11d4f-207">enterpriseProxyServers</span></span>|<span data-ttu-id="11d4f-208">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-209">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="11d4f-209">This is a list of proxy servers.</span></span> <span data-ttu-id="11d4f-210">Сервер, который не входит в этот список, не считается корпоративным.</span><span class="sxs-lookup"><span data-stu-id="11d4f-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="11d4f-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="11d4f-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="11d4f-212">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-213">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="11d4f-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="11d4f-214">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="11d4f-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="11d4f-215">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="11d4f-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="11d4f-216">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="11d4f-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="11d4f-217">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="11d4f-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="11d4f-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="11d4f-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="11d4f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-219">Boolean</span></span>|<span data-ttu-id="11d4f-220">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="11d4f-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="11d4f-221">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="11d4f-221">Default is false</span></span>|
|<span data-ttu-id="11d4f-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="11d4f-222">neutralDomainResources</span></span>|<span data-ttu-id="11d4f-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-224">Список доменных имен, которые можно использовать для рабочих или личных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="11d4f-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="11d4f-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="11d4f-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="11d4f-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-226">Boolean</span></span>|<span data-ttu-id="11d4f-227">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы.</span><span class="sxs-lookup"><span data-stu-id="11d4f-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="11d4f-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="11d4f-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="11d4f-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="11d4f-230">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия.</span><span class="sxs-lookup"><span data-stu-id="11d4f-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="11d4f-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="11d4f-231">isAssigned</span></span>|<span data-ttu-id="11d4f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d4f-232">Boolean</span></span>|<span data-ttu-id="11d4f-233">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="11d4f-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11d4f-234">Связи</span><span class="sxs-lookup"><span data-stu-id="11d4f-234">Relationships</span></span>
|<span data-ttu-id="11d4f-235">Связь</span><span class="sxs-lookup"><span data-stu-id="11d4f-235">Relationship</span></span>|<span data-ttu-id="11d4f-236">Тип</span><span class="sxs-lookup"><span data-stu-id="11d4f-236">Type</span></span>|<span data-ttu-id="11d4f-237">Описание</span><span class="sxs-lookup"><span data-stu-id="11d4f-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11d4f-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="11d4f-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="11d4f-239">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="11d4f-240">Еще один способ ввести данные о защищенных приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="11d4f-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="11d4f-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="11d4f-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="11d4f-242">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="11d4f-243">Еще один способ ввести данные об исключаемых приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="11d4f-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="11d4f-244">assignments</span><span class="sxs-lookup"><span data-stu-id="11d4f-244">assignments</span></span>|<span data-ttu-id="11d4f-245">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11d4f-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="11d4f-246">Список групп безопасности, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="11d4f-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11d4f-247">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11d4f-247">JSON Representation</span></span>
<span data-ttu-id="11d4f-248">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11d4f-248">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



