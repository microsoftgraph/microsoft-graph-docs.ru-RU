---
title: Создание mdmWindowsInformationProtectionPolicy
description: Создание объекта mdmWindowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7ee5979c4f099650770a7d26e76df72751b0f5d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986317"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="83b73-103">Создание mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="83b73-103">Create mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="83b73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83b73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83b73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83b73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83b73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83b73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83b73-107">Создание объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-107">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83b73-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83b73-108">Prerequisites</span></span>
<span data-ttu-id="83b73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83b73-111">Permission type</span></span>|<span data-ttu-id="83b73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83b73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83b73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83b73-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="83b73-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="83b73-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="83b73-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b73-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="83b73-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="83b73-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="83b73-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b73-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83b73-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83b73-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83b73-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83b73-119">Not supported.</span></span>|
|<span data-ttu-id="83b73-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83b73-120">Application</span></span>||
| <span data-ttu-id="83b73-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="83b73-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="83b73-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b73-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="83b73-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="83b73-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="83b73-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b73-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83b73-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83b73-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="83b73-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83b73-126">Request headers</span></span>
|<span data-ttu-id="83b73-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83b73-127">Header</span></span>|<span data-ttu-id="83b73-128">Значение</span><span class="sxs-lookup"><span data-stu-id="83b73-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83b73-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b73-129">Authorization</span></span>|<span data-ttu-id="83b73-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83b73-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83b73-131">Accept</span><span class="sxs-lookup"><span data-stu-id="83b73-131">Accept</span></span>|<span data-ttu-id="83b73-132">application/json</span><span class="sxs-lookup"><span data-stu-id="83b73-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b73-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83b73-133">Request body</span></span>
<span data-ttu-id="83b73-134">В теле запроса добавьте представление объекта mdmWindowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83b73-134">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="83b73-135">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="83b73-135">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="83b73-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="83b73-136">Property</span></span>|<span data-ttu-id="83b73-137">Тип</span><span class="sxs-lookup"><span data-stu-id="83b73-137">Type</span></span>|<span data-ttu-id="83b73-138">Описание</span><span class="sxs-lookup"><span data-stu-id="83b73-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b73-139">displayName</span><span class="sxs-lookup"><span data-stu-id="83b73-139">displayName</span></span>|<span data-ttu-id="83b73-140">String</span><span class="sxs-lookup"><span data-stu-id="83b73-140">String</span></span>|<span data-ttu-id="83b73-141">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="83b73-141">Policy display name.</span></span> <span data-ttu-id="83b73-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-143">description</span><span class="sxs-lookup"><span data-stu-id="83b73-143">description</span></span>|<span data-ttu-id="83b73-144">String</span><span class="sxs-lookup"><span data-stu-id="83b73-144">String</span></span>|<span data-ttu-id="83b73-145">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="83b73-145">The policy's description.</span></span> <span data-ttu-id="83b73-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83b73-147">createdDateTime</span></span>|<span data-ttu-id="83b73-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b73-148">DateTimeOffset</span></span>|<span data-ttu-id="83b73-149">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="83b73-149">The date and time the policy was created.</span></span> <span data-ttu-id="83b73-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83b73-151">lastModifiedDateTime</span></span>|<span data-ttu-id="83b73-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b73-152">DateTimeOffset</span></span>|<span data-ttu-id="83b73-153">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="83b73-153">Last time the policy was modified.</span></span> <span data-ttu-id="83b73-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83b73-155">roleScopeTagIds</span></span>|<span data-ttu-id="83b73-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="83b73-156">String collection</span></span>|<span data-ttu-id="83b73-157">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="83b73-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83b73-158">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-159">id</span><span class="sxs-lookup"><span data-stu-id="83b73-159">id</span></span>|<span data-ttu-id="83b73-160">String</span><span class="sxs-lookup"><span data-stu-id="83b73-160">String</span></span>|<span data-ttu-id="83b73-161">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83b73-161">Key of the entity.</span></span> <span data-ttu-id="83b73-162">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-163">version</span><span class="sxs-lookup"><span data-stu-id="83b73-163">version</span></span>|<span data-ttu-id="83b73-164">String</span><span class="sxs-lookup"><span data-stu-id="83b73-164">String</span></span>|<span data-ttu-id="83b73-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="83b73-165">Version of the entity.</span></span> <span data-ttu-id="83b73-166">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="83b73-167">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="83b73-167">enforcementLevel</span></span>|[<span data-ttu-id="83b73-168">виндовсинформатионпротектионенфорцементлевел</span><span class="sxs-lookup"><span data-stu-id="83b73-168">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="83b73-169">Уровень принудительного применения НЗП. Ознакомьтесь с определением перечисления для поддерживаемых значений, наследуемых от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-169">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="83b73-170">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="83b73-170">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="83b73-171">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="83b73-171">enterpriseDomain</span></span>|<span data-ttu-id="83b73-172">String</span><span class="sxs-lookup"><span data-stu-id="83b73-172">String</span></span>|<span data-ttu-id="83b73-173">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-173">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-174">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="83b73-174">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="83b73-175">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-175">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-176">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-176">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-177">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="83b73-177">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="83b73-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-178">Boolean</span></span>|<span data-ttu-id="83b73-179">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-179">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-180">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="83b73-180">dataRecoveryCertificate</span></span>|[<span data-ttu-id="83b73-181">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="83b73-181">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="83b73-182">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="83b73-182">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="83b73-183">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-183">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-184">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="83b73-184">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="83b73-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-185">Boolean</span></span>|<span data-ttu-id="83b73-186">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="83b73-186">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="83b73-187">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="83b73-187">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="83b73-188">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="83b73-188">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="83b73-189">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-189">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-190">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="83b73-190">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="83b73-191">Guid</span><span class="sxs-lookup"><span data-stu-id="83b73-191">Guid</span></span>|<span data-ttu-id="83b73-192">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="83b73-192">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="83b73-193">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-193">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-194">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="83b73-194">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="83b73-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-195">Boolean</span></span>|<span data-ttu-id="83b73-196">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-196">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-197">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="83b73-197">iconsVisible</span></span>|<span data-ttu-id="83b73-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-198">Boolean</span></span>|<span data-ttu-id="83b73-199">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="83b73-199">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="83b73-200">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-200">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-201">protectedApps</span><span class="sxs-lookup"><span data-stu-id="83b73-201">protectedApps</span></span>|<span data-ttu-id="83b73-202">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-202">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="83b73-203">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-203">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-204">exemptApps</span><span class="sxs-lookup"><span data-stu-id="83b73-204">exemptApps</span></span>|<span data-ttu-id="83b73-205">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-205">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="83b73-206">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="83b73-206">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="83b73-207">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="83b73-207">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="83b73-208">Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-208">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-209">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="83b73-209">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="83b73-210">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-210">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-211">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="83b73-211">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="83b73-212">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-212">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-213">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="83b73-213">enterpriseProxiedDomains</span></span>|<span data-ttu-id="83b73-214">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-214">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="83b73-215">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="83b73-215">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="83b73-216">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="83b73-216">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="83b73-217">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="83b73-217">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="83b73-218">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-218">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-219">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="83b73-219">enterpriseIPRanges</span></span>|<span data-ttu-id="83b73-220">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-220">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="83b73-221">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="83b73-221">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="83b73-222">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="83b73-222">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="83b73-223">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-223">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-224">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="83b73-224">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="83b73-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-225">Boolean</span></span>|<span data-ttu-id="83b73-226">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="83b73-226">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="83b73-227">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-227">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-228">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="83b73-228">enterpriseProxyServers</span></span>|<span data-ttu-id="83b73-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-230">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="83b73-230">This is a list of proxy servers.</span></span> <span data-ttu-id="83b73-231">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-231">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-232">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="83b73-232">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="83b73-233">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-234">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="83b73-234">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="83b73-235">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="83b73-235">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="83b73-236">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="83b73-236">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="83b73-237">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="83b73-237">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="83b73-238">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-238">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-239">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="83b73-239">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="83b73-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-240">Boolean</span></span>|<span data-ttu-id="83b73-241">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="83b73-241">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="83b73-242">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-242">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-243">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="83b73-243">neutralDomainResources</span></span>|<span data-ttu-id="83b73-244">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-245">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-245">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-246">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="83b73-246">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="83b73-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-247">Boolean</span></span>|<span data-ttu-id="83b73-248">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-248">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-249">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="83b73-249">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="83b73-250">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="83b73-250">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="83b73-251">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-251">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="83b73-252">isAssigned</span><span class="sxs-lookup"><span data-stu-id="83b73-252">isAssigned</span></span>|<span data-ttu-id="83b73-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b73-253">Boolean</span></span>|<span data-ttu-id="83b73-254">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="83b73-254">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="83b73-255">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="83b73-255">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="83b73-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="83b73-256">Response</span></span>
<span data-ttu-id="83b73-257">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83b73-257">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b73-258">Пример</span><span class="sxs-lookup"><span data-stu-id="83b73-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="83b73-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="83b73-259">Request</span></span>
<span data-ttu-id="83b73-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83b73-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
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

### <a name="response"></a><span data-ttu-id="83b73-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="83b73-261">Response</span></span>
<span data-ttu-id="83b73-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83b73-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









