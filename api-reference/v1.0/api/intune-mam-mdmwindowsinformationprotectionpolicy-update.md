---
title: Обновление объекта mdmWindowsInformationProtectionPolicy
description: Обновляет свойства объекта mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c72208750cbc23c1dc8633af98a276622bc16194
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745438"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="0c34d-103">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0c34d-103">Update mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="0c34d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c34d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c34d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c34d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c34d-106">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-106">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c34d-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="0c34d-107">Prerequisites</span></span>
<span data-ttu-id="0c34d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c34d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c34d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c34d-110">Permission type</span></span>|<span data-ttu-id="0c34d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c34d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c34d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c34d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c34d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c34d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c34d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c34d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c34d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c34d-115">Not supported.</span></span>|
|<span data-ttu-id="0c34d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c34d-116">Application</span></span>|<span data-ttu-id="0c34d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c34d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c34d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c34d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0c34d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c34d-119">Request headers</span></span>
|<span data-ttu-id="0c34d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c34d-120">Header</span></span>|<span data-ttu-id="0c34d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c34d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c34d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c34d-122">Authorization</span></span>|<span data-ttu-id="0c34d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c34d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c34d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c34d-124">Accept</span></span>|<span data-ttu-id="0c34d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c34d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c34d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c34d-126">Request body</span></span>
<span data-ttu-id="0c34d-127">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c34d-127">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="0c34d-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-128">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="0c34d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c34d-129">Property</span></span>|<span data-ttu-id="0c34d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c34d-130">Type</span></span>|<span data-ttu-id="0c34d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c34d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c34d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0c34d-132">displayName</span></span>|<span data-ttu-id="0c34d-133">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-133">String</span></span>|<span data-ttu-id="0c34d-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0c34d-134">Policy display name.</span></span> <span data-ttu-id="0c34d-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-136">description</span><span class="sxs-lookup"><span data-stu-id="0c34d-136">description</span></span>|<span data-ttu-id="0c34d-137">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-137">String</span></span>|<span data-ttu-id="0c34d-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0c34d-138">The policy's description.</span></span> <span data-ttu-id="0c34d-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c34d-140">createdDateTime</span></span>|<span data-ttu-id="0c34d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c34d-141">DateTimeOffset</span></span>|<span data-ttu-id="0c34d-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0c34d-142">The date and time the policy was created.</span></span> <span data-ttu-id="0c34d-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c34d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0c34d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c34d-145">DateTimeOffset</span></span>|<span data-ttu-id="0c34d-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0c34d-146">Last time the policy was modified.</span></span> <span data-ttu-id="0c34d-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-148">id</span><span class="sxs-lookup"><span data-stu-id="0c34d-148">id</span></span>|<span data-ttu-id="0c34d-149">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-149">String</span></span>|<span data-ttu-id="0c34d-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c34d-150">Key of the entity.</span></span> <span data-ttu-id="0c34d-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-152">version</span><span class="sxs-lookup"><span data-stu-id="0c34d-152">version</span></span>|<span data-ttu-id="0c34d-153">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-153">String</span></span>|<span data-ttu-id="0c34d-154">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0c34d-154">Version of the entity.</span></span> <span data-ttu-id="0c34d-155">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0c34d-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="0c34d-156">enforcementLevel</span></span>|[<span data-ttu-id="0c34d-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="0c34d-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="0c34d-158">Уровень правоприменения WIP. См. определение Enum для поддерживаемых значений, унаследованных от [windowsInformationProtection.](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="0c34d-159">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="0c34d-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="0c34d-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="0c34d-160">enterpriseDomain</span></span>|<span data-ttu-id="0c34d-161">String</span><span class="sxs-lookup"><span data-stu-id="0c34d-161">String</span></span>|<span data-ttu-id="0c34d-162">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="0c34d-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="0c34d-164">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-165">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="0c34d-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="0c34d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-167">Boolean</span></span>|<span data-ttu-id="0c34d-168">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0c34d-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="0c34d-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0c34d-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="0c34d-171">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="0c34d-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="0c34d-172">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="0c34d-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="0c34d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-174">Boolean</span></span>|<span data-ttu-id="0c34d-175">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="0c34d-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="0c34d-176">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="0c34d-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="0c34d-177">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="0c34d-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="0c34d-178">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="0c34d-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="0c34d-180">Guid</span><span class="sxs-lookup"><span data-stu-id="0c34d-180">Guid</span></span>|<span data-ttu-id="0c34d-181">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="0c34d-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="0c34d-182">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="0c34d-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="0c34d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-184">Boolean</span></span>|<span data-ttu-id="0c34d-185">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="0c34d-186">iconsVisible</span></span>|<span data-ttu-id="0c34d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-187">Boolean</span></span>|<span data-ttu-id="0c34d-188">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="0c34d-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="0c34d-189">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="0c34d-190">protectedApps</span></span>|<span data-ttu-id="0c34d-191">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0c34d-192">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="0c34d-193">exemptApps</span></span>|<span data-ttu-id="0c34d-194">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0c34d-195">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="0c34d-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="0c34d-196">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="0c34d-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="0c34d-197">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="0c34d-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="0c34d-199">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-200">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="0c34d-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="0c34d-201">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="0c34d-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="0c34d-203">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="0c34d-204">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="0c34d-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="0c34d-205">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="0c34d-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="0c34d-206">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="0c34d-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="0c34d-207">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="0c34d-208">enterpriseIPRanges</span></span>|<span data-ttu-id="0c34d-209">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="0c34d-210">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="0c34d-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="0c34d-211">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="0c34d-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="0c34d-212">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0c34d-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="0c34d-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-214">Boolean</span></span>|<span data-ttu-id="0c34d-215">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="0c34d-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="0c34d-216">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="0c34d-217">enterpriseProxyServers</span></span>|<span data-ttu-id="0c34d-218">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-219">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="0c34d-219">This is a list of proxy servers.</span></span> <span data-ttu-id="0c34d-220">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="0c34d-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="0c34d-222">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-223">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="0c34d-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="0c34d-224">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="0c34d-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="0c34d-225">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0c34d-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="0c34d-226">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="0c34d-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="0c34d-227">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0c34d-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="0c34d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-229">Boolean</span></span>|<span data-ttu-id="0c34d-230">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="0c34d-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="0c34d-231">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="0c34d-232">neutralDomainResources</span></span>|<span data-ttu-id="0c34d-233">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-234">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="0c34d-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="0c34d-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-236">Boolean</span></span>|<span data-ttu-id="0c34d-237">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="0c34d-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="0c34d-239">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0c34d-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0c34d-240">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0c34d-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0c34d-241">isAssigned</span></span>|<span data-ttu-id="0c34d-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c34d-242">Boolean</span></span>|<span data-ttu-id="0c34d-243">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="0c34d-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="0c34d-244">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c34d-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0c34d-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c34d-245">Response</span></span>
<span data-ttu-id="0c34d-246">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c34d-246">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c34d-247">Пример</span><span class="sxs-lookup"><span data-stu-id="0c34d-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c34d-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c34d-248">Request</span></span>
<span data-ttu-id="0c34d-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c34d-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="0c34d-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c34d-250">Response</span></span>
<span data-ttu-id="0c34d-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c34d-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




