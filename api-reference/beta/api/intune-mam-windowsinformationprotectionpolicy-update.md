---
title: Обновление объекта windowsInformationProtectionPolicy
description: Обновление свойств объекта windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db7d45945d9427e666b629b120c47575da002d37
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285704"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="84242-103">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="84242-103">Update windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="84242-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84242-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84242-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84242-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84242-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84242-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84242-107">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-107">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84242-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84242-108">Prerequisites</span></span>
<span data-ttu-id="84242-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84242-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84242-111">Permission type</span></span>|<span data-ttu-id="84242-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84242-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84242-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84242-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84242-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84242-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84242-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84242-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84242-116">Not supported.</span></span>|
|<span data-ttu-id="84242-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84242-117">Application</span></span>|<span data-ttu-id="84242-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84242-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84242-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84242-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="84242-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84242-120">Request headers</span></span>
|<span data-ttu-id="84242-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84242-121">Header</span></span>|<span data-ttu-id="84242-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84242-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84242-123">Authorization</span></span>|<span data-ttu-id="84242-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84242-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84242-125">Accept</span></span>|<span data-ttu-id="84242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84242-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84242-127">Request body</span></span>
<span data-ttu-id="84242-128">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84242-128">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="84242-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-129">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="84242-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84242-130">Property</span></span>|<span data-ttu-id="84242-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84242-131">Type</span></span>|<span data-ttu-id="84242-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84242-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84242-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84242-133">displayName</span></span>|<span data-ttu-id="84242-134">String</span><span class="sxs-lookup"><span data-stu-id="84242-134">String</span></span>|<span data-ttu-id="84242-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="84242-135">Policy display name.</span></span> <span data-ttu-id="84242-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-137">description</span><span class="sxs-lookup"><span data-stu-id="84242-137">description</span></span>|<span data-ttu-id="84242-138">String</span><span class="sxs-lookup"><span data-stu-id="84242-138">String</span></span>|<span data-ttu-id="84242-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="84242-139">The policy's description.</span></span> <span data-ttu-id="84242-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84242-141">createdDateTime</span></span>|<span data-ttu-id="84242-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84242-142">DateTimeOffset</span></span>|<span data-ttu-id="84242-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="84242-143">The date and time the policy was created.</span></span> <span data-ttu-id="84242-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84242-145">lastModifiedDateTime</span></span>|<span data-ttu-id="84242-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84242-146">DateTimeOffset</span></span>|<span data-ttu-id="84242-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="84242-147">Last time the policy was modified.</span></span> <span data-ttu-id="84242-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84242-149">roleScopeTagIds</span></span>|<span data-ttu-id="84242-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="84242-150">String collection</span></span>|<span data-ttu-id="84242-151">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="84242-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84242-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-153">id</span><span class="sxs-lookup"><span data-stu-id="84242-153">id</span></span>|<span data-ttu-id="84242-154">String</span><span class="sxs-lookup"><span data-stu-id="84242-154">String</span></span>|<span data-ttu-id="84242-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84242-155">Key of the entity.</span></span> <span data-ttu-id="84242-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-157">version</span><span class="sxs-lookup"><span data-stu-id="84242-157">version</span></span>|<span data-ttu-id="84242-158">String</span><span class="sxs-lookup"><span data-stu-id="84242-158">String</span></span>|<span data-ttu-id="84242-159">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="84242-159">Version of the entity.</span></span> <span data-ttu-id="84242-160">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84242-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="84242-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="84242-161">enforcementLevel</span></span>|[<span data-ttu-id="84242-162">виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="84242-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="84242-163">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="84242-164">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="84242-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="84242-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="84242-165">enterpriseDomain</span></span>|<span data-ttu-id="84242-166">String</span><span class="sxs-lookup"><span data-stu-id="84242-166">String</span></span>|<span data-ttu-id="84242-167">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="84242-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="84242-169">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-170">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="84242-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="84242-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-172">Boolean</span></span>|<span data-ttu-id="84242-173">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="84242-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="84242-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="84242-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="84242-176">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="84242-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="84242-177">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="84242-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="84242-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-179">Boolean</span></span>|<span data-ttu-id="84242-180">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="84242-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="84242-181">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="84242-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="84242-182">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="84242-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="84242-183">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="84242-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="84242-185">Guid</span><span class="sxs-lookup"><span data-stu-id="84242-185">Guid</span></span>|<span data-ttu-id="84242-186">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="84242-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="84242-187">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="84242-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="84242-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-189">Boolean</span></span>|<span data-ttu-id="84242-190">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="84242-191">iconsVisible</span></span>|<span data-ttu-id="84242-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-192">Boolean</span></span>|<span data-ttu-id="84242-193">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="84242-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="84242-194">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="84242-195">protectedApps</span></span>|<span data-ttu-id="84242-196">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="84242-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="84242-197">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="84242-198">exemptApps</span></span>|<span data-ttu-id="84242-199">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="84242-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="84242-200">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="84242-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="84242-201">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="84242-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="84242-202">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="84242-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="84242-204">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-205">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="84242-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="84242-206">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="84242-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="84242-208">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="84242-209">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="84242-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="84242-210">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="84242-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="84242-211">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="84242-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="84242-212">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="84242-213">enterpriseIPRanges</span></span>|<span data-ttu-id="84242-214">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="84242-215">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="84242-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="84242-216">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="84242-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="84242-217">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="84242-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="84242-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-219">Boolean</span></span>|<span data-ttu-id="84242-220">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="84242-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="84242-221">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="84242-222">enterpriseProxyServers</span></span>|<span data-ttu-id="84242-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-224">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="84242-224">This is a list of proxy servers.</span></span> <span data-ttu-id="84242-225">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="84242-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="84242-227">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-228">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="84242-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="84242-229">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="84242-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="84242-230">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="84242-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="84242-231">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="84242-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="84242-232">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="84242-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="84242-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-234">Boolean</span></span>|<span data-ttu-id="84242-235">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="84242-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="84242-236">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="84242-237">neutralDomainResources</span></span>|<span data-ttu-id="84242-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-239">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="84242-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="84242-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-241">Boolean</span></span>|<span data-ttu-id="84242-242">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="84242-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="84242-244">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="84242-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="84242-245">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="84242-246">isAssigned</span></span>|<span data-ttu-id="84242-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-247">Boolean</span></span>|<span data-ttu-id="84242-248">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="84242-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="84242-249">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="84242-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="84242-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="84242-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="84242-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-251">Boolean</span></span>|<span data-ttu-id="84242-252">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="84242-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="84242-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="84242-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="84242-254">String</span><span class="sxs-lookup"><span data-stu-id="84242-254">String</span></span>|<span data-ttu-id="84242-255">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="84242-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="84242-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="84242-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="84242-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="84242-257">Boolean</span></span>|<span data-ttu-id="84242-258">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="84242-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="84242-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84242-259">pinMinimumLength</span></span>|<span data-ttu-id="84242-260">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-260">Int32</span></span>|<span data-ttu-id="84242-261">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="84242-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="84242-262">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="84242-262">Default value is 4.</span></span> <span data-ttu-id="84242-263">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="84242-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="84242-264">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="84242-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="84242-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="84242-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="84242-266">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="84242-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84242-267">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="84242-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84242-268">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="84242-268">Default is NotAllow.</span></span> <span data-ttu-id="84242-269">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="84242-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="84242-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="84242-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="84242-271">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="84242-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84242-272">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="84242-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84242-273">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="84242-273">Default is NotAllow.</span></span> <span data-ttu-id="84242-274">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="84242-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="84242-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="84242-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="84242-276">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="84242-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="84242-277">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="84242-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="84242-278">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="84242-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="84242-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="84242-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="84242-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="84242-280">/ : ; < = > ?</span></span><span data-ttu-id="84242-281"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: ` notAllow `, ` рекуиреатлеастоне `, ` allow ".</span><span class="sxs-lookup"><span data-stu-id="84242-281"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="84242-282">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84242-282">pinExpirationDays</span></span>|<span data-ttu-id="84242-283">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-283">Int32</span></span>|<span data-ttu-id="84242-284">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="84242-284">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="84242-285">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="84242-285">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="84242-286">до 0.</span><span class="sxs-lookup"><span data-stu-id="84242-286">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="84242-287">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="84242-287">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="84242-288">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="84242-288">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="84242-289">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="84242-289">Default is 0.</span></span>|
|<span data-ttu-id="84242-290">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="84242-290">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="84242-291">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-291">Int32</span></span>|<span data-ttu-id="84242-292">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="84242-292">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="84242-293">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="84242-293">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="84242-294">до 0.</span><span class="sxs-lookup"><span data-stu-id="84242-294">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="84242-295">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="84242-295">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="84242-296">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="84242-296">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="84242-297">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="84242-297">Default is 0.</span></span>|
|<span data-ttu-id="84242-298">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="84242-298">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="84242-299">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-299">Int32</span></span>|<span data-ttu-id="84242-300">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="84242-300">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="84242-301">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="84242-301">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="84242-302">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="84242-302">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="84242-303">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="84242-303">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="84242-304">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-304">Int32</span></span>|<span data-ttu-id="84242-305">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="84242-305">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="84242-306">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="84242-306">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="84242-307">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="84242-307">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="84242-308">Int32</span><span class="sxs-lookup"><span data-stu-id="84242-308">Int32</span></span>|<span data-ttu-id="84242-309">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях).</span><span class="sxs-lookup"><span data-stu-id="84242-309">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="84242-310">Отклик</span><span class="sxs-lookup"><span data-stu-id="84242-310">Response</span></span>
<span data-ttu-id="84242-311">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84242-311">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84242-312">Пример</span><span class="sxs-lookup"><span data-stu-id="84242-312">Example</span></span>

### <a name="request"></a><span data-ttu-id="84242-313">Запрос</span><span class="sxs-lookup"><span data-stu-id="84242-313">Request</span></span>
<span data-ttu-id="84242-314">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84242-314">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4365

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="84242-315">Отклик</span><span class="sxs-lookup"><span data-stu-id="84242-315">Response</span></span>
<span data-ttu-id="84242-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84242-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4537

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




