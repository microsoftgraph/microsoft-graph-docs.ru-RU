# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="7c679-101">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="7c679-101">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="7c679-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7c679-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c679-103">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-103">Update the properties of a [calendar](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c679-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="7c679-104">Prerequisites</span></span>
<span data-ttu-id="7c679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c679-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c679-107">Permission type</span></span>|<span data-ttu-id="7c679-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c679-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c679-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c679-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7c679-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c679-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c679-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c679-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c679-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c679-112">Not supported.</span></span>|
|<span data-ttu-id="7c679-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c679-113">Application</span></span>|<span data-ttu-id="7c679-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c679-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c679-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c679-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7c679-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c679-116">Request headers</span></span>
|<span data-ttu-id="7c679-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c679-117">Header</span></span>|<span data-ttu-id="7c679-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7c679-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c679-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c679-119">Authorization</span></span>|<span data-ttu-id="7c679-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c679-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c679-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7c679-121">Accept</span></span>|<span data-ttu-id="7c679-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7c679-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c679-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c679-123">Request body</span></span>
<span data-ttu-id="7c679-124">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c679-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="7c679-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7c679-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c679-126">Property</span></span>|<span data-ttu-id="7c679-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7c679-127">Type</span></span>|<span data-ttu-id="7c679-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7c679-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c679-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7c679-129">displayName</span></span>|<span data-ttu-id="7c679-130">String</span><span class="sxs-lookup"><span data-stu-id="7c679-130">String</span></span>|<span data-ttu-id="7c679-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="7c679-131">Policy display name.</span></span> <span data-ttu-id="7c679-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-133">description</span><span class="sxs-lookup"><span data-stu-id="7c679-133">description</span></span>|<span data-ttu-id="7c679-134">String</span><span class="sxs-lookup"><span data-stu-id="7c679-134">String</span></span>|<span data-ttu-id="7c679-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="7c679-135">The policy's description.</span></span> <span data-ttu-id="7c679-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c679-137">createdDateTime</span></span>|<span data-ttu-id="7c679-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c679-138">DateTimeOffset</span></span>|<span data-ttu-id="7c679-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="7c679-139">The date and time the group was created.</span></span> <span data-ttu-id="7c679-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c679-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7c679-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c679-142">DateTimeOffset</span></span>|<span data-ttu-id="7c679-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="7c679-143">Last time the policy was modified.</span></span> <span data-ttu-id="7c679-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-145">id</span><span class="sxs-lookup"><span data-stu-id="7c679-145">id</span></span>|<span data-ttu-id="7c679-146">String</span><span class="sxs-lookup"><span data-stu-id="7c679-146">String</span></span>|<span data-ttu-id="7c679-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7c679-147">Key of the setting.</span></span> <span data-ttu-id="7c679-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-149">version</span><span class="sxs-lookup"><span data-stu-id="7c679-149">version</span></span>|<span data-ttu-id="7c679-150">String</span><span class="sxs-lookup"><span data-stu-id="7c679-150">String</span></span>|<span data-ttu-id="7c679-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="7c679-151">Version of the entity.</span></span> <span data-ttu-id="7c679-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c679-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="7c679-153">enforcementLevel</span></span>|<span data-ttu-id="7c679-154">String</span><span class="sxs-lookup"><span data-stu-id="7c679-154">String</span></span>|<span data-ttu-id="7c679-155">Уровень применения WIP. Поддерживаемые значения см. в определении Enum. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="7c679-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="7c679-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="7c679-156">enterpriseDomain</span></span>|<span data-ttu-id="7c679-157">String</span><span class="sxs-lookup"><span data-stu-id="7c679-157">String</span></span>|<span data-ttu-id="7c679-158">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="7c679-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="7c679-160">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-161">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="7c679-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="7c679-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-163">Boolean</span></span>|<span data-ttu-id="7c679-164">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="7c679-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="7c679-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="7c679-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="7c679-167">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="7c679-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="7c679-168">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="7c679-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="7c679-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-170">Boolean</span></span>|<span data-ttu-id="7c679-171">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="7c679-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="7c679-172">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="7c679-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="7c679-173">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="7c679-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="7c679-174">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="7c679-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="7c679-176">Guid</span><span class="sxs-lookup"><span data-stu-id="7c679-176">Guid</span></span>|<span data-ttu-id="7c679-177">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="7c679-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="7c679-178">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="7c679-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="7c679-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-180">Boolean</span></span>|<span data-ttu-id="7c679-181">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="7c679-182">iconsVisible</span></span>|<span data-ttu-id="7c679-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-183">Boolean</span></span>|<span data-ttu-id="7c679-184">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="7c679-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="7c679-185">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="7c679-186">protectedApps</span></span>|<span data-ttu-id="7c679-187">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="7c679-188">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="7c679-189">exemptApps</span></span>|<span data-ttu-id="7c679-190">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="7c679-191">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="7c679-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="7c679-192">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="7c679-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="7c679-193">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="7c679-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="7c679-195">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-196">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="7c679-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="7c679-197">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="7c679-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="7c679-199">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="7c679-200">Содержит список доменов корпоративных ресурсов, размещенных в облаке, которые нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="7c679-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="7c679-201">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="7c679-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="7c679-202">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="7c679-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="7c679-203">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="7c679-204">enterpriseIPRanges</span></span>|<span data-ttu-id="7c679-205">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="7c679-206">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="7c679-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="7c679-207">Данные, поступающие с этих компьютеров, защищены и считаются корпоративными.</span><span class="sxs-lookup"><span data-stu-id="7c679-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="7c679-208">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="7c679-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="7c679-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-210">Boolean</span></span>|<span data-ttu-id="7c679-211">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="7c679-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="7c679-212">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="7c679-213">enterpriseProxyServers</span></span>|<span data-ttu-id="7c679-214">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-215">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="7c679-215">This is a list of proxy servers.</span></span> <span data-ttu-id="7c679-216">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="7c679-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="7c679-218">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-219">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="7c679-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="7c679-220">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="7c679-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="7c679-221">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="7c679-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="7c679-222">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="7c679-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="7c679-223">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="7c679-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="7c679-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-225">Boolean</span></span>|<span data-ttu-id="7c679-226">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="7c679-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="7c679-227">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="7c679-228">neutralDomainResources</span></span>|<span data-ttu-id="7c679-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-230">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="7c679-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="7c679-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-232">Boolean</span></span>|<span data-ttu-id="7c679-233">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="7c679-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="7c679-235">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7c679-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="7c679-236">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="7c679-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7c679-237">isAssigned</span></span>|<span data-ttu-id="7c679-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c679-238">Boolean</span></span>|<span data-ttu-id="7c679-239">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="7c679-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="7c679-240">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7c679-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7c679-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c679-241">Response</span></span>
<span data-ttu-id="7c679-242">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7c679-242">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c679-243">Пример</span><span class="sxs-lookup"><span data-stu-id="7c679-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c679-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c679-244">Request</span></span>
<span data-ttu-id="7c679-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c679-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3890

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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="7c679-246">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c679-246">Response</span></span>
<span data-ttu-id="7c679-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7c679-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4074

{
  "@odata.type": "#microsoft.intune_mam_graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```



