---
title: Обновление объекта windowsInformationProtectionPolicy
description: Обновление свойств объекта windowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e417f7444e60c7d021c4bb3a88a610e5f6884da
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639098"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="fef1c-103">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fef1c-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="fef1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fef1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef1c-106">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-106">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fef1c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fef1c-107">Prerequisites</span></span>
<span data-ttu-id="fef1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef1c-110">Permission type</span></span>|<span data-ttu-id="fef1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fef1c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef1c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fef1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef1c-115">Not supported.</span></span>|
|<span data-ttu-id="fef1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fef1c-116">Application</span></span>|<span data-ttu-id="fef1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fef1c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef1c-119">Request headers</span></span>
|<span data-ttu-id="fef1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fef1c-120">Header</span></span>|<span data-ttu-id="fef1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fef1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef1c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fef1c-122">Authorization</span></span>|<span data-ttu-id="fef1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fef1c-124">Accept</span></span>|<span data-ttu-id="fef1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fef1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef1c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fef1c-126">Request body</span></span>
<span data-ttu-id="fef1c-127">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fef1c-127">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="fef1c-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-128">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="fef1c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fef1c-129">Property</span></span>|<span data-ttu-id="fef1c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fef1c-130">Type</span></span>|<span data-ttu-id="fef1c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fef1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef1c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fef1c-132">displayName</span></span>|<span data-ttu-id="fef1c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fef1c-133">String</span></span>|<span data-ttu-id="fef1c-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="fef1c-134">Policy display name.</span></span> <span data-ttu-id="fef1c-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-136">description</span><span class="sxs-lookup"><span data-stu-id="fef1c-136">description</span></span>|<span data-ttu-id="fef1c-137">String</span><span class="sxs-lookup"><span data-stu-id="fef1c-137">String</span></span>|<span data-ttu-id="fef1c-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="fef1c-138">The policy's description.</span></span> <span data-ttu-id="fef1c-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fef1c-140">createdDateTime</span></span>|<span data-ttu-id="fef1c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fef1c-141">DateTimeOffset</span></span>|<span data-ttu-id="fef1c-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="fef1c-142">The date and time the policy was created.</span></span> <span data-ttu-id="fef1c-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fef1c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fef1c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fef1c-145">DateTimeOffset</span></span>|<span data-ttu-id="fef1c-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="fef1c-146">Last time the policy was modified.</span></span> <span data-ttu-id="fef1c-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fef1c-148">roleScopeTagIds</span></span>|<span data-ttu-id="fef1c-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fef1c-149">String collection</span></span>|<span data-ttu-id="fef1c-150">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fef1c-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fef1c-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-152">id</span><span class="sxs-lookup"><span data-stu-id="fef1c-152">id</span></span>|<span data-ttu-id="fef1c-153">String</span><span class="sxs-lookup"><span data-stu-id="fef1c-153">String</span></span>|<span data-ttu-id="fef1c-154">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fef1c-154">Key of the entity.</span></span> <span data-ttu-id="fef1c-155">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-156">version</span><span class="sxs-lookup"><span data-stu-id="fef1c-156">version</span></span>|<span data-ttu-id="fef1c-157">String</span><span class="sxs-lookup"><span data-stu-id="fef1c-157">String</span></span>|<span data-ttu-id="fef1c-158">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="fef1c-158">Version of the entity.</span></span> <span data-ttu-id="fef1c-159">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fef1c-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fef1c-160">enforcementLevel</span></span>|[<span data-ttu-id="fef1c-161">Виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="fef1c-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="fef1c-162">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="fef1c-163">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="fef1c-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="fef1c-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="fef1c-164">enterpriseDomain</span></span>|<span data-ttu-id="fef1c-165">String</span><span class="sxs-lookup"><span data-stu-id="fef1c-165">String</span></span>|<span data-ttu-id="fef1c-166">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="fef1c-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="fef1c-168">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-169">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="fef1c-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="fef1c-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-171">Boolean</span></span>|<span data-ttu-id="fef1c-172">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fef1c-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="fef1c-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fef1c-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="fef1c-175">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="fef1c-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="fef1c-176">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="fef1c-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="fef1c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-178">Boolean</span></span>|<span data-ttu-id="fef1c-179">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="fef1c-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="fef1c-180">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="fef1c-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="fef1c-181">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="fef1c-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="fef1c-182">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="fef1c-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="fef1c-184">Guid</span><span class="sxs-lookup"><span data-stu-id="fef1c-184">Guid</span></span>|<span data-ttu-id="fef1c-185">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="fef1c-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="fef1c-186">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="fef1c-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="fef1c-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-188">Boolean</span></span>|<span data-ttu-id="fef1c-189">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="fef1c-190">iconsVisible</span></span>|<span data-ttu-id="fef1c-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-191">Boolean</span></span>|<span data-ttu-id="fef1c-192">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="fef1c-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="fef1c-193">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="fef1c-194">protectedApps</span></span>|<span data-ttu-id="fef1c-195">Коллекция объектов [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fef1c-196">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="fef1c-197">exemptApps</span></span>|<span data-ttu-id="fef1c-198">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fef1c-199">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="fef1c-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="fef1c-200">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="fef1c-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="fef1c-201">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="fef1c-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="fef1c-203">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-204">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="fef1c-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="fef1c-205">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fef1c-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="fef1c-207">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="fef1c-208">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="fef1c-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="fef1c-209">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="fef1c-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="fef1c-210">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="fef1c-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="fef1c-211">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="fef1c-212">enterpriseIPRanges</span></span>|<span data-ttu-id="fef1c-213">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="fef1c-214">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="fef1c-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="fef1c-215">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="fef1c-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="fef1c-216">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fef1c-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="fef1c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-218">Boolean</span></span>|<span data-ttu-id="fef1c-219">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="fef1c-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="fef1c-220">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="fef1c-221">enterpriseProxyServers</span></span>|<span data-ttu-id="fef1c-222">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-223">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="fef1c-223">This is a list of proxy servers.</span></span> <span data-ttu-id="fef1c-224">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="fef1c-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="fef1c-226">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-227">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="fef1c-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="fef1c-228">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="fef1c-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="fef1c-229">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="fef1c-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="fef1c-230">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="fef1c-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="fef1c-231">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fef1c-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="fef1c-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-233">Boolean</span></span>|<span data-ttu-id="fef1c-234">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="fef1c-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="fef1c-235">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="fef1c-236">neutralDomainResources</span></span>|<span data-ttu-id="fef1c-237">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-238">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="fef1c-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="fef1c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-240">Boolean</span></span>|<span data-ttu-id="fef1c-241">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="fef1c-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="fef1c-243">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fef1c-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fef1c-244">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fef1c-245">isAssigned</span></span>|<span data-ttu-id="fef1c-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-246">Boolean</span></span>|<span data-ttu-id="fef1c-247">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="fef1c-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="fef1c-248">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fef1c-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fef1c-249">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="fef1c-249">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="fef1c-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-250">Boolean</span></span>|<span data-ttu-id="fef1c-251">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="fef1c-251">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="fef1c-252">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="fef1c-252">mdmEnrollmentUrl</span></span>|<span data-ttu-id="fef1c-253">String</span><span class="sxs-lookup"><span data-stu-id="fef1c-253">String</span></span>|<span data-ttu-id="fef1c-254">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="fef1c-254">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="fef1c-255">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="fef1c-255">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="fef1c-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef1c-256">Boolean</span></span>|<span data-ttu-id="fef1c-257">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="fef1c-257">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="fef1c-258">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fef1c-258">pinMinimumLength</span></span>|<span data-ttu-id="fef1c-259">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-259">Int32</span></span>|<span data-ttu-id="fef1c-260">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="fef1c-260">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="fef1c-261">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="fef1c-261">Default value is 4.</span></span> <span data-ttu-id="fef1c-262">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="fef1c-262">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="fef1c-263">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="fef1c-263">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="fef1c-264">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="fef1c-264">pinUppercaseLetters</span></span>|[<span data-ttu-id="fef1c-265">Виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="fef1c-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fef1c-266">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fef1c-266">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fef1c-267">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="fef1c-267">Default is NotAllow.</span></span> <span data-ttu-id="fef1c-268">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="fef1c-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fef1c-269">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="fef1c-269">pinLowercaseLetters</span></span>|[<span data-ttu-id="fef1c-270">Виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="fef1c-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fef1c-271">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fef1c-271">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fef1c-272">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="fef1c-272">Default is NotAllow.</span></span> <span data-ttu-id="fef1c-273">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="fef1c-273">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fef1c-274">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="fef1c-274">pinSpecialCharacters</span></span>|[<span data-ttu-id="fef1c-275">Виндовсинформатионпротектионпинчарактеррекуирементс</span><span class="sxs-lookup"><span data-stu-id="fef1c-275">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="fef1c-276">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fef1c-276">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fef1c-277">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="fef1c-277">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="fef1c-278">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="fef1c-278">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="fef1c-279">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="fef1c-279">/ : ; < = > ?</span></span><span data-ttu-id="fef1c-280"> @ \[ \ \]^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="fef1c-280"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="fef1c-281">} ~.</span><span class="sxs-lookup"><span data-stu-id="fef1c-281">} ~.</span></span> <span data-ttu-id="fef1c-282">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="fef1c-282">Default is NotAllow.</span></span> <span data-ttu-id="fef1c-283">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="fef1c-283">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="fef1c-284">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fef1c-284">pinExpirationDays</span></span>|<span data-ttu-id="fef1c-285">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-285">Int32</span></span>|<span data-ttu-id="fef1c-286">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="fef1c-286">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="fef1c-287">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="fef1c-287">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="fef1c-288">до 0.</span><span class="sxs-lookup"><span data-stu-id="fef1c-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="fef1c-289">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="fef1c-289">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="fef1c-290">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="fef1c-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="fef1c-291">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="fef1c-291">Default is 0.</span></span>|
|<span data-ttu-id="fef1c-292">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="fef1c-292">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="fef1c-293">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-293">Int32</span></span>|<span data-ttu-id="fef1c-294">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="fef1c-294">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="fef1c-295">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="fef1c-295">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="fef1c-296">до 0.</span><span class="sxs-lookup"><span data-stu-id="fef1c-296">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="fef1c-297">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="fef1c-297">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="fef1c-298">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="fef1c-298">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="fef1c-299">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="fef1c-299">Default is 0.</span></span>|
|<span data-ttu-id="fef1c-300">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="fef1c-300">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="fef1c-301">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-301">Int32</span></span>|<span data-ttu-id="fef1c-302">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="fef1c-302">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="fef1c-303">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="fef1c-303">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="fef1c-304">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="fef1c-304">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="fef1c-305">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="fef1c-305">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="fef1c-306">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-306">Int32</span></span>|<span data-ttu-id="fef1c-307">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="fef1c-307">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="fef1c-308">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="fef1c-308">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="fef1c-309">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="fef1c-309">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="fef1c-310">Int32</span><span class="sxs-lookup"><span data-stu-id="fef1c-310">Int32</span></span>|<span data-ttu-id="fef1c-311">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях).</span><span class="sxs-lookup"><span data-stu-id="fef1c-311">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="fef1c-312">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef1c-312">Response</span></span>
<span data-ttu-id="fef1c-313">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fef1c-313">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef1c-314">Пример</span><span class="sxs-lookup"><span data-stu-id="fef1c-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef1c-315">Запрос</span><span class="sxs-lookup"><span data-stu-id="fef1c-315">Request</span></span>
<span data-ttu-id="fef1c-316">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fef1c-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
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

### <a name="response"></a><span data-ttu-id="fef1c-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef1c-317">Response</span></span>
<span data-ttu-id="fef1c-p132">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fef1c-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





