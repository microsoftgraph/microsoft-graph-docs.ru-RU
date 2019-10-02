---
title: Обновление объекта windowsInformationProtectionPolicy
description: Обновление свойств объекта windowsInformationProtectionPolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6ba66c2ca065785ef8ddf70319daec45b3e7557
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362928"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="0075e-103">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0075e-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="0075e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0075e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0075e-105">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-105">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0075e-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0075e-106">Prerequisites</span></span>
<span data-ttu-id="0075e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0075e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0075e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0075e-109">Permission type</span></span>|<span data-ttu-id="0075e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0075e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0075e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0075e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0075e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0075e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0075e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0075e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0075e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0075e-114">Not supported.</span></span>|
|<span data-ttu-id="0075e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0075e-115">Application</span></span>|<span data-ttu-id="0075e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0075e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0075e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0075e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0075e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0075e-118">Request headers</span></span>
|<span data-ttu-id="0075e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0075e-119">Header</span></span>|<span data-ttu-id="0075e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0075e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0075e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0075e-121">Authorization</span></span>|<span data-ttu-id="0075e-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0075e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0075e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0075e-123">Accept</span></span>|<span data-ttu-id="0075e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0075e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0075e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0075e-125">Request body</span></span>
<span data-ttu-id="0075e-126">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0075e-126">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="0075e-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-127">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="0075e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0075e-128">Property</span></span>|<span data-ttu-id="0075e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0075e-129">Type</span></span>|<span data-ttu-id="0075e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0075e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0075e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0075e-131">displayName</span></span>|<span data-ttu-id="0075e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0075e-132">String</span></span>|<span data-ttu-id="0075e-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0075e-133">Policy display name.</span></span> <span data-ttu-id="0075e-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-135">description</span><span class="sxs-lookup"><span data-stu-id="0075e-135">description</span></span>|<span data-ttu-id="0075e-136">String</span><span class="sxs-lookup"><span data-stu-id="0075e-136">String</span></span>|<span data-ttu-id="0075e-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0075e-137">The policy's description.</span></span> <span data-ttu-id="0075e-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0075e-139">createdDateTime</span></span>|<span data-ttu-id="0075e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0075e-140">DateTimeOffset</span></span>|<span data-ttu-id="0075e-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0075e-141">The date and time the policy was created.</span></span> <span data-ttu-id="0075e-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0075e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="0075e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0075e-144">DateTimeOffset</span></span>|<span data-ttu-id="0075e-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0075e-145">Last time the policy was modified.</span></span> <span data-ttu-id="0075e-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-147">id</span><span class="sxs-lookup"><span data-stu-id="0075e-147">id</span></span>|<span data-ttu-id="0075e-148">String</span><span class="sxs-lookup"><span data-stu-id="0075e-148">String</span></span>|<span data-ttu-id="0075e-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0075e-149">Key of the entity.</span></span> <span data-ttu-id="0075e-150">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-151">version</span><span class="sxs-lookup"><span data-stu-id="0075e-151">version</span></span>|<span data-ttu-id="0075e-152">String</span><span class="sxs-lookup"><span data-stu-id="0075e-152">String</span></span>|<span data-ttu-id="0075e-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0075e-153">Version of the entity.</span></span> <span data-ttu-id="0075e-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0075e-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="0075e-155">enforcementLevel</span></span>|[<span data-ttu-id="0075e-156">виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="0075e-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="0075e-157">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="0075e-158">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="0075e-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="0075e-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="0075e-159">enterpriseDomain</span></span>|<span data-ttu-id="0075e-160">String</span><span class="sxs-lookup"><span data-stu-id="0075e-160">String</span></span>|<span data-ttu-id="0075e-161">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="0075e-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="0075e-163">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-164">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="0075e-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="0075e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-166">Boolean</span></span>|<span data-ttu-id="0075e-167">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0075e-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="0075e-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0075e-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="0075e-170">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="0075e-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="0075e-171">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="0075e-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="0075e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-173">Boolean</span></span>|<span data-ttu-id="0075e-174">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="0075e-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="0075e-175">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="0075e-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="0075e-176">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="0075e-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="0075e-177">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="0075e-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="0075e-179">Guid</span><span class="sxs-lookup"><span data-stu-id="0075e-179">Guid</span></span>|<span data-ttu-id="0075e-180">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="0075e-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="0075e-181">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="0075e-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="0075e-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-183">Boolean</span></span>|<span data-ttu-id="0075e-184">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="0075e-185">iconsVisible</span></span>|<span data-ttu-id="0075e-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-186">Boolean</span></span>|<span data-ttu-id="0075e-187">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="0075e-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="0075e-188">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="0075e-189">protectedApps</span></span>|<span data-ttu-id="0075e-190">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0075e-191">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="0075e-192">exemptApps</span></span>|<span data-ttu-id="0075e-193">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0075e-194">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="0075e-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="0075e-195">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="0075e-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="0075e-196">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="0075e-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="0075e-198">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-199">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="0075e-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="0075e-200">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="0075e-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="0075e-202">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="0075e-203">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="0075e-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="0075e-204">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="0075e-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="0075e-205">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="0075e-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="0075e-206">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="0075e-207">enterpriseIPRanges</span></span>|<span data-ttu-id="0075e-208">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="0075e-209">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="0075e-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="0075e-210">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="0075e-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="0075e-211">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0075e-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="0075e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-213">Boolean</span></span>|<span data-ttu-id="0075e-214">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="0075e-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="0075e-215">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="0075e-216">enterpriseProxyServers</span></span>|<span data-ttu-id="0075e-217">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-218">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="0075e-218">This is a list of proxy servers.</span></span> <span data-ttu-id="0075e-219">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="0075e-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="0075e-221">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-222">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="0075e-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="0075e-223">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="0075e-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="0075e-224">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0075e-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="0075e-225">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="0075e-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="0075e-226">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0075e-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="0075e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-228">Boolean</span></span>|<span data-ttu-id="0075e-229">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="0075e-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="0075e-230">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="0075e-231">neutralDomainResources</span></span>|<span data-ttu-id="0075e-232">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-233">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="0075e-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="0075e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-235">Boolean</span></span>|<span data-ttu-id="0075e-236">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="0075e-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="0075e-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0075e-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0075e-239">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0075e-240">isAssigned</span></span>|<span data-ttu-id="0075e-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-241">Boolean</span></span>|<span data-ttu-id="0075e-242">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="0075e-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="0075e-243">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0075e-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0075e-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="0075e-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="0075e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-245">Boolean</span></span>|<span data-ttu-id="0075e-246">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="0075e-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="0075e-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="0075e-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="0075e-248">String</span><span class="sxs-lookup"><span data-stu-id="0075e-248">String</span></span>|<span data-ttu-id="0075e-249">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="0075e-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="0075e-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="0075e-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="0075e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="0075e-251">Boolean</span></span>|<span data-ttu-id="0075e-252">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="0075e-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="0075e-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0075e-253">pinMinimumLength</span></span>|<span data-ttu-id="0075e-254">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-254">Int32</span></span>|<span data-ttu-id="0075e-255">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="0075e-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="0075e-256">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="0075e-256">Default value is 4.</span></span> <span data-ttu-id="0075e-257">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="0075e-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="0075e-258">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="0075e-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="0075e-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="0075e-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="0075e-260">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="0075e-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="0075e-261">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0075e-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="0075e-262">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="0075e-262">Default is NotAllow.</span></span> <span data-ttu-id="0075e-263">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="0075e-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="0075e-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="0075e-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="0075e-265">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="0075e-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="0075e-266">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0075e-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="0075e-267">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="0075e-267">Default is NotAllow.</span></span> <span data-ttu-id="0075e-268">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="0075e-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="0075e-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="0075e-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="0075e-270">виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="0075e-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="0075e-271">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0075e-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="0075e-272">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="0075e-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="0075e-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="0075e-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="0075e-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="0075e-274">/ : ; < = > ?</span></span><span data-ttu-id="0075e-275"> @ \[ \ \]^ _ \` { | } ~.</span><span class="sxs-lookup"><span data-stu-id="0075e-275"> @ \[ \ \] ^ _ \` { | } ~.</span></span> <span data-ttu-id="0075e-276">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="0075e-276">Default is NotAllow.</span></span> <span data-ttu-id="0075e-277">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="0075e-277">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="0075e-278">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0075e-278">pinExpirationDays</span></span>|<span data-ttu-id="0075e-279">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-279">Int32</span></span>|<span data-ttu-id="0075e-280">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="0075e-280">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="0075e-281">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="0075e-281">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="0075e-282">до 0.</span><span class="sxs-lookup"><span data-stu-id="0075e-282">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="0075e-283">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="0075e-283">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="0075e-284">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="0075e-284">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="0075e-285">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="0075e-285">Default is 0.</span></span>|
|<span data-ttu-id="0075e-286">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="0075e-286">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="0075e-287">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-287">Int32</span></span>|<span data-ttu-id="0075e-288">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="0075e-288">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="0075e-289">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="0075e-289">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="0075e-290">до 0.</span><span class="sxs-lookup"><span data-stu-id="0075e-290">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="0075e-291">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="0075e-291">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="0075e-292">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="0075e-292">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="0075e-293">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="0075e-293">Default is 0.</span></span>|
|<span data-ttu-id="0075e-294">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="0075e-294">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="0075e-295">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-295">Int32</span></span>|<span data-ttu-id="0075e-296">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="0075e-296">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="0075e-297">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="0075e-297">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="0075e-298">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="0075e-298">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="0075e-299">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="0075e-299">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="0075e-300">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-300">Int32</span></span>|<span data-ttu-id="0075e-301">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="0075e-301">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="0075e-302">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="0075e-302">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="0075e-303">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="0075e-303">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="0075e-304">Int32</span><span class="sxs-lookup"><span data-stu-id="0075e-304">Int32</span></span>|<span data-ttu-id="0075e-305">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях).</span><span class="sxs-lookup"><span data-stu-id="0075e-305">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="0075e-306">Отклик</span><span class="sxs-lookup"><span data-stu-id="0075e-306">Response</span></span>
<span data-ttu-id="0075e-307">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0075e-307">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0075e-308">Пример</span><span class="sxs-lookup"><span data-stu-id="0075e-308">Example</span></span>

### <a name="request"></a><span data-ttu-id="0075e-309">Запрос</span><span class="sxs-lookup"><span data-stu-id="0075e-309">Request</span></span>
<span data-ttu-id="0075e-310">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0075e-310">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4405

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
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
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

### <a name="response"></a><span data-ttu-id="0075e-311">Отклик</span><span class="sxs-lookup"><span data-stu-id="0075e-311">Response</span></span>
<span data-ttu-id="0075e-p130">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0075e-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4577

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
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
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




