---
title: Создание mdmWindowsInformationProtectionPolicy
description: Создание объекта mdmWindowsInformationProtectionPolicy.
ms.openlocfilehash: 4546a44e859c768303179335e54787f892f6d594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077202"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="b205c-103">Создание mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b205c-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="b205c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b205c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b205c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b205c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b205c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b205c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b205c-107">Создание объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-107">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b205c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b205c-108">Prerequisites</span></span>
<span data-ttu-id="b205c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b205c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b205c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b205c-111">Permission type</span></span>|<span data-ttu-id="b205c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b205c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b205c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b205c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b205c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b205c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b205c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b205c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b205c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b205c-116">Not supported.</span></span>|
|<span data-ttu-id="b205c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b205c-117">Application</span></span>|<span data-ttu-id="b205c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b205c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b205c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b205c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b205c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b205c-120">Request headers</span></span>
|<span data-ttu-id="b205c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b205c-121">Header</span></span>|<span data-ttu-id="b205c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b205c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b205c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b205c-123">Authorization</span></span>|<span data-ttu-id="b205c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b205c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b205c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b205c-125">Accept</span></span>|<span data-ttu-id="b205c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b205c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b205c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b205c-127">Request body</span></span>
<span data-ttu-id="b205c-128">В теле запроса добавьте представление объекта mdmWindowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b205c-128">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="b205c-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="b205c-129">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="b205c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b205c-130">Property</span></span>|<span data-ttu-id="b205c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b205c-131">Type</span></span>|<span data-ttu-id="b205c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b205c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b205c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b205c-133">displayName</span></span>|<span data-ttu-id="b205c-134">String</span><span class="sxs-lookup"><span data-stu-id="b205c-134">String</span></span>|<span data-ttu-id="b205c-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="b205c-135">Policy display name.</span></span> <span data-ttu-id="b205c-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-137">описание</span><span class="sxs-lookup"><span data-stu-id="b205c-137">description</span></span>|<span data-ttu-id="b205c-138">String</span><span class="sxs-lookup"><span data-stu-id="b205c-138">String</span></span>|<span data-ttu-id="b205c-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="b205c-139">The policy's description.</span></span> <span data-ttu-id="b205c-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b205c-141">createdDateTime</span></span>|<span data-ttu-id="b205c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b205c-142">DateTimeOffset</span></span>|<span data-ttu-id="b205c-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="b205c-143">The date and time the policy was created.</span></span> <span data-ttu-id="b205c-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b205c-145">lastModifiedDateTime</span></span>|<span data-ttu-id="b205c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b205c-146">DateTimeOffset</span></span>|<span data-ttu-id="b205c-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="b205c-147">Last time the policy was modified.</span></span> <span data-ttu-id="b205c-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-149">id</span><span class="sxs-lookup"><span data-stu-id="b205c-149">id</span></span>|<span data-ttu-id="b205c-150">String</span><span class="sxs-lookup"><span data-stu-id="b205c-150">String</span></span>|<span data-ttu-id="b205c-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b205c-151">Key of the entity.</span></span> <span data-ttu-id="b205c-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-153">version</span><span class="sxs-lookup"><span data-stu-id="b205c-153">version</span></span>|<span data-ttu-id="b205c-154">String</span><span class="sxs-lookup"><span data-stu-id="b205c-154">String</span></span>|<span data-ttu-id="b205c-155">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="b205c-155">Version of the entity.</span></span> <span data-ttu-id="b205c-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b205c-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b205c-157">enforcementLevel</span></span>|[<span data-ttu-id="b205c-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b205c-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="b205c-159">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="b205c-160">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="b205c-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="b205c-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="b205c-161">enterpriseDomain</span></span>|<span data-ttu-id="b205c-162">String</span><span class="sxs-lookup"><span data-stu-id="b205c-162">String</span></span>|<span data-ttu-id="b205c-163">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="b205c-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="b205c-165">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-166">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="b205c-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="b205c-168">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-168">Boolean</span></span>|<span data-ttu-id="b205c-169">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b205c-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="b205c-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="b205c-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="b205c-172">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="b205c-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="b205c-173">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="b205c-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="b205c-175">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-175">Boolean</span></span>|<span data-ttu-id="b205c-176">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="b205c-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="b205c-177">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="b205c-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="b205c-178">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="b205c-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="b205c-179">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="b205c-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="b205c-181">Guid</span><span class="sxs-lookup"><span data-stu-id="b205c-181">Guid</span></span>|<span data-ttu-id="b205c-182">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="b205c-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="b205c-183">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="b205c-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="b205c-185">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-185">Boolean</span></span>|<span data-ttu-id="b205c-186">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="b205c-187">iconsVisible</span></span>|<span data-ttu-id="b205c-188">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-188">Boolean</span></span>|<span data-ttu-id="b205c-189">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="b205c-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="b205c-190">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="b205c-191">protectedApps</span></span>|<span data-ttu-id="b205c-192">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b205c-193">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="b205c-194">exemptApps</span></span>|<span data-ttu-id="b205c-195">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="b205c-196">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="b205c-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="b205c-197">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="b205c-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="b205c-198">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="b205c-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="b205c-200">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-201">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="b205c-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="b205c-202">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="b205c-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="b205c-204">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="b205c-205">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="b205c-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="b205c-206">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="b205c-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="b205c-207">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="b205c-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="b205c-208">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="b205c-209">enterpriseIPRanges</span></span>|<span data-ttu-id="b205c-210">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="b205c-211">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="b205c-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="b205c-212">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="b205c-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="b205c-213">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b205c-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="b205c-215">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-215">Boolean</span></span>|<span data-ttu-id="b205c-216">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="b205c-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="b205c-217">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="b205c-218">enterpriseProxyServers</span></span>|<span data-ttu-id="b205c-219">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-220">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="b205c-220">This is a list of proxy servers.</span></span> <span data-ttu-id="b205c-221">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="b205c-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="b205c-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-224">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="b205c-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="b205c-225">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="b205c-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="b205c-226">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b205c-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="b205c-227">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="b205c-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="b205c-228">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="b205c-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="b205c-230">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-230">Boolean</span></span>|<span data-ttu-id="b205c-231">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="b205c-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="b205c-232">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="b205c-233">neutralDomainResources</span></span>|<span data-ttu-id="b205c-234">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-235">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="b205c-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="b205c-237">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-237">Boolean</span></span>|<span data-ttu-id="b205c-238">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="b205c-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="b205c-240">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="b205c-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="b205c-241">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="b205c-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b205c-242">isAssigned</span></span>|<span data-ttu-id="b205c-243">Логический</span><span class="sxs-lookup"><span data-stu-id="b205c-243">Boolean</span></span>|<span data-ttu-id="b205c-244">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="b205c-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="b205c-245">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b205c-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b205c-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="b205c-246">Response</span></span>
<span data-ttu-id="b205c-247">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b205c-247">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b205c-248">Пример</span><span class="sxs-lookup"><span data-stu-id="b205c-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="b205c-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="b205c-249">Request</span></span>
<span data-ttu-id="b205c-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b205c-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3969

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="b205c-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="b205c-251">Response</span></span>
<span data-ttu-id="b205c-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b205c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





