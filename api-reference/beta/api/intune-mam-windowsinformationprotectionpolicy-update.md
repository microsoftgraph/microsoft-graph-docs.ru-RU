---
title: Обновление объекта windowsInformationProtectionPolicy
description: Обновление свойств объекта windowsInformationProtectionPolicy.
ms.openlocfilehash: b16084790fcdb4ad613dcedcc04cf5d0bf9ab2ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079694"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="74e3b-103">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="74e3b-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="74e3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74e3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74e3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74e3b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74e3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74e3b-107">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-107">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74e3b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="74e3b-108">Prerequisites</span></span>
<span data-ttu-id="74e3b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74e3b-111">Permission type</span></span>|<span data-ttu-id="74e3b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74e3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74e3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74e3b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e3b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74e3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74e3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e3b-116">Not supported.</span></span>|
|<span data-ttu-id="74e3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74e3b-117">Application</span></span>|<span data-ttu-id="74e3b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74e3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="74e3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74e3b-120">Request headers</span></span>
|<span data-ttu-id="74e3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74e3b-121">Header</span></span>|<span data-ttu-id="74e3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74e3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e3b-123">Authorization</span></span>|<span data-ttu-id="74e3b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74e3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74e3b-125">Accept</span></span>|<span data-ttu-id="74e3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74e3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74e3b-127">Request body</span></span>
<span data-ttu-id="74e3b-128">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74e3b-128">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="74e3b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-129">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="74e3b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74e3b-130">Property</span></span>|<span data-ttu-id="74e3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74e3b-131">Type</span></span>|<span data-ttu-id="74e3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74e3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e3b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="74e3b-133">displayName</span></span>|<span data-ttu-id="74e3b-134">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-134">String</span></span>|<span data-ttu-id="74e3b-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="74e3b-135">Policy display name.</span></span> <span data-ttu-id="74e3b-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-137">описание</span><span class="sxs-lookup"><span data-stu-id="74e3b-137">description</span></span>|<span data-ttu-id="74e3b-138">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-138">String</span></span>|<span data-ttu-id="74e3b-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="74e3b-139">The policy's description.</span></span> <span data-ttu-id="74e3b-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74e3b-141">createdDateTime</span></span>|<span data-ttu-id="74e3b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74e3b-142">DateTimeOffset</span></span>|<span data-ttu-id="74e3b-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="74e3b-143">The date and time the policy was created.</span></span> <span data-ttu-id="74e3b-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74e3b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="74e3b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74e3b-146">DateTimeOffset</span></span>|<span data-ttu-id="74e3b-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="74e3b-147">Last time the policy was modified.</span></span> <span data-ttu-id="74e3b-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-149">id</span><span class="sxs-lookup"><span data-stu-id="74e3b-149">id</span></span>|<span data-ttu-id="74e3b-150">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-150">String</span></span>|<span data-ttu-id="74e3b-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="74e3b-151">Key of the entity.</span></span> <span data-ttu-id="74e3b-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-153">version</span><span class="sxs-lookup"><span data-stu-id="74e3b-153">version</span></span>|<span data-ttu-id="74e3b-154">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-154">String</span></span>|<span data-ttu-id="74e3b-155">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="74e3b-155">Version of the entity.</span></span> <span data-ttu-id="74e3b-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74e3b-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="74e3b-157">enforcementLevel</span></span>|[<span data-ttu-id="74e3b-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="74e3b-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="74e3b-159">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="74e3b-160">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="74e3b-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="74e3b-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="74e3b-161">enterpriseDomain</span></span>|<span data-ttu-id="74e3b-162">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-162">String</span></span>|<span data-ttu-id="74e3b-163">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="74e3b-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="74e3b-165">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-166">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="74e3b-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="74e3b-168">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-168">Boolean</span></span>|<span data-ttu-id="74e3b-169">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="74e3b-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="74e3b-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="74e3b-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="74e3b-172">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="74e3b-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="74e3b-173">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="74e3b-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="74e3b-175">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-175">Boolean</span></span>|<span data-ttu-id="74e3b-176">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="74e3b-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="74e3b-177">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="74e3b-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="74e3b-178">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="74e3b-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="74e3b-179">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="74e3b-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="74e3b-181">Guid</span><span class="sxs-lookup"><span data-stu-id="74e3b-181">Guid</span></span>|<span data-ttu-id="74e3b-182">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="74e3b-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="74e3b-183">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="74e3b-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="74e3b-185">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-185">Boolean</span></span>|<span data-ttu-id="74e3b-186">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="74e3b-187">iconsVisible</span></span>|<span data-ttu-id="74e3b-188">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-188">Boolean</span></span>|<span data-ttu-id="74e3b-189">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="74e3b-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="74e3b-190">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="74e3b-191">protectedApps</span></span>|<span data-ttu-id="74e3b-192">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="74e3b-193">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="74e3b-194">exemptApps</span></span>|<span data-ttu-id="74e3b-195">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="74e3b-196">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="74e3b-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="74e3b-197">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="74e3b-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="74e3b-198">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="74e3b-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="74e3b-200">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-201">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="74e3b-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="74e3b-202">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="74e3b-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="74e3b-204">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="74e3b-205">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="74e3b-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="74e3b-206">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="74e3b-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="74e3b-207">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="74e3b-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="74e3b-208">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="74e3b-209">enterpriseIPRanges</span></span>|<span data-ttu-id="74e3b-210">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="74e3b-211">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="74e3b-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="74e3b-212">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="74e3b-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="74e3b-213">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="74e3b-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="74e3b-215">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-215">Boolean</span></span>|<span data-ttu-id="74e3b-216">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="74e3b-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="74e3b-217">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="74e3b-218">enterpriseProxyServers</span></span>|<span data-ttu-id="74e3b-219">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-220">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="74e3b-220">This is a list of proxy servers.</span></span> <span data-ttu-id="74e3b-221">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="74e3b-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="74e3b-223">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-224">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="74e3b-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="74e3b-225">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="74e3b-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="74e3b-226">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="74e3b-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="74e3b-227">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="74e3b-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="74e3b-228">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="74e3b-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="74e3b-230">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-230">Boolean</span></span>|<span data-ttu-id="74e3b-231">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="74e3b-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="74e3b-232">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="74e3b-233">neutralDomainResources</span></span>|<span data-ttu-id="74e3b-234">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-235">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="74e3b-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="74e3b-237">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-237">Boolean</span></span>|<span data-ttu-id="74e3b-238">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="74e3b-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="74e3b-240">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="74e3b-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="74e3b-241">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="74e3b-242">isAssigned</span></span>|<span data-ttu-id="74e3b-243">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-243">Boolean</span></span>|<span data-ttu-id="74e3b-244">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="74e3b-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="74e3b-245">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="74e3b-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="74e3b-246">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="74e3b-246">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="74e3b-247">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-247">Boolean</span></span>|<span data-ttu-id="74e3b-248">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="74e3b-248">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="74e3b-249">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="74e3b-249">mdmEnrollmentUrl</span></span>|<span data-ttu-id="74e3b-250">String</span><span class="sxs-lookup"><span data-stu-id="74e3b-250">String</span></span>|<span data-ttu-id="74e3b-251">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="74e3b-251">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="74e3b-252">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="74e3b-252">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="74e3b-253">Логический</span><span class="sxs-lookup"><span data-stu-id="74e3b-253">Boolean</span></span>|<span data-ttu-id="74e3b-254">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="74e3b-254">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="74e3b-255">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="74e3b-255">pinMinimumLength</span></span>|<span data-ttu-id="74e3b-256">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-256">Int32</span></span>|<span data-ttu-id="74e3b-257">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="74e3b-257">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="74e3b-258">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="74e3b-258">Default value is 4.</span></span> <span data-ttu-id="74e3b-259">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="74e3b-259">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="74e3b-260">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="74e3b-260">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="74e3b-261">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="74e3b-261">pinUppercaseLetters</span></span>|[<span data-ttu-id="74e3b-262">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="74e3b-262">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="74e3b-263">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="74e3b-263">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="74e3b-264">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="74e3b-264">Default is NotAllow.</span></span> <span data-ttu-id="74e3b-265">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="74e3b-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="74e3b-266">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="74e3b-266">pinLowercaseLetters</span></span>|[<span data-ttu-id="74e3b-267">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="74e3b-267">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="74e3b-268">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="74e3b-268">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="74e3b-269">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="74e3b-269">Default is NotAllow.</span></span> <span data-ttu-id="74e3b-270">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="74e3b-270">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="74e3b-271">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="74e3b-271">pinSpecialCharacters</span></span>|[<span data-ttu-id="74e3b-272">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="74e3b-272">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="74e3b-273">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="74e3b-273">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="74e3b-274">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="74e3b-274">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="74e3b-275">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="74e3b-275">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="74e3b-276">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="74e3b-276">/ : ; < = > ?</span></span><span data-ttu-id="74e3b-277"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="74e3b-277"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="74e3b-278">} ~.</span><span class="sxs-lookup"><span data-stu-id="74e3b-278">} ~.</span></span> <span data-ttu-id="74e3b-279">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="74e3b-279">Default is NotAllow.</span></span> <span data-ttu-id="74e3b-280">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="74e3b-280">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="74e3b-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="74e3b-281">pinExpirationDays</span></span>|<span data-ttu-id="74e3b-282">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-282">Int32</span></span>|<span data-ttu-id="74e3b-283">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="74e3b-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="74e3b-284">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="74e3b-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="74e3b-285">до 0.</span><span class="sxs-lookup"><span data-stu-id="74e3b-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="74e3b-286">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="74e3b-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="74e3b-287">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="74e3b-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="74e3b-288">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="74e3b-288">Default is 0.</span></span>|
|<span data-ttu-id="74e3b-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="74e3b-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="74e3b-290">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-290">Int32</span></span>|<span data-ttu-id="74e3b-291">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="74e3b-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="74e3b-292">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="74e3b-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="74e3b-293">до 0.</span><span class="sxs-lookup"><span data-stu-id="74e3b-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="74e3b-294">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="74e3b-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="74e3b-295">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="74e3b-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="74e3b-296">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="74e3b-296">Default is 0.</span></span>|
|<span data-ttu-id="74e3b-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="74e3b-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="74e3b-298">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-298">Int32</span></span>|<span data-ttu-id="74e3b-299">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="74e3b-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="74e3b-300">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="74e3b-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="74e3b-301">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="74e3b-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="74e3b-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="74e3b-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="74e3b-303">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-303">Int32</span></span>|<span data-ttu-id="74e3b-304">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="74e3b-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="74e3b-305">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="74e3b-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="74e3b-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="74e3b-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="74e3b-307">Int32</span><span class="sxs-lookup"><span data-stu-id="74e3b-307">Int32</span></span>|<span data-ttu-id="74e3b-308">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях)</span><span class="sxs-lookup"><span data-stu-id="74e3b-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="74e3b-309">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e3b-309">Response</span></span>
<span data-ttu-id="74e3b-310">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74e3b-310">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e3b-311">Пример</span><span class="sxs-lookup"><span data-stu-id="74e3b-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="74e3b-312">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e3b-312">Request</span></span>
<span data-ttu-id="74e3b-313">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74e3b-313">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4396

{
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

### <a name="response"></a><span data-ttu-id="74e3b-314">Ответ</span><span class="sxs-lookup"><span data-stu-id="74e3b-314">Response</span></span>
<span data-ttu-id="74e3b-p132">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="74e3b-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4577

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





