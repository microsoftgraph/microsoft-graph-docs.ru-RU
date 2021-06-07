---
title: Create windowsInformationProtectionPolicy
description: Создание объекта windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32a6841ae42b038885e58005f3646d898219df3a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756921"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="796fd-103">Create windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="796fd-103">Create windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="796fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="796fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="796fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="796fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="796fd-106">Создание объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-106">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="796fd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="796fd-107">Prerequisites</span></span>
<span data-ttu-id="796fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="796fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="796fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="796fd-110">Permission type</span></span>|<span data-ttu-id="796fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="796fd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="796fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="796fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="796fd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796fd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="796fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="796fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="796fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="796fd-115">Not supported.</span></span>|
|<span data-ttu-id="796fd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="796fd-116">Application</span></span>|<span data-ttu-id="796fd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796fd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="796fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="796fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="796fd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="796fd-119">Request headers</span></span>
|<span data-ttu-id="796fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="796fd-120">Header</span></span>|<span data-ttu-id="796fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="796fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="796fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="796fd-122">Authorization</span></span>|<span data-ttu-id="796fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="796fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="796fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="796fd-124">Accept</span></span>|<span data-ttu-id="796fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="796fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="796fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="796fd-126">Request body</span></span>
<span data-ttu-id="796fd-127">В теле запроса добавьте представление объекта windowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="796fd-127">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="796fd-128">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="796fd-128">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="796fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="796fd-129">Property</span></span>|<span data-ttu-id="796fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="796fd-130">Type</span></span>|<span data-ttu-id="796fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="796fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="796fd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="796fd-132">displayName</span></span>|<span data-ttu-id="796fd-133">String</span><span class="sxs-lookup"><span data-stu-id="796fd-133">String</span></span>|<span data-ttu-id="796fd-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="796fd-134">Policy display name.</span></span> <span data-ttu-id="796fd-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-136">description</span><span class="sxs-lookup"><span data-stu-id="796fd-136">description</span></span>|<span data-ttu-id="796fd-137">String</span><span class="sxs-lookup"><span data-stu-id="796fd-137">String</span></span>|<span data-ttu-id="796fd-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="796fd-138">The policy's description.</span></span> <span data-ttu-id="796fd-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="796fd-140">createdDateTime</span></span>|<span data-ttu-id="796fd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796fd-141">DateTimeOffset</span></span>|<span data-ttu-id="796fd-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="796fd-142">The date and time the policy was created.</span></span> <span data-ttu-id="796fd-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="796fd-144">lastModifiedDateTime</span></span>|<span data-ttu-id="796fd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796fd-145">DateTimeOffset</span></span>|<span data-ttu-id="796fd-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="796fd-146">Last time the policy was modified.</span></span> <span data-ttu-id="796fd-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-148">id</span><span class="sxs-lookup"><span data-stu-id="796fd-148">id</span></span>|<span data-ttu-id="796fd-149">String</span><span class="sxs-lookup"><span data-stu-id="796fd-149">String</span></span>|<span data-ttu-id="796fd-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="796fd-150">Key of the entity.</span></span> <span data-ttu-id="796fd-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-152">version</span><span class="sxs-lookup"><span data-stu-id="796fd-152">version</span></span>|<span data-ttu-id="796fd-153">String</span><span class="sxs-lookup"><span data-stu-id="796fd-153">String</span></span>|<span data-ttu-id="796fd-154">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="796fd-154">Version of the entity.</span></span> <span data-ttu-id="796fd-155">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="796fd-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="796fd-156">enforcementLevel</span></span>|[<span data-ttu-id="796fd-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="796fd-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="796fd-158">Уровень правоприменения WIP. См. определение Enum для поддерживаемых значений, унаследованных от [windowsInformationProtection.](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="796fd-159">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="796fd-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="796fd-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="796fd-160">enterpriseDomain</span></span>|<span data-ttu-id="796fd-161">String</span><span class="sxs-lookup"><span data-stu-id="796fd-161">String</span></span>|<span data-ttu-id="796fd-162">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="796fd-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="796fd-164">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-165">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="796fd-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="796fd-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-167">Boolean</span></span>|<span data-ttu-id="796fd-168">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="796fd-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="796fd-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="796fd-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="796fd-171">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="796fd-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="796fd-172">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="796fd-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="796fd-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-174">Boolean</span></span>|<span data-ttu-id="796fd-175">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="796fd-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="796fd-176">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="796fd-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="796fd-177">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="796fd-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="796fd-178">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="796fd-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="796fd-180">Guid</span><span class="sxs-lookup"><span data-stu-id="796fd-180">Guid</span></span>|<span data-ttu-id="796fd-181">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="796fd-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="796fd-182">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="796fd-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="796fd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-184">Boolean</span></span>|<span data-ttu-id="796fd-185">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="796fd-186">iconsVisible</span></span>|<span data-ttu-id="796fd-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-187">Boolean</span></span>|<span data-ttu-id="796fd-188">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="796fd-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="796fd-189">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="796fd-190">protectedApps</span></span>|<span data-ttu-id="796fd-191">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="796fd-192">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="796fd-193">exemptApps</span></span>|<span data-ttu-id="796fd-194">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="796fd-195">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="796fd-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="796fd-196">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="796fd-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="796fd-197">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="796fd-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="796fd-199">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-200">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="796fd-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="796fd-201">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="796fd-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="796fd-203">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="796fd-204">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="796fd-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="796fd-205">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="796fd-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="796fd-206">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="796fd-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="796fd-207">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="796fd-208">enterpriseIPRanges</span></span>|<span data-ttu-id="796fd-209">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="796fd-210">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="796fd-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="796fd-211">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="796fd-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="796fd-212">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="796fd-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="796fd-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-214">Boolean</span></span>|<span data-ttu-id="796fd-215">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="796fd-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="796fd-216">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="796fd-217">enterpriseProxyServers</span></span>|<span data-ttu-id="796fd-218">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-219">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="796fd-219">This is a list of proxy servers.</span></span> <span data-ttu-id="796fd-220">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="796fd-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="796fd-222">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-223">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="796fd-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="796fd-224">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="796fd-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="796fd-225">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="796fd-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="796fd-226">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="796fd-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="796fd-227">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="796fd-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="796fd-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-229">Boolean</span></span>|<span data-ttu-id="796fd-230">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="796fd-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="796fd-231">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="796fd-232">neutralDomainResources</span></span>|<span data-ttu-id="796fd-233">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-234">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="796fd-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="796fd-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-236">Boolean</span></span>|<span data-ttu-id="796fd-237">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="796fd-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="796fd-239">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="796fd-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="796fd-240">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="796fd-241">isAssigned</span></span>|<span data-ttu-id="796fd-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-242">Boolean</span></span>|<span data-ttu-id="796fd-243">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="796fd-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="796fd-244">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="796fd-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="796fd-245">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="796fd-245">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="796fd-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-246">Boolean</span></span>|<span data-ttu-id="796fd-247">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="796fd-247">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="796fd-248">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="796fd-248">mdmEnrollmentUrl</span></span>|<span data-ttu-id="796fd-249">String</span><span class="sxs-lookup"><span data-stu-id="796fd-249">String</span></span>|<span data-ttu-id="796fd-250">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="796fd-250">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="796fd-251">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="796fd-251">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="796fd-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="796fd-252">Boolean</span></span>|<span data-ttu-id="796fd-253">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="796fd-253">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="796fd-254">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="796fd-254">pinMinimumLength</span></span>|<span data-ttu-id="796fd-255">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-255">Int32</span></span>|<span data-ttu-id="796fd-256">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="796fd-256">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="796fd-257">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="796fd-257">Default value is 4.</span></span> <span data-ttu-id="796fd-258">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="796fd-258">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="796fd-259">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="796fd-259">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="796fd-260">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="796fd-260">pinUppercaseLetters</span></span>|[<span data-ttu-id="796fd-261">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="796fd-261">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="796fd-262">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="796fd-262">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="796fd-263">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="796fd-263">Default is NotAllow.</span></span> <span data-ttu-id="796fd-264">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="796fd-264">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="796fd-265">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="796fd-265">pinLowercaseLetters</span></span>|[<span data-ttu-id="796fd-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="796fd-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="796fd-267">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="796fd-267">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="796fd-268">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="796fd-268">Default is NotAllow.</span></span> <span data-ttu-id="796fd-269">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="796fd-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="796fd-270">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="796fd-270">pinSpecialCharacters</span></span>|[<span data-ttu-id="796fd-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="796fd-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="796fd-272">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="796fd-272">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="796fd-273">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="796fd-273">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="796fd-274">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="796fd-274">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="796fd-275">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="796fd-275">/ : ; < = > ?</span></span><span data-ttu-id="796fd-276"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: ` notAllow `, ` requireAtLeastOne `, ` allow'.</span><span class="sxs-lookup"><span data-stu-id="796fd-276"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="796fd-277">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="796fd-277">pinExpirationDays</span></span>|<span data-ttu-id="796fd-278">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-278">Int32</span></span>|<span data-ttu-id="796fd-279">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="796fd-279">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="796fd-280">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="796fd-280">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="796fd-281">до 0.</span><span class="sxs-lookup"><span data-stu-id="796fd-281">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="796fd-282">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="796fd-282">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="796fd-283">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="796fd-283">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="796fd-284">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="796fd-284">Default is 0.</span></span>|
|<span data-ttu-id="796fd-285">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="796fd-285">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="796fd-286">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-286">Int32</span></span>|<span data-ttu-id="796fd-287">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="796fd-287">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="796fd-288">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="796fd-288">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="796fd-289">до 0.</span><span class="sxs-lookup"><span data-stu-id="796fd-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="796fd-290">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="796fd-290">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="796fd-291">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="796fd-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="796fd-292">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="796fd-292">Default is 0.</span></span>|
|<span data-ttu-id="796fd-293">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="796fd-293">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="796fd-294">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-294">Int32</span></span>|<span data-ttu-id="796fd-295">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="796fd-295">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="796fd-296">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="796fd-296">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="796fd-297">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="796fd-297">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="796fd-298">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="796fd-298">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="796fd-299">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-299">Int32</span></span>|<span data-ttu-id="796fd-300">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="796fd-300">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="796fd-301">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="796fd-301">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="796fd-302">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="796fd-302">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="796fd-303">Int32</span><span class="sxs-lookup"><span data-stu-id="796fd-303">Int32</span></span>|<span data-ttu-id="796fd-304">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях).</span><span class="sxs-lookup"><span data-stu-id="796fd-304">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="796fd-305">Ответ</span><span class="sxs-lookup"><span data-stu-id="796fd-305">Response</span></span>
<span data-ttu-id="796fd-306">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="796fd-306">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="796fd-307">Пример</span><span class="sxs-lookup"><span data-stu-id="796fd-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="796fd-308">Запрос</span><span class="sxs-lookup"><span data-stu-id="796fd-308">Request</span></span>
<span data-ttu-id="796fd-309">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="796fd-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4303

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.ipRange"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```

### <a name="response"></a><span data-ttu-id="796fd-310">Отклик</span><span class="sxs-lookup"><span data-stu-id="796fd-310">Response</span></span>
<span data-ttu-id="796fd-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="796fd-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4475

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "6397be61-be61-6397-61be-976361be9763",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.ipRange"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```




