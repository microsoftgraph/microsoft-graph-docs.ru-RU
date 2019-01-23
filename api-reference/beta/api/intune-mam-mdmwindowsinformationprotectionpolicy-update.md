---
title: Обновление объекта mdmWindowsInformationProtectionPolicy
description: Обновление свойств объекта mdmWindowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 900a2eaf57b6b6ba33d0f6071aaa9fc875e81762
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400251"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="0ecee-103">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0ecee-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="0ecee-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ecee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ecee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ecee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ecee-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ecee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ecee-107">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ecee-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="0ecee-108">Prerequisites</span></span>
<span data-ttu-id="0ecee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ecee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ecee-111">Permission type</span></span>|<span data-ttu-id="0ecee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ecee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ecee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ecee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ecee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ecee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ecee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ecee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ecee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ecee-116">Not supported.</span></span>|
|<span data-ttu-id="0ecee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ecee-117">Application</span></span>|<span data-ttu-id="0ecee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ecee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ecee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ecee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0ecee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ecee-120">Request headers</span></span>
|<span data-ttu-id="0ecee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ecee-121">Header</span></span>|<span data-ttu-id="0ecee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ecee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ecee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ecee-123">Authorization</span></span>|<span data-ttu-id="0ecee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ecee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ecee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ecee-125">Accept</span></span>|<span data-ttu-id="0ecee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ecee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ecee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ecee-127">Request body</span></span>
<span data-ttu-id="0ecee-128">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ecee-128">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="0ecee-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-129">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="0ecee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ecee-130">Property</span></span>|<span data-ttu-id="0ecee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ecee-131">Type</span></span>|<span data-ttu-id="0ecee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ecee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecee-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0ecee-133">displayName</span></span>|<span data-ttu-id="0ecee-134">String</span><span class="sxs-lookup"><span data-stu-id="0ecee-134">String</span></span>|<span data-ttu-id="0ecee-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0ecee-135">Policy display name.</span></span> <span data-ttu-id="0ecee-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-137">description</span><span class="sxs-lookup"><span data-stu-id="0ecee-137">description</span></span>|<span data-ttu-id="0ecee-138">String</span><span class="sxs-lookup"><span data-stu-id="0ecee-138">String</span></span>|<span data-ttu-id="0ecee-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0ecee-139">The policy's description.</span></span> <span data-ttu-id="0ecee-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecee-141">createdDateTime</span></span>|<span data-ttu-id="0ecee-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecee-142">DateTimeOffset</span></span>|<span data-ttu-id="0ecee-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0ecee-143">The date and time the policy was created.</span></span> <span data-ttu-id="0ecee-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecee-145">lastModifiedDateTime</span></span>|<span data-ttu-id="0ecee-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecee-146">DateTimeOffset</span></span>|<span data-ttu-id="0ecee-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0ecee-147">Last time the policy was modified.</span></span> <span data-ttu-id="0ecee-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ecee-149">roleScopeTagIds</span></span>|<span data-ttu-id="0ecee-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ecee-150">String collection</span></span>|<span data-ttu-id="0ecee-151">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0ecee-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ecee-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-153">id</span><span class="sxs-lookup"><span data-stu-id="0ecee-153">id</span></span>|<span data-ttu-id="0ecee-154">String</span><span class="sxs-lookup"><span data-stu-id="0ecee-154">String</span></span>|<span data-ttu-id="0ecee-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0ecee-155">Key of the entity.</span></span> <span data-ttu-id="0ecee-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-157">version</span><span class="sxs-lookup"><span data-stu-id="0ecee-157">version</span></span>|<span data-ttu-id="0ecee-158">String</span><span class="sxs-lookup"><span data-stu-id="0ecee-158">String</span></span>|<span data-ttu-id="0ecee-159">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0ecee-159">Version of the entity.</span></span> <span data-ttu-id="0ecee-160">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0ecee-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="0ecee-161">enforcementLevel</span></span>|[<span data-ttu-id="0ecee-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="0ecee-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="0ecee-163">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="0ecee-164">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="0ecee-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="0ecee-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="0ecee-165">enterpriseDomain</span></span>|<span data-ttu-id="0ecee-166">String</span><span class="sxs-lookup"><span data-stu-id="0ecee-166">String</span></span>|<span data-ttu-id="0ecee-167">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="0ecee-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="0ecee-169">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-170">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="0ecee-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="0ecee-172">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-172">Boolean</span></span>|<span data-ttu-id="0ecee-173">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecee-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="0ecee-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0ecee-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="0ecee-176">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="0ecee-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="0ecee-177">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="0ecee-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="0ecee-179">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-179">Boolean</span></span>|<span data-ttu-id="0ecee-180">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="0ecee-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="0ecee-181">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="0ecee-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="0ecee-182">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="0ecee-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="0ecee-183">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="0ecee-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="0ecee-185">Guid</span><span class="sxs-lookup"><span data-stu-id="0ecee-185">Guid</span></span>|<span data-ttu-id="0ecee-186">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="0ecee-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="0ecee-187">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="0ecee-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="0ecee-189">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-189">Boolean</span></span>|<span data-ttu-id="0ecee-190">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="0ecee-191">iconsVisible</span></span>|<span data-ttu-id="0ecee-192">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-192">Boolean</span></span>|<span data-ttu-id="0ecee-193">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="0ecee-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="0ecee-194">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="0ecee-195">protectedApps</span></span>|<span data-ttu-id="0ecee-196">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0ecee-197">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="0ecee-198">exemptApps</span></span>|<span data-ttu-id="0ecee-199">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="0ecee-200">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="0ecee-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="0ecee-201">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="0ecee-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="0ecee-202">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="0ecee-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="0ecee-204">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-205">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="0ecee-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="0ecee-206">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="0ecee-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="0ecee-208">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="0ecee-209">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="0ecee-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="0ecee-210">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="0ecee-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="0ecee-211">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="0ecee-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="0ecee-212">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="0ecee-213">enterpriseIPRanges</span></span>|<span data-ttu-id="0ecee-214">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="0ecee-215">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="0ecee-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="0ecee-216">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="0ecee-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="0ecee-217">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0ecee-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="0ecee-219">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-219">Boolean</span></span>|<span data-ttu-id="0ecee-220">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="0ecee-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="0ecee-221">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="0ecee-222">enterpriseProxyServers</span></span>|<span data-ttu-id="0ecee-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-224">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="0ecee-224">This is a list of proxy servers.</span></span> <span data-ttu-id="0ecee-225">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="0ecee-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="0ecee-227">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-228">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="0ecee-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="0ecee-229">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="0ecee-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="0ecee-230">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0ecee-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="0ecee-231">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="0ecee-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="0ecee-232">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0ecee-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="0ecee-234">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-234">Boolean</span></span>|<span data-ttu-id="0ecee-235">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="0ecee-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="0ecee-236">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="0ecee-237">neutralDomainResources</span></span>|<span data-ttu-id="0ecee-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-239">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="0ecee-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="0ecee-241">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-241">Boolean</span></span>|<span data-ttu-id="0ecee-242">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="0ecee-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="0ecee-244">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="0ecee-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="0ecee-245">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="0ecee-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0ecee-246">isAssigned</span></span>|<span data-ttu-id="0ecee-247">Логический</span><span class="sxs-lookup"><span data-stu-id="0ecee-247">Boolean</span></span>|<span data-ttu-id="0ecee-248">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="0ecee-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="0ecee-249">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0ecee-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0ecee-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ecee-250">Response</span></span>
<span data-ttu-id="0ecee-251">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ecee-251">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ecee-252">Пример</span><span class="sxs-lookup"><span data-stu-id="0ecee-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ecee-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ecee-253">Request</span></span>
<span data-ttu-id="0ecee-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ecee-254">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ecee-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ecee-255">Response</span></span>
<span data-ttu-id="0ecee-p124">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ecee-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




