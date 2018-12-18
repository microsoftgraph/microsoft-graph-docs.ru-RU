---
title: Обновление объекта mdmWindowsInformationProtectionPolicy
description: Обновление свойств объекта mdmWindowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: 2449409b4dfd7d18efcfe961ad65d44a2e9c48bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346762"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="7cfac-103">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7cfac-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="7cfac-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7cfac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cfac-105">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-105">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cfac-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="7cfac-106">Prerequisites</span></span>
<span data-ttu-id="7cfac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cfac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cfac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cfac-109">Permission type</span></span>|<span data-ttu-id="7cfac-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cfac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cfac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cfac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cfac-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cfac-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cfac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cfac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cfac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cfac-114">Not supported.</span></span>|
|<span data-ttu-id="7cfac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cfac-115">Application</span></span>|<span data-ttu-id="7cfac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cfac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cfac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cfac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7cfac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cfac-118">Request headers</span></span>
|<span data-ttu-id="7cfac-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cfac-119">Header</span></span>|<span data-ttu-id="7cfac-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7cfac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cfac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cfac-121">Authorization</span></span>|<span data-ttu-id="7cfac-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7cfac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cfac-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7cfac-123">Accept</span></span>|<span data-ttu-id="7cfac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cfac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cfac-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cfac-125">Request body</span></span>
<span data-ttu-id="7cfac-126">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cfac-126">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="7cfac-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-127">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="7cfac-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cfac-128">Property</span></span>|<span data-ttu-id="7cfac-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7cfac-129">Type</span></span>|<span data-ttu-id="7cfac-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7cfac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cfac-131">displayName</span><span class="sxs-lookup"><span data-stu-id="7cfac-131">displayName</span></span>|<span data-ttu-id="7cfac-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7cfac-132">String</span></span>|<span data-ttu-id="7cfac-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="7cfac-133">Policy display name.</span></span> <span data-ttu-id="7cfac-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-135">описание</span><span class="sxs-lookup"><span data-stu-id="7cfac-135">description</span></span>|<span data-ttu-id="7cfac-136">Строка</span><span class="sxs-lookup"><span data-stu-id="7cfac-136">String</span></span>|<span data-ttu-id="7cfac-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="7cfac-137">The policy's description.</span></span> <span data-ttu-id="7cfac-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cfac-139">createdDateTime</span></span>|<span data-ttu-id="7cfac-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cfac-140">DateTimeOffset</span></span>|<span data-ttu-id="7cfac-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="7cfac-141">The date and time the policy was created.</span></span> <span data-ttu-id="7cfac-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cfac-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7cfac-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cfac-144">DateTimeOffset</span></span>|<span data-ttu-id="7cfac-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="7cfac-145">Last time the policy was modified.</span></span> <span data-ttu-id="7cfac-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-147">id</span><span class="sxs-lookup"><span data-stu-id="7cfac-147">id</span></span>|<span data-ttu-id="7cfac-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7cfac-148">String</span></span>|<span data-ttu-id="7cfac-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7cfac-149">Key of the entity.</span></span> <span data-ttu-id="7cfac-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-151">version</span><span class="sxs-lookup"><span data-stu-id="7cfac-151">version</span></span>|<span data-ttu-id="7cfac-152">Строка</span><span class="sxs-lookup"><span data-stu-id="7cfac-152">String</span></span>|<span data-ttu-id="7cfac-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="7cfac-153">Version of the entity.</span></span> <span data-ttu-id="7cfac-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7cfac-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="7cfac-155">enforcementLevel</span></span>|[<span data-ttu-id="7cfac-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="7cfac-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="7cfac-157">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="7cfac-158">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="7cfac-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="7cfac-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="7cfac-159">enterpriseDomain</span></span>|<span data-ttu-id="7cfac-160">Строка</span><span class="sxs-lookup"><span data-stu-id="7cfac-160">String</span></span>|<span data-ttu-id="7cfac-161">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="7cfac-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="7cfac-163">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-164">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="7cfac-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="7cfac-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-166">Boolean</span></span>|<span data-ttu-id="7cfac-167">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="7cfac-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="7cfac-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="7cfac-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="7cfac-170">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="7cfac-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="7cfac-171">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="7cfac-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="7cfac-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-173">Boolean</span></span>|<span data-ttu-id="7cfac-174">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="7cfac-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="7cfac-175">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="7cfac-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="7cfac-176">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="7cfac-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="7cfac-177">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="7cfac-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="7cfac-179">Guid</span><span class="sxs-lookup"><span data-stu-id="7cfac-179">Guid</span></span>|<span data-ttu-id="7cfac-180">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="7cfac-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="7cfac-181">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="7cfac-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="7cfac-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-183">Boolean</span></span>|<span data-ttu-id="7cfac-184">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="7cfac-185">iconsVisible</span></span>|<span data-ttu-id="7cfac-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-186">Boolean</span></span>|<span data-ttu-id="7cfac-187">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="7cfac-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="7cfac-188">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="7cfac-189">protectedApps</span></span>|<span data-ttu-id="7cfac-190">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="7cfac-191">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="7cfac-192">exemptApps</span></span>|<span data-ttu-id="7cfac-193">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="7cfac-194">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="7cfac-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="7cfac-195">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="7cfac-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="7cfac-196">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="7cfac-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="7cfac-198">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-199">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="7cfac-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="7cfac-200">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="7cfac-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="7cfac-202">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="7cfac-203">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="7cfac-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="7cfac-204">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="7cfac-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="7cfac-205">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="7cfac-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="7cfac-206">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="7cfac-207">enterpriseIPRanges</span></span>|<span data-ttu-id="7cfac-208">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="7cfac-209">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="7cfac-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="7cfac-210">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="7cfac-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="7cfac-211">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="7cfac-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="7cfac-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-213">Boolean</span></span>|<span data-ttu-id="7cfac-214">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="7cfac-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="7cfac-215">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="7cfac-216">enterpriseProxyServers</span></span>|<span data-ttu-id="7cfac-217">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-218">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="7cfac-218">This is a list of proxy servers.</span></span> <span data-ttu-id="7cfac-219">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="7cfac-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="7cfac-221">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-222">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="7cfac-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="7cfac-223">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="7cfac-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="7cfac-224">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="7cfac-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="7cfac-225">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="7cfac-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="7cfac-226">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="7cfac-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="7cfac-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-228">Boolean</span></span>|<span data-ttu-id="7cfac-229">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="7cfac-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="7cfac-230">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="7cfac-231">neutralDomainResources</span></span>|<span data-ttu-id="7cfac-232">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-233">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="7cfac-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="7cfac-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-235">Boolean</span></span>|<span data-ttu-id="7cfac-236">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="7cfac-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="7cfac-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7cfac-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7cfac-239">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7cfac-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7cfac-240">isAssigned</span></span>|<span data-ttu-id="7cfac-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfac-241">Boolean</span></span>|<span data-ttu-id="7cfac-242">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="7cfac-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="7cfac-243">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cfac-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7cfac-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cfac-244">Response</span></span>
<span data-ttu-id="7cfac-245">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7cfac-245">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cfac-246">Пример</span><span class="sxs-lookup"><span data-stu-id="7cfac-246">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cfac-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cfac-247">Request</span></span>
<span data-ttu-id="7cfac-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cfac-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7cfac-249">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cfac-249">Response</span></span>
<span data-ttu-id="7cfac-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7cfac-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



