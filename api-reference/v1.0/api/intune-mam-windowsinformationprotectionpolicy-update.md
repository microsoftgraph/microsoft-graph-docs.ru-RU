---
title: Обновление объекта windowsInformationProtectionPolicy
description: Обновление свойств объекта windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db347138feacaf19a0832f744bb409eebb10fae7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954633"
---
# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="8b2f3-103">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b2f3-103">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="8b2f3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b2f3-105">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-105">Update the properties of a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b2f3-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b2f3-106">Prerequisites</span></span>
<span data-ttu-id="8b2f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b2f3-109">Permission type</span></span>|<span data-ttu-id="8b2f3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b2f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b2f3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2f3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b2f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b2f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-114">Not supported.</span></span>|
|<span data-ttu-id="8b2f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b2f3-115">Application</span></span>|<span data-ttu-id="8b2f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b2f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b2f3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8b2f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b2f3-118">Request headers</span></span>
|<span data-ttu-id="8b2f3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b2f3-119">Header</span></span>|<span data-ttu-id="8b2f3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8b2f3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b2f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b2f3-121">Authorization</span></span>|<span data-ttu-id="8b2f3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8b2f3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b2f3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8b2f3-123">Accept</span></span>|<span data-ttu-id="8b2f3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8b2f3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b2f3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b2f3-125">Request body</span></span>
<span data-ttu-id="8b2f3-126">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-126">In the request body, supply a JSON representation for the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="8b2f3-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-127">The following table shows the properties that are required when you create the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="8b2f3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b2f3-128">Property</span></span>|<span data-ttu-id="8b2f3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8b2f3-129">Type</span></span>|<span data-ttu-id="8b2f3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8b2f3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2f3-131">displayName</span><span class="sxs-lookup"><span data-stu-id="8b2f3-131">displayName</span></span>|<span data-ttu-id="8b2f3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-132">String</span></span>|<span data-ttu-id="8b2f3-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-133">Policy display name.</span></span> <span data-ttu-id="8b2f3-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-135">описание</span><span class="sxs-lookup"><span data-stu-id="8b2f3-135">description</span></span>|<span data-ttu-id="8b2f3-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-136">String</span></span>|<span data-ttu-id="8b2f3-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-137">The policy's description.</span></span> <span data-ttu-id="8b2f3-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b2f3-139">createdDateTime</span></span>|<span data-ttu-id="8b2f3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b2f3-140">DateTimeOffset</span></span>|<span data-ttu-id="8b2f3-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-141">The date and time the policy was created.</span></span> <span data-ttu-id="8b2f3-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b2f3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8b2f3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b2f3-144">DateTimeOffset</span></span>|<span data-ttu-id="8b2f3-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-145">Last time the policy was modified.</span></span> <span data-ttu-id="8b2f3-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-147">id</span><span class="sxs-lookup"><span data-stu-id="8b2f3-147">id</span></span>|<span data-ttu-id="8b2f3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-148">String</span></span>|<span data-ttu-id="8b2f3-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-149">Key of the entity.</span></span> <span data-ttu-id="8b2f3-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-151">version</span><span class="sxs-lookup"><span data-stu-id="8b2f3-151">version</span></span>|<span data-ttu-id="8b2f3-152">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-152">String</span></span>|<span data-ttu-id="8b2f3-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-153">Version of the entity.</span></span> <span data-ttu-id="8b2f3-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8b2f3-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8b2f3-155">enforcementLevel</span></span>|[<span data-ttu-id="8b2f3-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8b2f3-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="8b2f3-157">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений унаследованные от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="8b2f3-158">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="8b2f3-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="8b2f3-159">enterpriseDomain</span></span>|<span data-ttu-id="8b2f3-160">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-160">String</span></span>|<span data-ttu-id="8b2f3-161">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="8b2f3-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="8b2f3-163">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-164">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="8b2f3-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="8b2f3-166">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-166">Boolean</span></span>|<span data-ttu-id="8b2f3-167">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8b2f3-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="8b2f3-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8b2f3-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="8b2f3-170">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="8b2f3-171">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="8b2f3-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="8b2f3-173">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-173">Boolean</span></span>|<span data-ttu-id="8b2f3-174">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="8b2f3-175">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="8b2f3-176">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="8b2f3-177">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="8b2f3-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="8b2f3-179">Guid</span><span class="sxs-lookup"><span data-stu-id="8b2f3-179">Guid</span></span>|<span data-ttu-id="8b2f3-180">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="8b2f3-181">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="8b2f3-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="8b2f3-183">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-183">Boolean</span></span>|<span data-ttu-id="8b2f3-184">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="8b2f3-185">iconsVisible</span></span>|<span data-ttu-id="8b2f3-186">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-186">Boolean</span></span>|<span data-ttu-id="8b2f3-187">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="8b2f3-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="8b2f3-188">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="8b2f3-189">protectedApps</span></span>|<span data-ttu-id="8b2f3-190">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8b2f3-191">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="8b2f3-192">exemptApps</span></span>|<span data-ttu-id="8b2f3-193">Коллекция [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8b2f3-194">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="8b2f3-195">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="8b2f3-196">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="8b2f3-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="8b2f3-198">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-199">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="8b2f3-200">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="8b2f3-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="8b2f3-202">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="8b2f3-203">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="8b2f3-204">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="8b2f3-205">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="8b2f3-206">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="8b2f3-207">enterpriseIPRanges</span></span>|<span data-ttu-id="8b2f3-208">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-209">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="8b2f3-210">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="8b2f3-211">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8b2f3-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="8b2f3-213">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-213">Boolean</span></span>|<span data-ttu-id="8b2f3-214">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="8b2f3-215">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="8b2f3-216">enterpriseProxyServers</span></span>|<span data-ttu-id="8b2f3-217">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-218">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-218">This is a list of proxy servers.</span></span> <span data-ttu-id="8b2f3-219">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="8b2f3-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="8b2f3-221">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-222">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="8b2f3-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="8b2f3-223">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="8b2f3-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="8b2f3-224">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="8b2f3-225">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="8b2f3-226">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8b2f3-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="8b2f3-228">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-228">Boolean</span></span>|<span data-ttu-id="8b2f3-229">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="8b2f3-230">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="8b2f3-231">neutralDomainResources</span></span>|<span data-ttu-id="8b2f3-232">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-233">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="8b2f3-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="8b2f3-235">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-235">Boolean</span></span>|<span data-ttu-id="8b2f3-236">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="8b2f3-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="8b2f3-238">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8b2f3-239">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8b2f3-240">isAssigned</span></span>|<span data-ttu-id="8b2f3-241">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-241">Boolean</span></span>|<span data-ttu-id="8b2f3-242">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="8b2f3-243">Наследуется от [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8b2f3-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="8b2f3-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="8b2f3-245">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-245">Boolean</span></span>|<span data-ttu-id="8b2f3-246">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="8b2f3-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="8b2f3-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="8b2f3-248">Строка</span><span class="sxs-lookup"><span data-stu-id="8b2f3-248">String</span></span>|<span data-ttu-id="8b2f3-249">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="8b2f3-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="8b2f3-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="8b2f3-251">Логический</span><span class="sxs-lookup"><span data-stu-id="8b2f3-251">Boolean</span></span>|<span data-ttu-id="8b2f3-252">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="8b2f3-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8b2f3-253">pinMinimumLength</span></span>|<span data-ttu-id="8b2f3-254">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-254">Int32</span></span>|<span data-ttu-id="8b2f3-255">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="8b2f3-256">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-256">Default value is 4.</span></span> <span data-ttu-id="8b2f3-257">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="8b2f3-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="8b2f3-258">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="8b2f3-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="8b2f3-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="8b2f3-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="8b2f3-260">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8b2f3-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8b2f3-261">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8b2f3-262">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-262">Default is NotAllow.</span></span> <span data-ttu-id="8b2f3-263">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="8b2f3-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="8b2f3-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="8b2f3-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8b2f3-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8b2f3-266">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8b2f3-267">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-267">Default is NotAllow.</span></span> <span data-ttu-id="8b2f3-268">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="8b2f3-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="8b2f3-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="8b2f3-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8b2f3-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8b2f3-271">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8b2f3-272">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="8b2f3-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="8b2f3-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="8b2f3-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="8b2f3-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="8b2f3-274">/ : ; < = > ?</span></span><span data-ttu-id="8b2f3-275"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="8b2f3-275"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="8b2f3-276">} ~.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-276">} ~.</span></span> <span data-ttu-id="8b2f3-277">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-277">Default is NotAllow.</span></span> <span data-ttu-id="8b2f3-278">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-278">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="8b2f3-279">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8b2f3-279">pinExpirationDays</span></span>|<span data-ttu-id="8b2f3-280">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-280">Int32</span></span>|<span data-ttu-id="8b2f3-281">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-281">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="8b2f3-282">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="8b2f3-282">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="8b2f3-283">до 0.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-283">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="8b2f3-284">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-284">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="8b2f3-285">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-285">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="8b2f3-286">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-286">Default is 0.</span></span>|
|<span data-ttu-id="8b2f3-287">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="8b2f3-287">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="8b2f3-288">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-288">Int32</span></span>|<span data-ttu-id="8b2f3-289">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-289">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="8b2f3-290">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="8b2f3-290">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="8b2f3-291">до 0.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-291">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="8b2f3-292">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-292">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="8b2f3-293">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-293">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="8b2f3-294">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-294">Default is 0.</span></span>|
|<span data-ttu-id="8b2f3-295">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="8b2f3-295">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="8b2f3-296">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-296">Int32</span></span>|<span data-ttu-id="8b2f3-297">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-297">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="8b2f3-298">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-298">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="8b2f3-299">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-299">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="8b2f3-300">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="8b2f3-300">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="8b2f3-301">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-301">Int32</span></span>|<span data-ttu-id="8b2f3-302">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-302">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="8b2f3-303">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-303">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="8b2f3-304">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="8b2f3-304">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="8b2f3-305">Int32</span><span class="sxs-lookup"><span data-stu-id="8b2f3-305">Int32</span></span>|<span data-ttu-id="8b2f3-306">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях)</span><span class="sxs-lookup"><span data-stu-id="8b2f3-306">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="8b2f3-307">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b2f3-307">Response</span></span>
<span data-ttu-id="8b2f3-308">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-308">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2f3-309">Пример</span><span class="sxs-lookup"><span data-stu-id="8b2f3-309">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b2f3-310">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b2f3-310">Request</span></span>
<span data-ttu-id="8b2f3-311">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-311">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4405

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="8b2f3-312">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b2f3-312">Response</span></span>
<span data-ttu-id="8b2f3-p131">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8b2f3-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



