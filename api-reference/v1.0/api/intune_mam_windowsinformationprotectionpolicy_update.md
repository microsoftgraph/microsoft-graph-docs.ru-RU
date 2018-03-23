# <a name="update-windowsinformationprotectionpolicy"></a><span data-ttu-id="4275a-101">Обновление объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="4275a-101">Update windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="4275a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4275a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4275a-103">Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-103">Update the properties of a [calendar](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4275a-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4275a-104">Prerequisites</span></span>
<span data-ttu-id="4275a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4275a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4275a-107">Permission type</span></span>|<span data-ttu-id="4275a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4275a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4275a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4275a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4275a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4275a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4275a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4275a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4275a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4275a-112">Not supported.</span></span>|
|<span data-ttu-id="4275a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4275a-113">Application</span></span>|<span data-ttu-id="4275a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4275a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4275a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4275a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4275a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4275a-116">Request headers</span></span>
|<span data-ttu-id="4275a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4275a-117">Header</span></span>|<span data-ttu-id="4275a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4275a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4275a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4275a-119">Authorization</span></span>|<span data-ttu-id="4275a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4275a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4275a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4275a-121">Accept</span></span>|<span data-ttu-id="4275a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4275a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4275a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4275a-123">Request body</span></span>
<span data-ttu-id="4275a-124">В тексте запроса добавьте представление объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4275a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="4275a-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4275a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4275a-126">Property</span></span>|<span data-ttu-id="4275a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4275a-127">Type</span></span>|<span data-ttu-id="4275a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4275a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4275a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4275a-129">displayName</span></span>|<span data-ttu-id="4275a-130">String</span><span class="sxs-lookup"><span data-stu-id="4275a-130">String</span></span>|<span data-ttu-id="4275a-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="4275a-131">Policy display name.</span></span> <span data-ttu-id="4275a-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-133">description</span><span class="sxs-lookup"><span data-stu-id="4275a-133">description</span></span>|<span data-ttu-id="4275a-134">String</span><span class="sxs-lookup"><span data-stu-id="4275a-134">String</span></span>|<span data-ttu-id="4275a-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="4275a-135">The policy's description.</span></span> <span data-ttu-id="4275a-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4275a-137">createdDateTime</span></span>|<span data-ttu-id="4275a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4275a-138">DateTimeOffset</span></span>|<span data-ttu-id="4275a-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="4275a-139">The date and time the group was created.</span></span> <span data-ttu-id="4275a-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4275a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4275a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4275a-142">DateTimeOffset</span></span>|<span data-ttu-id="4275a-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="4275a-143">Last time the policy was modified.</span></span> <span data-ttu-id="4275a-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-145">id</span><span class="sxs-lookup"><span data-stu-id="4275a-145">id</span></span>|<span data-ttu-id="4275a-146">String</span><span class="sxs-lookup"><span data-stu-id="4275a-146">String</span></span>|<span data-ttu-id="4275a-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4275a-147">Key of the setting.</span></span> <span data-ttu-id="4275a-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-149">version</span><span class="sxs-lookup"><span data-stu-id="4275a-149">version</span></span>|<span data-ttu-id="4275a-150">String</span><span class="sxs-lookup"><span data-stu-id="4275a-150">String</span></span>|<span data-ttu-id="4275a-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="4275a-151">Version of the entity.</span></span> <span data-ttu-id="4275a-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4275a-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="4275a-153">enforcementLevel</span></span>|<span data-ttu-id="4275a-154">String</span><span class="sxs-lookup"><span data-stu-id="4275a-154">String</span></span>|<span data-ttu-id="4275a-155">Уровень применения WIP. Поддерживаемые значения см. в определении Enum. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="4275a-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="4275a-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="4275a-156">enterpriseDomain</span></span>|<span data-ttu-id="4275a-157">String</span><span class="sxs-lookup"><span data-stu-id="4275a-157">String</span></span>|<span data-ttu-id="4275a-158">Основной домен предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="4275a-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="4275a-160">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-161">Список доменов предприятия, подлежащих защите. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="4275a-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="4275a-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-163">Boolean</span></span>|<span data-ttu-id="4275a-164">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4275a-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="4275a-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4275a-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="4275a-167">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="4275a-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="4275a-168">То же, что сертификат агента восстановления данных (DRA) для шифрованной файловой системы (EFS). Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="4275a-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="4275a-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-170">Boolean</span></span>|<span data-ttu-id="4275a-171">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="4275a-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="4275a-172">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="4275a-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="4275a-173">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="4275a-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="4275a-174">Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="4275a-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="4275a-176">Guid</span><span class="sxs-lookup"><span data-stu-id="4275a-176">Guid</span></span>|<span data-ttu-id="4275a-177">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="4275a-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="4275a-178">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="4275a-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="4275a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-180">Boolean</span></span>|<span data-ttu-id="4275a-181">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="4275a-182">iconsVisible</span></span>|<span data-ttu-id="4275a-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-183">Boolean</span></span>|<span data-ttu-id="4275a-184">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="4275a-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="4275a-185">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного WIP приложения. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="4275a-186">protectedApps</span></span>|<span data-ttu-id="4275a-187">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4275a-188">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="4275a-189">exemptApps</span></span>|<span data-ttu-id="4275a-190">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4275a-191">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="4275a-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="4275a-192">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="4275a-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="4275a-193">Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="4275a-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="4275a-195">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-196">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="4275a-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="4275a-197">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4275a-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="4275a-199">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="4275a-200">Содержит список корпоративных доменов ресурсов, размещенных в облаке, которое необходимо защищать.</span><span class="sxs-lookup"><span data-stu-id="4275a-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="4275a-201">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="4275a-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="4275a-202">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="4275a-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="4275a-203">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="4275a-204">enterpriseIPRanges</span></span>|<span data-ttu-id="4275a-205">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="4275a-206">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="4275a-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="4275a-207">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="4275a-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="4275a-208">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4275a-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="4275a-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-210">Boolean</span></span>|<span data-ttu-id="4275a-211">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="4275a-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="4275a-212">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="4275a-213">enterpriseProxyServers</span></span>|<span data-ttu-id="4275a-214">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-215">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="4275a-215">This is a list of proxy servers.</span></span> <span data-ttu-id="4275a-216">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="4275a-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="4275a-218">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-219">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="4275a-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="4275a-220">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="4275a-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="4275a-221">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="4275a-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="4275a-222">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="4275a-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="4275a-223">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4275a-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="4275a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-225">Boolean</span></span>|<span data-ttu-id="4275a-226">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="4275a-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="4275a-227">Значение по умолчанию — false. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="4275a-228">neutralDomainResources</span></span>|<span data-ttu-id="4275a-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-230">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="4275a-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="4275a-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-232">Boolean</span></span>|<span data-ttu-id="4275a-233">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="4275a-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="4275a-235">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4275a-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4275a-236">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4275a-237">isAssigned</span></span>|<span data-ttu-id="4275a-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-238">Boolean</span></span>|<span data-ttu-id="4275a-239">Указывает, развернута ли политика в группах включения.</span><span class="sxs-lookup"><span data-stu-id="4275a-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="4275a-240">Наследуется от объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4275a-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="4275a-241">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="4275a-241">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="4275a-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-242">Boolean</span></span>|<span data-ttu-id="4275a-243">Новое свойство в RS2, документация готовится.</span><span class="sxs-lookup"><span data-stu-id="4275a-243">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="4275a-244">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="4275a-244">mdmEnrollmentUrl</span></span>|<span data-ttu-id="4275a-245">String</span><span class="sxs-lookup"><span data-stu-id="4275a-245">String</span></span>|<span data-ttu-id="4275a-246">URL-адрес регистрации в системе MDM.</span><span class="sxs-lookup"><span data-stu-id="4275a-246">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="4275a-247">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="4275a-247">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="4275a-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="4275a-248">Boolean</span></span>|<span data-ttu-id="4275a-249">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="4275a-249">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="4275a-250">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4275a-250">pinMinimumLength</span></span>|<span data-ttu-id="4275a-251">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-251">Int32</span></span>|<span data-ttu-id="4275a-252">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="4275a-252">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="4275a-253">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="4275a-253">Default value is 4.</span></span> <span data-ttu-id="4275a-254">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="4275a-254">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="4275a-255">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="4275a-255">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="4275a-256">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="4275a-256">pinUppercaseLetters</span></span>|<span data-ttu-id="4275a-257">String</span><span class="sxs-lookup"><span data-stu-id="4275a-257">String</span></span>|<span data-ttu-id="4275a-258">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4275a-258">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4275a-259">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="4275a-259">Default is NotAllow.</span></span> <span data-ttu-id="4275a-260">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="4275a-260">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4275a-261">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="4275a-261">pinLowercaseLetters</span></span>|<span data-ttu-id="4275a-262">String</span><span class="sxs-lookup"><span data-stu-id="4275a-262">String</span></span>|<span data-ttu-id="4275a-263">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4275a-263">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4275a-264">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="4275a-264">Default is NotAllow.</span></span> <span data-ttu-id="4275a-265">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="4275a-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4275a-266">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="4275a-266">pinSpecialCharacters</span></span>|<span data-ttu-id="4275a-267">String</span><span class="sxs-lookup"><span data-stu-id="4275a-267">String</span></span>|<span data-ttu-id="4275a-268">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4275a-268">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4275a-269">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="4275a-269">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="4275a-270">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="4275a-270">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="4275a-271">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="4275a-271">/ : ; < = > ?</span></span><span data-ttu-id="4275a-272"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="4275a-272"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="4275a-273">} ~.</span><span class="sxs-lookup"><span data-stu-id="4275a-273">=, ==</span></span> <span data-ttu-id="4275a-274">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="4275a-274">Default is NotAllow.</span></span> <span data-ttu-id="4275a-275">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="4275a-275">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="4275a-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4275a-276">pinExpirationDays</span></span>|<span data-ttu-id="4275a-277">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-277">Int32</span></span>|<span data-ttu-id="4275a-278">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="4275a-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="4275a-279">Для этого параметра политики можно установить значение в диапазоне от 730</span><span class="sxs-lookup"><span data-stu-id="4275a-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="4275a-280">до 0.</span><span class="sxs-lookup"><span data-stu-id="4275a-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="4275a-281">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="4275a-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="4275a-282">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="4275a-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="4275a-283">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="4275a-283">Default is 0.</span></span>|
|<span data-ttu-id="4275a-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="4275a-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="4275a-285">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-285">Int32</span></span>|<span data-ttu-id="4275a-286">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="4275a-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="4275a-287">Для этого параметра политики можно установить значение в диапазоне от 50</span><span class="sxs-lookup"><span data-stu-id="4275a-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="4275a-288">до 0.</span><span class="sxs-lookup"><span data-stu-id="4275a-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="4275a-289">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="4275a-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="4275a-290">Этот узел добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="4275a-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="4275a-291">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="4275a-291">Default is 0.</span></span>|
|<span data-ttu-id="4275a-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="4275a-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="4275a-293">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-293">Int32</span></span>|<span data-ttu-id="4275a-294">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="4275a-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="4275a-295">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="4275a-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="4275a-296">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="4275a-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="4275a-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="4275a-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="4275a-298">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-298">Int32</span></span>|<span data-ttu-id="4275a-299">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="4275a-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="4275a-300">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="4275a-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="4275a-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="4275a-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="4275a-302">Int32</span><span class="sxs-lookup"><span data-stu-id="4275a-302">Int32</span></span>|<span data-ttu-id="4275a-303">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях).</span><span class="sxs-lookup"><span data-stu-id="4275a-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="4275a-304">Отклик</span><span class="sxs-lookup"><span data-stu-id="4275a-304">Response</span></span>
<span data-ttu-id="4275a-305">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4275a-305">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4275a-306">Пример</span><span class="sxs-lookup"><span data-stu-id="4275a-306">Example</span></span>
### <a name="request"></a><span data-ttu-id="4275a-307">Запрос</span><span class="sxs-lookup"><span data-stu-id="4275a-307">Request</span></span>
<span data-ttu-id="4275a-308">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4275a-308">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 4393

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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="4275a-309">Ответ</span><span class="sxs-lookup"><span data-stu-id="4275a-309">Response</span></span>
<span data-ttu-id="4275a-p130">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4275a-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4574

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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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



