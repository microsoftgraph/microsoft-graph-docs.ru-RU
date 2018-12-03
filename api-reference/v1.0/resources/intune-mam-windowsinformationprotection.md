---
title: Тип ресурса windowsInformationProtection
description: Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.
ms.openlocfilehash: fed8a72a3d90a5dd016292272f691e025abe1a57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026659"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="abbe1-103">Тип ресурса windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="abbe1-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="abbe1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abbe1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abbe1-105">Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.</span><span class="sxs-lookup"><span data-stu-id="abbe1-105">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="abbe1-106">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="abbe1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="abbe1-107">Methods</span></span>
|<span data-ttu-id="abbe1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="abbe1-108">Method</span></span>|<span data-ttu-id="abbe1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abbe1-109">Return Type</span></span>|<span data-ttu-id="abbe1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="abbe1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abbe1-111">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="abbe1-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="abbe1-112">Коллекция объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="abbe1-113">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="abbe1-114">Получение объекта windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="abbe1-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="abbe1-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="abbe1-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="abbe1-116">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="abbe1-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="abbe1-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="abbe1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="abbe1-118">None</span></span>|<span data-ttu-id="abbe1-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="abbe1-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="abbe1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="abbe1-120">Properties</span></span>
|<span data-ttu-id="abbe1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="abbe1-121">Property</span></span>|<span data-ttu-id="abbe1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="abbe1-122">Type</span></span>|<span data-ttu-id="abbe1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abbe1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbe1-124">displayName</span><span class="sxs-lookup"><span data-stu-id="abbe1-124">displayName</span></span>|<span data-ttu-id="abbe1-125">String</span><span class="sxs-lookup"><span data-stu-id="abbe1-125">String</span></span>|<span data-ttu-id="abbe1-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="abbe1-126">Policy display name.</span></span> <span data-ttu-id="abbe1-127">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-128">описание</span><span class="sxs-lookup"><span data-stu-id="abbe1-128">description</span></span>|<span data-ttu-id="abbe1-129">String</span><span class="sxs-lookup"><span data-stu-id="abbe1-129">String</span></span>|<span data-ttu-id="abbe1-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="abbe1-130">The policy's description.</span></span> <span data-ttu-id="abbe1-131">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abbe1-132">createdDateTime</span></span>|<span data-ttu-id="abbe1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbe1-133">DateTimeOffset</span></span>|<span data-ttu-id="abbe1-134">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="abbe1-134">The date and time the policy was created.</span></span> <span data-ttu-id="abbe1-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abbe1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="abbe1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbe1-137">DateTimeOffset</span></span>|<span data-ttu-id="abbe1-138">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="abbe1-138">Last time the policy was modified.</span></span> <span data-ttu-id="abbe1-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-140">id</span><span class="sxs-lookup"><span data-stu-id="abbe1-140">id</span></span>|<span data-ttu-id="abbe1-141">String</span><span class="sxs-lookup"><span data-stu-id="abbe1-141">String</span></span>|<span data-ttu-id="abbe1-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="abbe1-142">Key of the entity.</span></span> <span data-ttu-id="abbe1-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-144">version</span><span class="sxs-lookup"><span data-stu-id="abbe1-144">version</span></span>|<span data-ttu-id="abbe1-145">String</span><span class="sxs-lookup"><span data-stu-id="abbe1-145">String</span></span>|<span data-ttu-id="abbe1-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="abbe1-146">Version of the entity.</span></span> <span data-ttu-id="abbe1-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="abbe1-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="abbe1-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="abbe1-148">enforcementLevel</span></span>|[<span data-ttu-id="abbe1-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="abbe1-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="abbe1-150">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений.</span><span class="sxs-lookup"><span data-stu-id="abbe1-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="abbe1-151">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="abbe1-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="abbe1-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="abbe1-152">enterpriseDomain</span></span>|<span data-ttu-id="abbe1-153">String</span><span class="sxs-lookup"><span data-stu-id="abbe1-153">String</span></span>|<span data-ttu-id="abbe1-154">Основной корпоративный домен.</span><span class="sxs-lookup"><span data-stu-id="abbe1-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="abbe1-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="abbe1-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="abbe1-156">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-157">Список корпоративных доменов, которые необходимо защитить.</span><span class="sxs-lookup"><span data-stu-id="abbe1-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="abbe1-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="abbe1-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="abbe1-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbe1-159">Boolean</span></span>|<span data-ttu-id="abbe1-160">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом).</span><span class="sxs-lookup"><span data-stu-id="abbe1-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="abbe1-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="abbe1-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="abbe1-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="abbe1-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="abbe1-163">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="abbe1-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="abbe1-164">То же, что сертификат DRA для шифрованной файловой системы (EFS).</span><span class="sxs-lookup"><span data-stu-id="abbe1-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="abbe1-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="abbe1-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="abbe1-166">Логический</span><span class="sxs-lookup"><span data-stu-id="abbe1-166">Boolean</span></span>|<span data-ttu-id="abbe1-167">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="abbe1-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="abbe1-168">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="abbe1-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="abbe1-169">Если ключи не отзываются, файлы не очищаются.</span><span class="sxs-lookup"><span data-stu-id="abbe1-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="abbe1-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="abbe1-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="abbe1-171">Guid</span><span class="sxs-lookup"><span data-stu-id="abbe1-171">Guid</span></span>|<span data-ttu-id="abbe1-172">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="abbe1-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="abbe1-173">Шаблон RMS позволяет ИТ-администратору настроить доступ (и его длительность) к защищенному RMS файлу для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="abbe1-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="abbe1-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="abbe1-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="abbe1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbe1-175">Boolean</span></span>|<span data-ttu-id="abbe1-176">Указывает, разрешать ли шифрование Azure RMS для WIP.</span><span class="sxs-lookup"><span data-stu-id="abbe1-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="abbe1-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="abbe1-177">iconsVisible</span></span>|<span data-ttu-id="abbe1-178">Логический</span><span class="sxs-lookup"><span data-stu-id="abbe1-178">Boolean</span></span>|<span data-ttu-id="abbe1-179">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов WIP в Проводнике и плиток приложений только для предприятий в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="abbe1-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="abbe1-180">Начиная с Windows 10 версии 1703, этот параметр также определяет, отображается ли значок WIP в заголовке окна защищенного приложения.</span><span class="sxs-lookup"><span data-stu-id="abbe1-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="abbe1-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="abbe1-181">protectedApps</span></span>|<span data-ttu-id="abbe1-182">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="abbe1-183">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются.</span><span class="sxs-lookup"><span data-stu-id="abbe1-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="abbe1-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="abbe1-184">exemptApps</span></span>|<span data-ttu-id="abbe1-185">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="abbe1-186">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="abbe1-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="abbe1-187">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="abbe1-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="abbe1-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="abbe1-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="abbe1-189">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-190">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="abbe1-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="abbe1-191">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно.</span><span class="sxs-lookup"><span data-stu-id="abbe1-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="abbe1-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="abbe1-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="abbe1-193">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="abbe1-194">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="abbe1-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="abbe1-195">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="abbe1-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="abbe1-196">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="abbe1-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="abbe1-197">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="abbe1-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="abbe1-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="abbe1-198">enterpriseIPRanges</span></span>|<span data-ttu-id="abbe1-199">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="abbe1-200">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="abbe1-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="abbe1-201">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="abbe1-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="abbe1-202">Считается, что отправлять корпоративные данные на эти компьютеры безопасно.</span><span class="sxs-lookup"><span data-stu-id="abbe1-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="abbe1-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="abbe1-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="abbe1-204">Логический</span><span class="sxs-lookup"><span data-stu-id="abbe1-204">Boolean</span></span>|<span data-ttu-id="abbe1-205">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="abbe1-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="abbe1-206">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="abbe1-206">Default is false</span></span>|
|<span data-ttu-id="abbe1-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="abbe1-207">enterpriseProxyServers</span></span>|<span data-ttu-id="abbe1-208">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-209">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="abbe1-209">This is a list of proxy servers.</span></span> <span data-ttu-id="abbe1-210">Сервер, который не входит в этот список, не считается корпоративным.</span><span class="sxs-lookup"><span data-stu-id="abbe1-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="abbe1-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="abbe1-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="abbe1-212">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-213">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="abbe1-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="abbe1-214">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="abbe1-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="abbe1-215">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="abbe1-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="abbe1-216">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="abbe1-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="abbe1-217">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="abbe1-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="abbe1-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="abbe1-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="abbe1-219">Логический</span><span class="sxs-lookup"><span data-stu-id="abbe1-219">Boolean</span></span>|<span data-ttu-id="abbe1-220">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="abbe1-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="abbe1-221">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="abbe1-221">Default is false</span></span>|
|<span data-ttu-id="abbe1-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="abbe1-222">neutralDomainResources</span></span>|<span data-ttu-id="abbe1-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-224">Список доменных имен, которые можно использовать для рабочих или личных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="abbe1-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="abbe1-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="abbe1-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="abbe1-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="abbe1-226">Boolean</span></span>|<span data-ttu-id="abbe1-227">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы.</span><span class="sxs-lookup"><span data-stu-id="abbe1-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="abbe1-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="abbe1-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="abbe1-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="abbe1-230">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия.</span><span class="sxs-lookup"><span data-stu-id="abbe1-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="abbe1-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="abbe1-231">isAssigned</span></span>|<span data-ttu-id="abbe1-232">Логический</span><span class="sxs-lookup"><span data-stu-id="abbe1-232">Boolean</span></span>|<span data-ttu-id="abbe1-233">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="abbe1-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abbe1-234">Связи</span><span class="sxs-lookup"><span data-stu-id="abbe1-234">Relationships</span></span>
|<span data-ttu-id="abbe1-235">Связь</span><span class="sxs-lookup"><span data-stu-id="abbe1-235">Relationship</span></span>|<span data-ttu-id="abbe1-236">Тип</span><span class="sxs-lookup"><span data-stu-id="abbe1-236">Type</span></span>|<span data-ttu-id="abbe1-237">Описание</span><span class="sxs-lookup"><span data-stu-id="abbe1-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbe1-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="abbe1-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="abbe1-239">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="abbe1-240">Еще один способ ввести данные о защищенных приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="abbe1-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="abbe1-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="abbe1-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="abbe1-242">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="abbe1-243">Еще один способ ввести данные об исключаемых приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="abbe1-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="abbe1-244">assignments</span><span class="sxs-lookup"><span data-stu-id="abbe1-244">assignments</span></span>|<span data-ttu-id="abbe1-245">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abbe1-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="abbe1-246">Список групп безопасности, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="abbe1-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abbe1-247">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abbe1-247">JSON Representation</span></span>
<span data-ttu-id="abbe1-248">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abbe1-248">Here is a JSON representation of the resource.</span></span>
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



