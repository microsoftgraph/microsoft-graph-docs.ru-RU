# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="fd680-101">Обновление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd680-101">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="fd680-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd680-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd680-103">Обновляет свойства объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-103">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd680-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="fd680-104">Prerequisites</span></span>
<span data-ttu-id="fd680-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd680-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd680-107">Permission type</span></span>|<span data-ttu-id="fd680-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd680-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd680-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd680-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd680-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd680-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd680-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd680-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd680-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd680-112">Not supported.</span></span>|
|<span data-ttu-id="fd680-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd680-113">Application</span></span>|<span data-ttu-id="fd680-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd680-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd680-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd680-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fd680-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd680-116">Request headers</span></span>
|<span data-ttu-id="fd680-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd680-117">Header</span></span>|<span data-ttu-id="fd680-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fd680-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd680-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd680-119">Authorization</span></span>|<span data-ttu-id="fd680-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fd680-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd680-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fd680-121">Accept</span></span>|<span data-ttu-id="fd680-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fd680-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd680-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd680-123">Request body</span></span>
<span data-ttu-id="fd680-124">В теле запроса добавьте представление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd680-124">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="fd680-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-125">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="fd680-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd680-126">Property</span></span>|<span data-ttu-id="fd680-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fd680-127">Type</span></span>|<span data-ttu-id="fd680-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fd680-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd680-129">displayName</span><span class="sxs-lookup"><span data-stu-id="fd680-129">displayName</span></span>|<span data-ttu-id="fd680-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fd680-130">String</span></span>|<span data-ttu-id="fd680-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="fd680-131">Policy display name.</span></span> <span data-ttu-id="fd680-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-133">description</span><span class="sxs-lookup"><span data-stu-id="fd680-133">description</span></span>|<span data-ttu-id="fd680-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fd680-134">String</span></span>|<span data-ttu-id="fd680-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="fd680-135">The policy's description.</span></span> <span data-ttu-id="fd680-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd680-137">createdDateTime</span></span>|<span data-ttu-id="fd680-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd680-138">DateTimeOffset</span></span>|<span data-ttu-id="fd680-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="fd680-139">The date and time the policy was created.</span></span> <span data-ttu-id="fd680-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd680-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fd680-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd680-142">DateTimeOffset</span></span>|<span data-ttu-id="fd680-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="fd680-143">Last time the policy was modified.</span></span> <span data-ttu-id="fd680-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-145">id</span><span class="sxs-lookup"><span data-stu-id="fd680-145">id</span></span>|<span data-ttu-id="fd680-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fd680-146">String</span></span>|<span data-ttu-id="fd680-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fd680-147">Key of the entity.</span></span> <span data-ttu-id="fd680-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-149">version</span><span class="sxs-lookup"><span data-stu-id="fd680-149">version</span></span>|<span data-ttu-id="fd680-150">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fd680-150">String</span></span>|<span data-ttu-id="fd680-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="fd680-151">Version of the entity.</span></span> <span data-ttu-id="fd680-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="fd680-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fd680-153">enforcementLevel</span></span>|[<span data-ttu-id="fd680-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fd680-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="fd680-155">Принудительное применение уровня WIP. См. определение перечисления для поддерживаемых значений, унаследованных от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: , , , .</span></span> <span data-ttu-id="fd680-156">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="fd680-156">The possible values are `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`, , , , , , , , or .</span></span>|
|<span data-ttu-id="fd680-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="fd680-157">enterpriseDomain</span></span>|<span data-ttu-id="fd680-158">String (строка)</span><span class="sxs-lookup"><span data-stu-id="fd680-158">String</span></span>|<span data-ttu-id="fd680-159">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-159">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="fd680-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="fd680-161">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-162">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-162">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="fd680-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="fd680-164">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-164">Boolean</span></span>|<span data-ttu-id="fd680-165">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd680-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="fd680-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd680-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="fd680-168">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="fd680-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="fd680-169">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="fd680-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="fd680-171">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-171">Boolean</span></span>|<span data-ttu-id="fd680-172">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="fd680-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="fd680-173">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="fd680-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="fd680-174">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="fd680-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="fd680-175">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-175">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="fd680-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="fd680-177">Guid</span><span class="sxs-lookup"><span data-stu-id="fd680-177">Guid</span></span>|<span data-ttu-id="fd680-178">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="fd680-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="fd680-179">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="fd680-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="fd680-181">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-181">Boolean</span></span>|<span data-ttu-id="fd680-182">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-182">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="fd680-183">iconsVisible</span></span>|<span data-ttu-id="fd680-184">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-184">Boolean</span></span>|<span data-ttu-id="fd680-185">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="fd680-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="fd680-186">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="fd680-187">protectedApps</span></span>|<span data-ttu-id="fd680-188">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fd680-189">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="fd680-190">exemptApps</span></span>|<span data-ttu-id="fd680-191">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fd680-192">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="fd680-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="fd680-193">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="fd680-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="fd680-194">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-194">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-195">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="fd680-195">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="fd680-196">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-197">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="fd680-197">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="fd680-198">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-198">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-199">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fd680-199">enterpriseProxiedDomains</span></span>|<span data-ttu-id="fd680-200">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="fd680-201">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="fd680-201">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="fd680-202">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="fd680-202">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="fd680-203">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="fd680-203">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="fd680-204">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-204">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-205">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="fd680-205">enterpriseIPRanges</span></span>|<span data-ttu-id="fd680-206">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="fd680-207">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="fd680-207">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="fd680-208">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="fd680-208">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="fd680-209">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-209">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-210">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fd680-210">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="fd680-211">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-211">Boolean</span></span>|<span data-ttu-id="fd680-212">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="fd680-212">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="fd680-213">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-213">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-214">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="fd680-214">enterpriseProxyServers</span></span>|<span data-ttu-id="fd680-215">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-216">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="fd680-216">This is a list of proxy servers.</span></span> <span data-ttu-id="fd680-217">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-217">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-218">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="fd680-218">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="fd680-219">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-220">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="fd680-220">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="fd680-221">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="fd680-221">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="fd680-222">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="fd680-222">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="fd680-223">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="fd680-223">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="fd680-224">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-224">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-225">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fd680-225">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="fd680-226">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-226">Boolean</span></span>|<span data-ttu-id="fd680-227">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="fd680-227">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="fd680-228">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-228">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-229">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="fd680-229">neutralDomainResources</span></span>|<span data-ttu-id="fd680-230">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-231">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-231">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-232">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="fd680-232">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="fd680-233">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-233">Boolean</span></span>|<span data-ttu-id="fd680-234">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-234">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-235">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="fd680-235">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="fd680-236">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fd680-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fd680-237">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-237">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fd680-238">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fd680-238">isAssigned</span></span>|<span data-ttu-id="fd680-239">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fd680-239">Boolean</span></span>|<span data-ttu-id="fd680-240">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="fd680-240">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="fd680-241">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd680-241">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fd680-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd680-242">Response</span></span>
<span data-ttu-id="fd680-243">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fd680-243">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd680-244">Пример</span><span class="sxs-lookup"><span data-stu-id="fd680-244">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd680-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd680-245">Request</span></span>
<span data-ttu-id="fd680-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd680-246">Here is an example of the request.</span></span>
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
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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

### <a name="response"></a><span data-ttu-id="fd680-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd680-247">Response</span></span>
<span data-ttu-id="fd680-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd680-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4074

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
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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



