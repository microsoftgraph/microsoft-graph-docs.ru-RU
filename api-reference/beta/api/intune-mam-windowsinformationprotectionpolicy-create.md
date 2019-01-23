---
title: Create windowsInformationProtectionPolicy
description: Создание объекта windowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74d9e4a8ddd9ae0979a6360eaf229396b2e107bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416610"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="f04fa-103">Create windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="f04fa-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="f04fa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f04fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f04fa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f04fa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f04fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f04fa-107">Создание объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f04fa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f04fa-108">Prerequisites</span></span>
<span data-ttu-id="f04fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f04fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f04fa-111">Permission type</span></span>|<span data-ttu-id="f04fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f04fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f04fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f04fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f04fa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f04fa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f04fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f04fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f04fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fa-116">Not supported.</span></span>|
|<span data-ttu-id="f04fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f04fa-117">Application</span></span>|<span data-ttu-id="f04fa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f04fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f04fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f04fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f04fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f04fa-120">Request headers</span></span>
|<span data-ttu-id="f04fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f04fa-121">Header</span></span>|<span data-ttu-id="f04fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f04fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f04fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f04fa-123">Authorization</span></span>|<span data-ttu-id="f04fa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f04fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f04fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f04fa-125">Accept</span></span>|<span data-ttu-id="f04fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f04fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f04fa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f04fa-127">Request body</span></span>
<span data-ttu-id="f04fa-128">В теле запроса добавьте представление объекта windowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f04fa-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="f04fa-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="f04fa-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="f04fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f04fa-130">Property</span></span>|<span data-ttu-id="f04fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f04fa-131">Type</span></span>|<span data-ttu-id="f04fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f04fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f04fa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f04fa-133">displayName</span></span>|<span data-ttu-id="f04fa-134">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-134">String</span></span>|<span data-ttu-id="f04fa-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="f04fa-135">Policy display name.</span></span> <span data-ttu-id="f04fa-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-137">description</span><span class="sxs-lookup"><span data-stu-id="f04fa-137">description</span></span>|<span data-ttu-id="f04fa-138">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-138">String</span></span>|<span data-ttu-id="f04fa-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="f04fa-139">The policy's description.</span></span> <span data-ttu-id="f04fa-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f04fa-141">createdDateTime</span></span>|<span data-ttu-id="f04fa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f04fa-142">DateTimeOffset</span></span>|<span data-ttu-id="f04fa-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="f04fa-143">The date and time the policy was created.</span></span> <span data-ttu-id="f04fa-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f04fa-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f04fa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f04fa-146">DateTimeOffset</span></span>|<span data-ttu-id="f04fa-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="f04fa-147">Last time the policy was modified.</span></span> <span data-ttu-id="f04fa-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f04fa-149">roleScopeTagIds</span></span>|<span data-ttu-id="f04fa-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f04fa-150">String collection</span></span>|<span data-ttu-id="f04fa-151">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f04fa-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f04fa-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-153">id</span><span class="sxs-lookup"><span data-stu-id="f04fa-153">id</span></span>|<span data-ttu-id="f04fa-154">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-154">String</span></span>|<span data-ttu-id="f04fa-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f04fa-155">Key of the entity.</span></span> <span data-ttu-id="f04fa-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-157">version</span><span class="sxs-lookup"><span data-stu-id="f04fa-157">version</span></span>|<span data-ttu-id="f04fa-158">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-158">String</span></span>|<span data-ttu-id="f04fa-159">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="f04fa-159">Version of the entity.</span></span> <span data-ttu-id="f04fa-160">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f04fa-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="f04fa-161">enforcementLevel</span></span>|[<span data-ttu-id="f04fa-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="f04fa-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="f04fa-163">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="f04fa-164">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="f04fa-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="f04fa-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="f04fa-165">enterpriseDomain</span></span>|<span data-ttu-id="f04fa-166">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-166">String</span></span>|<span data-ttu-id="f04fa-167">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="f04fa-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="f04fa-169">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-170">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="f04fa-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="f04fa-172">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-172">Boolean</span></span>|<span data-ttu-id="f04fa-173">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f04fa-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="f04fa-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f04fa-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="f04fa-176">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="f04fa-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="f04fa-177">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="f04fa-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="f04fa-179">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-179">Boolean</span></span>|<span data-ttu-id="f04fa-180">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="f04fa-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="f04fa-181">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="f04fa-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="f04fa-182">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="f04fa-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="f04fa-183">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="f04fa-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="f04fa-185">Guid</span><span class="sxs-lookup"><span data-stu-id="f04fa-185">Guid</span></span>|<span data-ttu-id="f04fa-186">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="f04fa-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="f04fa-187">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="f04fa-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="f04fa-189">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-189">Boolean</span></span>|<span data-ttu-id="f04fa-190">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="f04fa-191">iconsVisible</span></span>|<span data-ttu-id="f04fa-192">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-192">Boolean</span></span>|<span data-ttu-id="f04fa-193">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="f04fa-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="f04fa-194">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="f04fa-195">protectedApps</span></span>|<span data-ttu-id="f04fa-196">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="f04fa-197">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="f04fa-198">exemptApps</span></span>|<span data-ttu-id="f04fa-199">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="f04fa-200">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="f04fa-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="f04fa-201">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="f04fa-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="f04fa-202">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="f04fa-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="f04fa-204">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-205">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="f04fa-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="f04fa-206">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="f04fa-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="f04fa-208">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="f04fa-209">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="f04fa-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="f04fa-210">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="f04fa-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="f04fa-211">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="f04fa-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="f04fa-212">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="f04fa-213">enterpriseIPRanges</span></span>|<span data-ttu-id="f04fa-214">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="f04fa-215">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="f04fa-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="f04fa-216">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="f04fa-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="f04fa-217">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f04fa-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="f04fa-219">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-219">Boolean</span></span>|<span data-ttu-id="f04fa-220">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="f04fa-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="f04fa-221">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="f04fa-222">enterpriseProxyServers</span></span>|<span data-ttu-id="f04fa-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-224">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="f04fa-224">This is a list of proxy servers.</span></span> <span data-ttu-id="f04fa-225">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="f04fa-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="f04fa-227">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-228">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="f04fa-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="f04fa-229">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="f04fa-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="f04fa-230">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f04fa-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="f04fa-231">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="f04fa-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="f04fa-232">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f04fa-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="f04fa-234">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-234">Boolean</span></span>|<span data-ttu-id="f04fa-235">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="f04fa-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="f04fa-236">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="f04fa-237">neutralDomainResources</span></span>|<span data-ttu-id="f04fa-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-239">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="f04fa-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="f04fa-241">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-241">Boolean</span></span>|<span data-ttu-id="f04fa-242">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="f04fa-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="f04fa-244">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="f04fa-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="f04fa-245">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f04fa-246">isAssigned</span></span>|<span data-ttu-id="f04fa-247">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-247">Boolean</span></span>|<span data-ttu-id="f04fa-248">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="f04fa-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="f04fa-249">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f04fa-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="f04fa-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="f04fa-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="f04fa-251">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-251">Boolean</span></span>|<span data-ttu-id="f04fa-252">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="f04fa-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="f04fa-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="f04fa-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="f04fa-254">String</span><span class="sxs-lookup"><span data-stu-id="f04fa-254">String</span></span>|<span data-ttu-id="f04fa-255">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="f04fa-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="f04fa-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="f04fa-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="f04fa-257">Логический</span><span class="sxs-lookup"><span data-stu-id="f04fa-257">Boolean</span></span>|<span data-ttu-id="f04fa-258">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="f04fa-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="f04fa-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f04fa-259">pinMinimumLength</span></span>|<span data-ttu-id="f04fa-260">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-260">Int32</span></span>|<span data-ttu-id="f04fa-261">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="f04fa-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="f04fa-262">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="f04fa-262">Default value is 4.</span></span> <span data-ttu-id="f04fa-263">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="f04fa-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="f04fa-264">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="f04fa-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="f04fa-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="f04fa-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="f04fa-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f04fa-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f04fa-267">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f04fa-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f04fa-268">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="f04fa-268">Default is NotAllow.</span></span> <span data-ttu-id="f04fa-269">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="f04fa-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f04fa-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="f04fa-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="f04fa-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f04fa-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f04fa-272">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f04fa-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f04fa-273">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="f04fa-273">Default is NotAllow.</span></span> <span data-ttu-id="f04fa-274">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="f04fa-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f04fa-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="f04fa-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="f04fa-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="f04fa-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="f04fa-277">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f04fa-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f04fa-278">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="f04fa-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="f04fa-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="f04fa-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="f04fa-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="f04fa-280">/ : ; < = > ?</span></span><span data-ttu-id="f04fa-281"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="f04fa-281"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="f04fa-282">} ~.</span><span class="sxs-lookup"><span data-stu-id="f04fa-282">} ~.</span></span> <span data-ttu-id="f04fa-283">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="f04fa-283">Default is NotAllow.</span></span> <span data-ttu-id="f04fa-284">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="f04fa-284">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="f04fa-285">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f04fa-285">pinExpirationDays</span></span>|<span data-ttu-id="f04fa-286">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-286">Int32</span></span>|<span data-ttu-id="f04fa-287">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="f04fa-287">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="f04fa-288">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="f04fa-288">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="f04fa-289">до 0.</span><span class="sxs-lookup"><span data-stu-id="f04fa-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="f04fa-290">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="f04fa-290">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="f04fa-291">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="f04fa-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="f04fa-292">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="f04fa-292">Default is 0.</span></span>|
|<span data-ttu-id="f04fa-293">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="f04fa-293">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="f04fa-294">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-294">Int32</span></span>|<span data-ttu-id="f04fa-295">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="f04fa-295">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="f04fa-296">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="f04fa-296">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="f04fa-297">до 0.</span><span class="sxs-lookup"><span data-stu-id="f04fa-297">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="f04fa-298">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="f04fa-298">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="f04fa-299">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="f04fa-299">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="f04fa-300">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="f04fa-300">Default is 0.</span></span>|
|<span data-ttu-id="f04fa-301">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="f04fa-301">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="f04fa-302">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-302">Int32</span></span>|<span data-ttu-id="f04fa-303">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="f04fa-303">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="f04fa-304">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="f04fa-304">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="f04fa-305">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="f04fa-305">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="f04fa-306">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="f04fa-306">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="f04fa-307">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-307">Int32</span></span>|<span data-ttu-id="f04fa-308">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="f04fa-308">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="f04fa-309">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="f04fa-309">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="f04fa-310">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="f04fa-310">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="f04fa-311">Int32</span><span class="sxs-lookup"><span data-stu-id="f04fa-311">Int32</span></span>|<span data-ttu-id="f04fa-312">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях)</span><span class="sxs-lookup"><span data-stu-id="f04fa-312">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="f04fa-313">Ответ</span><span class="sxs-lookup"><span data-stu-id="f04fa-313">Response</span></span>
<span data-ttu-id="f04fa-314">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f04fa-314">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f04fa-315">Пример</span><span class="sxs-lookup"><span data-stu-id="f04fa-315">Example</span></span>

### <a name="request"></a><span data-ttu-id="f04fa-316">Запрос</span><span class="sxs-lookup"><span data-stu-id="f04fa-316">Request</span></span>
<span data-ttu-id="f04fa-317">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f04fa-317">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4467

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

### <a name="response"></a><span data-ttu-id="f04fa-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="f04fa-318">Response</span></span>
<span data-ttu-id="f04fa-p133">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f04fa-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4639

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




