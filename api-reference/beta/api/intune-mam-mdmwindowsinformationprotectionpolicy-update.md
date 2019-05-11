---
title: Обновление объекта mdmWindowsInformationProtectionPolicy
description: Обновляет свойства объекта mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a86440f68f9fb2c7d2c8a1faf4b2113c925e7e37
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902915"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="b5668-103">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b5668-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="b5668-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5668-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5668-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5668-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5668-106">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-106">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5668-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="b5668-107">Prerequisites</span></span>
<span data-ttu-id="b5668-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5668-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5668-110">Permission type</span></span>|<span data-ttu-id="b5668-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5668-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5668-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5668-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5668-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5668-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5668-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5668-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5668-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5668-115">Not supported.</span></span>|
|<span data-ttu-id="b5668-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5668-116">Application</span></span>|<span data-ttu-id="b5668-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5668-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5668-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5668-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b5668-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5668-119">Request headers</span></span>
|<span data-ttu-id="b5668-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5668-120">Header</span></span>|<span data-ttu-id="b5668-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5668-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5668-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5668-122">Authorization</span></span>|<span data-ttu-id="b5668-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5668-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5668-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5668-124">Accept</span></span>|<span data-ttu-id="b5668-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5668-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5668-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5668-126">Request body</span></span>
<span data-ttu-id="b5668-127">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5668-127">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="b5668-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-128">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="b5668-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5668-129">Property</span></span>|<span data-ttu-id="b5668-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5668-130">Type</span></span>|<span data-ttu-id="b5668-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5668-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5668-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b5668-132">displayName</span></span>|<span data-ttu-id="b5668-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b5668-133">String</span></span>|<span data-ttu-id="b5668-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="b5668-134">Policy display name.</span></span> <span data-ttu-id="b5668-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-136">description</span><span class="sxs-lookup"><span data-stu-id="b5668-136">description</span></span>|<span data-ttu-id="b5668-137">String</span><span class="sxs-lookup"><span data-stu-id="b5668-137">String</span></span>|<span data-ttu-id="b5668-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="b5668-138">The policy's description.</span></span> <span data-ttu-id="b5668-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5668-140">createdDateTime</span></span>|<span data-ttu-id="b5668-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5668-141">DateTimeOffset</span></span>|<span data-ttu-id="b5668-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="b5668-142">The date and time the policy was created.</span></span> <span data-ttu-id="b5668-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5668-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b5668-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5668-145">DateTimeOffset</span></span>|<span data-ttu-id="b5668-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="b5668-146">Last time the policy was modified.</span></span> <span data-ttu-id="b5668-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5668-148">roleScopeTagIds</span></span>|<span data-ttu-id="b5668-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5668-149">String collection</span></span>|<span data-ttu-id="b5668-150">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b5668-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5668-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-152">id</span><span class="sxs-lookup"><span data-stu-id="b5668-152">id</span></span>|<span data-ttu-id="b5668-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b5668-153">String</span></span>|<span data-ttu-id="b5668-154">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b5668-154">Key of the entity.</span></span> <span data-ttu-id="b5668-155">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-156">version</span><span class="sxs-lookup"><span data-stu-id="b5668-156">version</span></span>|<span data-ttu-id="b5668-157">Строка</span><span class="sxs-lookup"><span data-stu-id="b5668-157">String</span></span>|<span data-ttu-id="b5668-158">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="b5668-158">Version of the entity.</span></span> <span data-ttu-id="b5668-159">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b5668-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b5668-160">enforcementLevel</span></span>|[<span data-ttu-id="b5668-161">Виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="b5668-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="b5668-162">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="b5668-163">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="b5668-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="b5668-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="b5668-164">enterpriseDomain</span></span>|<span data-ttu-id="b5668-165">String</span><span class="sxs-lookup"><span data-stu-id="b5668-165">String</span></span>|<span data-ttu-id="b5668-166">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="b5668-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="b5668-168">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-169">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="b5668-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="b5668-171">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-171">Boolean</span></span>|<span data-ttu-id="b5668-172">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b5668-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="b5668-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b5668-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="b5668-175">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="b5668-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="b5668-176">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="b5668-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="b5668-178">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-178">Boolean</span></span>|<span data-ttu-id="b5668-179">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="b5668-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="b5668-180">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="b5668-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="b5668-181">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="b5668-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="b5668-182">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="b5668-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="b5668-184">Guid</span><span class="sxs-lookup"><span data-stu-id="b5668-184">Guid</span></span>|<span data-ttu-id="b5668-185">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="b5668-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="b5668-186">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="b5668-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="b5668-188">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-188">Boolean</span></span>|<span data-ttu-id="b5668-189">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="b5668-190">iconsVisible</span></span>|<span data-ttu-id="b5668-191">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-191">Boolean</span></span>|<span data-ttu-id="b5668-192">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="b5668-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="b5668-193">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="b5668-194">protectedApps</span></span>|<span data-ttu-id="b5668-195">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b5668-196">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="b5668-197">exemptApps</span></span>|<span data-ttu-id="b5668-198">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b5668-199">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="b5668-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="b5668-200">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="b5668-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="b5668-201">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="b5668-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="b5668-203">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-204">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="b5668-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="b5668-205">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="b5668-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="b5668-207">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="b5668-208">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="b5668-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="b5668-209">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="b5668-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="b5668-210">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="b5668-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="b5668-211">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="b5668-212">enterpriseIPRanges</span></span>|<span data-ttu-id="b5668-213">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="b5668-214">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="b5668-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="b5668-215">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="b5668-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="b5668-216">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b5668-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="b5668-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5668-218">Boolean</span></span>|<span data-ttu-id="b5668-219">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="b5668-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="b5668-220">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="b5668-221">enterpriseProxyServers</span></span>|<span data-ttu-id="b5668-222">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-223">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="b5668-223">This is a list of proxy servers.</span></span> <span data-ttu-id="b5668-224">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="b5668-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="b5668-226">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-227">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="b5668-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="b5668-228">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="b5668-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="b5668-229">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b5668-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="b5668-230">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="b5668-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="b5668-231">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b5668-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="b5668-233">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-233">Boolean</span></span>|<span data-ttu-id="b5668-234">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="b5668-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="b5668-235">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="b5668-236">neutralDomainResources</span></span>|<span data-ttu-id="b5668-237">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-238">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="b5668-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="b5668-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5668-240">Boolean</span></span>|<span data-ttu-id="b5668-241">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="b5668-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="b5668-243">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b5668-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b5668-244">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b5668-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b5668-245">isAssigned</span></span>|<span data-ttu-id="b5668-246">Логический</span><span class="sxs-lookup"><span data-stu-id="b5668-246">Boolean</span></span>|<span data-ttu-id="b5668-247">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="b5668-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="b5668-248">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b5668-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b5668-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5668-249">Response</span></span>
<span data-ttu-id="b5668-250">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b5668-250">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5668-251">Пример</span><span class="sxs-lookup"><span data-stu-id="b5668-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5668-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5668-252">Request</span></span>
<span data-ttu-id="b5668-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5668-253">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5668-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5668-254">Response</span></span>
<span data-ttu-id="b5668-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5668-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




