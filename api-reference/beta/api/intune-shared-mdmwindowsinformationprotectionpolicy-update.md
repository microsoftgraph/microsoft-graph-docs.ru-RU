---
title: Обновление объекта mdmWindowsInformationProtectionPolicy
description: Обновляет свойства объекта mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81d7a65d5422f51e305daacbf7df08770ad9c6fd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939734"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="d6d7a-103">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d6d7a-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="d6d7a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d7a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d7a-106">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-106">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d7a-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="d6d7a-107">Prerequisites</span></span>
<span data-ttu-id="d6d7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d7a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6d7a-110">Permission type</span></span>|<span data-ttu-id="d6d7a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d7a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d6d7a-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d6d7a-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="d6d7a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d7a-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d6d7a-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d6d7a-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d6d7a-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d7a-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d6d7a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d7a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-118">Not supported.</span></span>|
|<span data-ttu-id="d6d7a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6d7a-119">Application</span></span>||
| <span data-ttu-id="d6d7a-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d6d7a-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="d6d7a-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d7a-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d6d7a-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d6d7a-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d6d7a-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d7a-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d7a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6d7a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d6d7a-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6d7a-125">Request headers</span></span>
|<span data-ttu-id="d6d7a-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6d7a-126">Header</span></span>|<span data-ttu-id="d6d7a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d6d7a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d7a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6d7a-128">Authorization</span></span>|<span data-ttu-id="d6d7a-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d7a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="d6d7a-130">Accept</span></span>|<span data-ttu-id="d6d7a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d7a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d7a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6d7a-132">Request body</span></span>
<span data-ttu-id="d6d7a-133">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-133">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="d6d7a-134">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-134">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="d6d7a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6d7a-135">Property</span></span>|<span data-ttu-id="d6d7a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d6d7a-136">Type</span></span>|<span data-ttu-id="d6d7a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d6d7a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d7a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d6d7a-138">displayName</span></span>|<span data-ttu-id="d6d7a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d6d7a-139">String</span></span>|<span data-ttu-id="d6d7a-140">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-140">Policy display name.</span></span> <span data-ttu-id="d6d7a-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-142">description</span><span class="sxs-lookup"><span data-stu-id="d6d7a-142">description</span></span>|<span data-ttu-id="d6d7a-143">String</span><span class="sxs-lookup"><span data-stu-id="d6d7a-143">String</span></span>|<span data-ttu-id="d6d7a-144">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-144">The policy's description.</span></span> <span data-ttu-id="d6d7a-145">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d7a-146">createdDateTime</span></span>|<span data-ttu-id="d6d7a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d7a-147">DateTimeOffset</span></span>|<span data-ttu-id="d6d7a-148">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-148">The date and time the policy was created.</span></span> <span data-ttu-id="d6d7a-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d7a-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d6d7a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d7a-151">DateTimeOffset</span></span>|<span data-ttu-id="d6d7a-152">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-152">Last time the policy was modified.</span></span> <span data-ttu-id="d6d7a-153">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6d7a-154">roleScopeTagIds</span></span>|<span data-ttu-id="d6d7a-155">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6d7a-155">String collection</span></span>|<span data-ttu-id="d6d7a-156">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6d7a-157">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-158">id</span><span class="sxs-lookup"><span data-stu-id="d6d7a-158">id</span></span>|<span data-ttu-id="d6d7a-159">Строка</span><span class="sxs-lookup"><span data-stu-id="d6d7a-159">String</span></span>|<span data-ttu-id="d6d7a-160">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-160">Key of the entity.</span></span> <span data-ttu-id="d6d7a-161">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-162">version</span><span class="sxs-lookup"><span data-stu-id="d6d7a-162">version</span></span>|<span data-ttu-id="d6d7a-163">Строка</span><span class="sxs-lookup"><span data-stu-id="d6d7a-163">String</span></span>|<span data-ttu-id="d6d7a-164">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-164">Version of the entity.</span></span> <span data-ttu-id="d6d7a-165">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d6d7a-166">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d6d7a-166">enforcementLevel</span></span>|[<span data-ttu-id="d6d7a-167">виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="d6d7a-167">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="d6d7a-168">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-168">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="d6d7a-169">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-169">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="d6d7a-170">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="d6d7a-170">enterpriseDomain</span></span>|<span data-ttu-id="d6d7a-171">String</span><span class="sxs-lookup"><span data-stu-id="d6d7a-171">String</span></span>|<span data-ttu-id="d6d7a-172">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-172">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-173">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="d6d7a-173">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="d6d7a-174">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-174">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-175">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-175">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-176">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="d6d7a-176">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="d6d7a-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-177">Boolean</span></span>|<span data-ttu-id="d6d7a-178">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-178">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-179">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d6d7a-179">dataRecoveryCertificate</span></span>|[<span data-ttu-id="d6d7a-180">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d6d7a-180">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="d6d7a-181">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-181">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="d6d7a-182">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-182">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-183">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="d6d7a-183">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="d6d7a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-184">Boolean</span></span>|<span data-ttu-id="d6d7a-185">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-185">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="d6d7a-186">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-186">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="d6d7a-187">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-187">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="d6d7a-188">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-188">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-189">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="d6d7a-189">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="d6d7a-190">Guid</span><span class="sxs-lookup"><span data-stu-id="d6d7a-190">Guid</span></span>|<span data-ttu-id="d6d7a-191">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-191">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="d6d7a-192">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-192">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-193">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="d6d7a-193">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="d6d7a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-194">Boolean</span></span>|<span data-ttu-id="d6d7a-195">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-195">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-196">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="d6d7a-196">iconsVisible</span></span>|<span data-ttu-id="d6d7a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-197">Boolean</span></span>|<span data-ttu-id="d6d7a-198">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="d6d7a-198">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="d6d7a-199">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-199">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-200">protectedApps</span><span class="sxs-lookup"><span data-stu-id="d6d7a-200">protectedApps</span></span>|<span data-ttu-id="d6d7a-201">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-201">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d6d7a-202">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-202">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-203">exemptApps</span><span class="sxs-lookup"><span data-stu-id="d6d7a-203">exemptApps</span></span>|<span data-ttu-id="d6d7a-204">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-204">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d6d7a-205">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-205">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="d6d7a-206">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-206">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="d6d7a-207">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-207">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-208">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="d6d7a-208">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="d6d7a-209">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-210">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-210">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="d6d7a-211">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-211">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-212">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d6d7a-212">enterpriseProxiedDomains</span></span>|<span data-ttu-id="d6d7a-213">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-213">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="d6d7a-214">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-214">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="d6d7a-215">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-215">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="d6d7a-216">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-216">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="d6d7a-217">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-217">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-218">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="d6d7a-218">enterpriseIPRanges</span></span>|<span data-ttu-id="d6d7a-219">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-219">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-220">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-220">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="d6d7a-221">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-221">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="d6d7a-222">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-222">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-223">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d6d7a-223">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="d6d7a-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-224">Boolean</span></span>|<span data-ttu-id="d6d7a-225">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-225">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="d6d7a-226">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-226">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-227">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="d6d7a-227">enterpriseProxyServers</span></span>|<span data-ttu-id="d6d7a-228">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-228">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-229">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-229">This is a list of proxy servers.</span></span> <span data-ttu-id="d6d7a-230">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-230">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-231">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="d6d7a-231">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="d6d7a-232">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-233">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="d6d7a-233">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="d6d7a-234">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="d6d7a-234">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="d6d7a-235">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-235">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="d6d7a-236">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-236">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="d6d7a-237">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-237">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-238">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d6d7a-238">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="d6d7a-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-239">Boolean</span></span>|<span data-ttu-id="d6d7a-240">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-240">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="d6d7a-241">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-241">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-242">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="d6d7a-242">neutralDomainResources</span></span>|<span data-ttu-id="d6d7a-243">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-244">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-244">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-245">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="d6d7a-245">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="d6d7a-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d7a-246">Boolean</span></span>|<span data-ttu-id="d6d7a-247">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-247">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-248">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="d6d7a-248">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="d6d7a-249">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d6d7a-249">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d6d7a-250">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-250">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d6d7a-251">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d6d7a-251">isAssigned</span></span>|<span data-ttu-id="d6d7a-252">Логический</span><span class="sxs-lookup"><span data-stu-id="d6d7a-252">Boolean</span></span>|<span data-ttu-id="d6d7a-253">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-253">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d6d7a-254">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d6d7a-254">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6d7a-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6d7a-255">Response</span></span>
<span data-ttu-id="d6d7a-256">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-256">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d7a-257">Пример</span><span class="sxs-lookup"><span data-stu-id="d6d7a-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d7a-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6d7a-258">Request</span></span>
<span data-ttu-id="d6d7a-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3967

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="d6d7a-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6d7a-260">Response</span></span>
<span data-ttu-id="d6d7a-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6d7a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4139

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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
  "isAssigned": true
}
```








