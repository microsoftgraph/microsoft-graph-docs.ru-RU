---
title: Тип ресурса windowsInformationProtection
description: Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b8deab3dfaebc87b95035ef9f474f27783aa507
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443515"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="27df4-103">Тип ресурса windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="27df4-103">windowsInformationProtection resource type</span></span>

<span data-ttu-id="27df4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27df4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27df4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27df4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27df4-106">Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.</span><span class="sxs-lookup"><span data-stu-id="27df4-106">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="27df4-107">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="27df4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="27df4-108">Methods</span></span>
|<span data-ttu-id="27df4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="27df4-109">Method</span></span>|<span data-ttu-id="27df4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27df4-110">Return Type</span></span>|<span data-ttu-id="27df4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27df4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27df4-112">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="27df4-112">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="27df4-113">Коллекция объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="27df4-114">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-114">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="27df4-115">Получение объекта windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="27df4-115">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="27df4-116">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="27df4-116">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="27df4-117">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-117">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="27df4-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="27df4-118">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="27df4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="27df4-119">None</span></span>|<span data-ttu-id="27df4-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="27df4-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="27df4-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="27df4-121">Properties</span></span>
|<span data-ttu-id="27df4-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="27df4-122">Property</span></span>|<span data-ttu-id="27df4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="27df4-123">Type</span></span>|<span data-ttu-id="27df4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="27df4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27df4-125">displayName</span><span class="sxs-lookup"><span data-stu-id="27df4-125">displayName</span></span>|<span data-ttu-id="27df4-126">Строка</span><span class="sxs-lookup"><span data-stu-id="27df4-126">String</span></span>|<span data-ttu-id="27df4-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="27df4-127">Policy display name.</span></span> <span data-ttu-id="27df4-128">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-129">description</span><span class="sxs-lookup"><span data-stu-id="27df4-129">description</span></span>|<span data-ttu-id="27df4-130">String</span><span class="sxs-lookup"><span data-stu-id="27df4-130">String</span></span>|<span data-ttu-id="27df4-131">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="27df4-131">The policy's description.</span></span> <span data-ttu-id="27df4-132">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27df4-133">createdDateTime</span></span>|<span data-ttu-id="27df4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27df4-134">DateTimeOffset</span></span>|<span data-ttu-id="27df4-135">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="27df4-135">The date and time the policy was created.</span></span> <span data-ttu-id="27df4-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27df4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="27df4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27df4-138">DateTimeOffset</span></span>|<span data-ttu-id="27df4-139">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="27df4-139">Last time the policy was modified.</span></span> <span data-ttu-id="27df4-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-141">id</span><span class="sxs-lookup"><span data-stu-id="27df4-141">id</span></span>|<span data-ttu-id="27df4-142">String</span><span class="sxs-lookup"><span data-stu-id="27df4-142">String</span></span>|<span data-ttu-id="27df4-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="27df4-143">Key of the entity.</span></span> <span data-ttu-id="27df4-144">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-145">version</span><span class="sxs-lookup"><span data-stu-id="27df4-145">version</span></span>|<span data-ttu-id="27df4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="27df4-146">String</span></span>|<span data-ttu-id="27df4-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="27df4-147">Version of the entity.</span></span> <span data-ttu-id="27df4-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27df4-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="27df4-149">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="27df4-149">enforcementLevel</span></span>|[<span data-ttu-id="27df4-150">виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="27df4-150">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="27df4-151">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений.</span><span class="sxs-lookup"><span data-stu-id="27df4-151">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="27df4-152">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="27df4-152">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="27df4-153">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="27df4-153">enterpriseDomain</span></span>|<span data-ttu-id="27df4-154">String</span><span class="sxs-lookup"><span data-stu-id="27df4-154">String</span></span>|<span data-ttu-id="27df4-155">Основной корпоративный домен.</span><span class="sxs-lookup"><span data-stu-id="27df4-155">Primary enterprise domain</span></span>|
|<span data-ttu-id="27df4-156">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="27df4-156">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="27df4-157">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-157">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-158">Список корпоративных доменов, которые необходимо защитить.</span><span class="sxs-lookup"><span data-stu-id="27df4-158">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="27df4-159">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="27df4-159">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="27df4-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-160">Boolean</span></span>|<span data-ttu-id="27df4-161">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом).</span><span class="sxs-lookup"><span data-stu-id="27df4-161">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="27df4-162">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="27df4-162">dataRecoveryCertificate</span></span>|[<span data-ttu-id="27df4-163">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="27df4-163">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="27df4-164">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="27df4-164">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="27df4-165">То же, что сертификат DRA для шифрованной файловой системы (EFS).</span><span class="sxs-lookup"><span data-stu-id="27df4-165">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="27df4-166">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="27df4-166">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="27df4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-167">Boolean</span></span>|<span data-ttu-id="27df4-168">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="27df4-168">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="27df4-169">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="27df4-169">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="27df4-170">Если ключи не отзываются, файлы не очищаются.</span><span class="sxs-lookup"><span data-stu-id="27df4-170">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="27df4-171">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="27df4-171">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="27df4-172">Guid</span><span class="sxs-lookup"><span data-stu-id="27df4-172">Guid</span></span>|<span data-ttu-id="27df4-173">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="27df4-173">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="27df4-174">Шаблон RMS позволяет ИТ-администратору настроить доступ (и его длительность) к защищенному RMS файлу для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="27df4-174">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="27df4-175">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="27df4-175">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="27df4-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-176">Boolean</span></span>|<span data-ttu-id="27df4-177">Указывает, разрешать ли шифрование Azure RMS для WIP.</span><span class="sxs-lookup"><span data-stu-id="27df4-177">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="27df4-178">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="27df4-178">iconsVisible</span></span>|<span data-ttu-id="27df4-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-179">Boolean</span></span>|<span data-ttu-id="27df4-180">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов WIP в Проводнике и плиток приложений только для предприятий в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="27df4-180">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="27df4-181">Начиная с Windows 10 версии 1703, этот параметр также определяет, отображается ли значок WIP в заголовке окна защищенного приложения.</span><span class="sxs-lookup"><span data-stu-id="27df4-181">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="27df4-182">protectedApps</span><span class="sxs-lookup"><span data-stu-id="27df4-182">protectedApps</span></span>|<span data-ttu-id="27df4-183">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-183">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="27df4-184">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются.</span><span class="sxs-lookup"><span data-stu-id="27df4-184">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="27df4-185">exemptApps</span><span class="sxs-lookup"><span data-stu-id="27df4-185">exemptApps</span></span>|<span data-ttu-id="27df4-186">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-186">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="27df4-187">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="27df4-187">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="27df4-188">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="27df4-188">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="27df4-189">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="27df4-189">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="27df4-190">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-190">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-191">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="27df4-191">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="27df4-192">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно.</span><span class="sxs-lookup"><span data-stu-id="27df4-192">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="27df4-193">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="27df4-193">enterpriseProxiedDomains</span></span>|<span data-ttu-id="27df4-194">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-194">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="27df4-195">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="27df4-195">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="27df4-196">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="27df4-196">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="27df4-197">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="27df4-197">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="27df4-198">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="27df4-198">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="27df4-199">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="27df4-199">enterpriseIPRanges</span></span>|<span data-ttu-id="27df4-200">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-200">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="27df4-201">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="27df4-201">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="27df4-202">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="27df4-202">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="27df4-203">Считается, что отправлять корпоративные данные на эти компьютеры безопасно.</span><span class="sxs-lookup"><span data-stu-id="27df4-203">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="27df4-204">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="27df4-204">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="27df4-205">Логический</span><span class="sxs-lookup"><span data-stu-id="27df4-205">Boolean</span></span>|<span data-ttu-id="27df4-206">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="27df4-206">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="27df4-207">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="27df4-207">Default is false</span></span>|
|<span data-ttu-id="27df4-208">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="27df4-208">enterpriseProxyServers</span></span>|<span data-ttu-id="27df4-209">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-210">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="27df4-210">This is a list of proxy servers.</span></span> <span data-ttu-id="27df4-211">Сервер, который не входит в этот список, не считается корпоративным.</span><span class="sxs-lookup"><span data-stu-id="27df4-211">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="27df4-212">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="27df4-212">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="27df4-213">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-214">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="27df4-214">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="27df4-215">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="27df4-215">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="27df4-216">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="27df4-216">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="27df4-217">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="27df4-217">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="27df4-218">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="27df4-218">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="27df4-219">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="27df4-219">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="27df4-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-220">Boolean</span></span>|<span data-ttu-id="27df4-221">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="27df4-221">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="27df4-222">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="27df4-222">Default is false</span></span>|
|<span data-ttu-id="27df4-223">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="27df4-223">neutralDomainResources</span></span>|<span data-ttu-id="27df4-224">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-224">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-225">Список доменных имен, которые можно использовать для рабочих или личных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="27df4-225">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="27df4-226">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="27df4-226">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="27df4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="27df4-227">Boolean</span></span>|<span data-ttu-id="27df4-228">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы.</span><span class="sxs-lookup"><span data-stu-id="27df4-228">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="27df4-229">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="27df4-229">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="27df4-230">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="27df4-231">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия.</span><span class="sxs-lookup"><span data-stu-id="27df4-231">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="27df4-232">isAssigned</span><span class="sxs-lookup"><span data-stu-id="27df4-232">isAssigned</span></span>|<span data-ttu-id="27df4-233">Логический</span><span class="sxs-lookup"><span data-stu-id="27df4-233">Boolean</span></span>|<span data-ttu-id="27df4-234">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="27df4-234">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27df4-235">Связи</span><span class="sxs-lookup"><span data-stu-id="27df4-235">Relationships</span></span>
|<span data-ttu-id="27df4-236">Связь</span><span class="sxs-lookup"><span data-stu-id="27df4-236">Relationship</span></span>|<span data-ttu-id="27df4-237">Тип</span><span class="sxs-lookup"><span data-stu-id="27df4-237">Type</span></span>|<span data-ttu-id="27df4-238">Описание</span><span class="sxs-lookup"><span data-stu-id="27df4-238">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27df4-239">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="27df4-239">protectedAppLockerFiles</span></span>|<span data-ttu-id="27df4-240">Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-240">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="27df4-241">Еще один способ ввести данные о защищенных приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="27df4-241">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="27df4-242">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="27df4-242">exemptAppLockerFiles</span></span>|<span data-ttu-id="27df4-243">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-243">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="27df4-244">Еще один способ ввести данные об исключаемых приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="27df4-244">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="27df4-245">assignments</span><span class="sxs-lookup"><span data-stu-id="27df4-245">assignments</span></span>|<span data-ttu-id="27df4-246">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="27df4-246">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="27df4-247">Список групп безопасности, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="27df4-247">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27df4-248">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27df4-248">JSON Representation</span></span>
<span data-ttu-id="27df4-249">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27df4-249">Here is a JSON representation of the resource.</span></span>
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







