---
title: Создание mdmWindowsInformationProtectionPolicy
description: Создание объекта mdmWindowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: 54f99110616f466e4a20188cf4a90b4ebfb9a3e7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349254"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="9f830-103">Создание mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9f830-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="9f830-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f830-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f830-105">Создание объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-105">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f830-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f830-106">Prerequisites</span></span>
<span data-ttu-id="9f830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f830-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f830-109">Permission type</span></span>|<span data-ttu-id="9f830-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f830-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f830-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f830-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f830-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f830-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f830-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f830-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f830-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f830-114">Not supported.</span></span>|
|<span data-ttu-id="9f830-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f830-115">Application</span></span>|<span data-ttu-id="9f830-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f830-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f830-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f830-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="9f830-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f830-118">Request headers</span></span>
|<span data-ttu-id="9f830-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f830-119">Header</span></span>|<span data-ttu-id="9f830-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9f830-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f830-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f830-121">Authorization</span></span>|<span data-ttu-id="9f830-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f830-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f830-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9f830-123">Accept</span></span>|<span data-ttu-id="9f830-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f830-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f830-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f830-125">Request body</span></span>
<span data-ttu-id="9f830-126">В теле запроса добавьте представление объекта mdmWindowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f830-126">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="9f830-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="9f830-127">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="9f830-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f830-128">Property</span></span>|<span data-ttu-id="9f830-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9f830-129">Type</span></span>|<span data-ttu-id="9f830-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9f830-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f830-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9f830-131">displayName</span></span>|<span data-ttu-id="9f830-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9f830-132">String</span></span>|<span data-ttu-id="9f830-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="9f830-133">Policy display name.</span></span> <span data-ttu-id="9f830-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-135">описание</span><span class="sxs-lookup"><span data-stu-id="9f830-135">description</span></span>|<span data-ttu-id="9f830-136">Строка</span><span class="sxs-lookup"><span data-stu-id="9f830-136">String</span></span>|<span data-ttu-id="9f830-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="9f830-137">The policy's description.</span></span> <span data-ttu-id="9f830-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f830-139">createdDateTime</span></span>|<span data-ttu-id="9f830-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f830-140">DateTimeOffset</span></span>|<span data-ttu-id="9f830-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="9f830-141">The date and time the policy was created.</span></span> <span data-ttu-id="9f830-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f830-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9f830-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f830-144">DateTimeOffset</span></span>|<span data-ttu-id="9f830-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="9f830-145">Last time the policy was modified.</span></span> <span data-ttu-id="9f830-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-147">id</span><span class="sxs-lookup"><span data-stu-id="9f830-147">id</span></span>|<span data-ttu-id="9f830-148">Строка</span><span class="sxs-lookup"><span data-stu-id="9f830-148">String</span></span>|<span data-ttu-id="9f830-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f830-149">Key of the entity.</span></span> <span data-ttu-id="9f830-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-151">version</span><span class="sxs-lookup"><span data-stu-id="9f830-151">version</span></span>|<span data-ttu-id="9f830-152">Строка</span><span class="sxs-lookup"><span data-stu-id="9f830-152">String</span></span>|<span data-ttu-id="9f830-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9f830-153">Version of the entity.</span></span> <span data-ttu-id="9f830-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9f830-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9f830-155">enforcementLevel</span></span>|[<span data-ttu-id="9f830-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9f830-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="9f830-157">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="9f830-158">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="9f830-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="9f830-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="9f830-159">enterpriseDomain</span></span>|<span data-ttu-id="9f830-160">Строка</span><span class="sxs-lookup"><span data-stu-id="9f830-160">String</span></span>|<span data-ttu-id="9f830-161">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="9f830-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="9f830-163">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-164">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="9f830-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="9f830-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-166">Boolean</span></span>|<span data-ttu-id="9f830-167">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9f830-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="9f830-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9f830-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="9f830-170">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="9f830-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="9f830-171">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="9f830-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="9f830-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-173">Boolean</span></span>|<span data-ttu-id="9f830-174">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="9f830-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="9f830-175">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="9f830-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="9f830-176">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="9f830-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="9f830-177">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="9f830-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="9f830-179">Guid</span><span class="sxs-lookup"><span data-stu-id="9f830-179">Guid</span></span>|<span data-ttu-id="9f830-180">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="9f830-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="9f830-181">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="9f830-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="9f830-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-183">Boolean</span></span>|<span data-ttu-id="9f830-184">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="9f830-185">iconsVisible</span></span>|<span data-ttu-id="9f830-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-186">Boolean</span></span>|<span data-ttu-id="9f830-187">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="9f830-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="9f830-188">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="9f830-189">protectedApps</span></span>|<span data-ttu-id="9f830-190">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9f830-191">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="9f830-192">exemptApps</span></span>|<span data-ttu-id="9f830-193">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9f830-194">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="9f830-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="9f830-195">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="9f830-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="9f830-196">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="9f830-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="9f830-198">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-199">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="9f830-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="9f830-200">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="9f830-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="9f830-202">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="9f830-203">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="9f830-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="9f830-204">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="9f830-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="9f830-205">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="9f830-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="9f830-206">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="9f830-207">enterpriseIPRanges</span></span>|<span data-ttu-id="9f830-208">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="9f830-209">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="9f830-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="9f830-210">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="9f830-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="9f830-211">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9f830-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="9f830-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-213">Boolean</span></span>|<span data-ttu-id="9f830-214">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="9f830-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="9f830-215">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="9f830-216">enterpriseProxyServers</span></span>|<span data-ttu-id="9f830-217">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-218">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="9f830-218">This is a list of proxy servers.</span></span> <span data-ttu-id="9f830-219">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9f830-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="9f830-221">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-222">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="9f830-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="9f830-223">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="9f830-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="9f830-224">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9f830-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="9f830-225">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="9f830-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="9f830-226">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9f830-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="9f830-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-228">Boolean</span></span>|<span data-ttu-id="9f830-229">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="9f830-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="9f830-230">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="9f830-231">neutralDomainResources</span></span>|<span data-ttu-id="9f830-232">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-233">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="9f830-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="9f830-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-235">Boolean</span></span>|<span data-ttu-id="9f830-236">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="9f830-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="9f830-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9f830-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9f830-239">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9f830-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9f830-240">isAssigned</span></span>|<span data-ttu-id="9f830-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f830-241">Boolean</span></span>|<span data-ttu-id="9f830-242">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="9f830-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="9f830-243">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9f830-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9f830-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f830-244">Response</span></span>
<span data-ttu-id="9f830-245">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f830-245">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f830-246">Пример</span><span class="sxs-lookup"><span data-stu-id="9f830-246">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f830-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f830-247">Request</span></span>
<span data-ttu-id="9f830-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f830-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
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

### <a name="response"></a><span data-ttu-id="9f830-249">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f830-249">Response</span></span>
<span data-ttu-id="9f830-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f830-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



