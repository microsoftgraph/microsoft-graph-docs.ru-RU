# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="87ab0-101">Create windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="87ab0-101">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="87ab0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87ab0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87ab0-103">Создание объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87ab0-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="87ab0-104">Prerequisites</span></span>
<span data-ttu-id="87ab0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87ab0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87ab0-107">Permission type</span></span>|<span data-ttu-id="87ab0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87ab0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ab0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87ab0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="87ab0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ab0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87ab0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87ab0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ab0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ab0-112">Not supported.</span></span>|
|<span data-ttu-id="87ab0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87ab0-113">Application</span></span>|<span data-ttu-id="87ab0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ab0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ab0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87ab0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="87ab0-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87ab0-116">Request headers</span></span>
|<span data-ttu-id="87ab0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87ab0-117">Header</span></span>|<span data-ttu-id="87ab0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="87ab0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87ab0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="87ab0-119">Authorization</span></span>|<span data-ttu-id="87ab0-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87ab0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="87ab0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="87ab0-121">Accept</span></span>|<span data-ttu-id="87ab0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="87ab0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ab0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87ab0-123">Request body</span></span>
<span data-ttu-id="87ab0-124">В теле запроса добавьте представление объекта windowsInformationProtectionPolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87ab0-124">In the request body, supply a JSON representation of calendar object.</span></span>

<span data-ttu-id="87ab0-125">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="87ab0-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="87ab0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="87ab0-126">Property</span></span>|<span data-ttu-id="87ab0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="87ab0-127">Type</span></span>|<span data-ttu-id="87ab0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="87ab0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ab0-129">displayName</span><span class="sxs-lookup"><span data-stu-id="87ab0-129">displayName</span></span>|<span data-ttu-id="87ab0-130">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-130">String</span></span>|<span data-ttu-id="87ab0-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="87ab0-131">Policy display name.</span></span> <span data-ttu-id="87ab0-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-133">description</span><span class="sxs-lookup"><span data-stu-id="87ab0-133">description</span></span>|<span data-ttu-id="87ab0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-134">String</span></span>|<span data-ttu-id="87ab0-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="87ab0-135">The policy's description.</span></span> <span data-ttu-id="87ab0-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87ab0-137">createdDateTime</span></span>|<span data-ttu-id="87ab0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ab0-138">DateTimeOffset</span></span>|<span data-ttu-id="87ab0-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="87ab0-139">The date and time the group was created.</span></span> <span data-ttu-id="87ab0-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87ab0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="87ab0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ab0-142">DateTimeOffset</span></span>|<span data-ttu-id="87ab0-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="87ab0-143">Last time the policy was modified.</span></span> <span data-ttu-id="87ab0-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-145">id</span><span class="sxs-lookup"><span data-stu-id="87ab0-145">id</span></span>|<span data-ttu-id="87ab0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-146">String</span></span>|<span data-ttu-id="87ab0-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87ab0-147">Key of the setting.</span></span> <span data-ttu-id="87ab0-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-149">version</span><span class="sxs-lookup"><span data-stu-id="87ab0-149">version</span></span>|<span data-ttu-id="87ab0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-150">String</span></span>|<span data-ttu-id="87ab0-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="87ab0-151">Version of the entity.</span></span> <span data-ttu-id="87ab0-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="87ab0-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="87ab0-153">enforcementLevel</span></span>|<span data-ttu-id="87ab0-154">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-154">String</span></span>|<span data-ttu-id="87ab0-155">Уровень применения WIP. Поддерживаемые значения см. в определении Enum. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="87ab0-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="87ab0-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="87ab0-156">enterpriseDomain</span></span>|<span data-ttu-id="87ab0-157">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-157">String</span></span>|<span data-ttu-id="87ab0-158">Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="87ab0-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="87ab0-160">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-161">Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="87ab0-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="87ab0-163">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-163">Boolean</span></span>|<span data-ttu-id="87ab0-164">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="87ab0-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="87ab0-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="87ab0-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="87ab0-167">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="87ab0-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="87ab0-168">То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="87ab0-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="87ab0-170">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-170">Boolean</span></span>|<span data-ttu-id="87ab0-171">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="87ab0-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="87ab0-172">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="87ab0-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="87ab0-173">Если не отзывать ключи, отзываемые файлы не будут удаляться.</span><span class="sxs-lookup"><span data-stu-id="87ab0-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="87ab0-174">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="87ab0-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="87ab0-176">Guid</span><span class="sxs-lookup"><span data-stu-id="87ab0-176">Guid</span></span>|<span data-ttu-id="87ab0-177">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="87ab0-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="87ab0-178">Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="87ab0-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="87ab0-180">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-180">Boolean</span></span>|<span data-ttu-id="87ab0-181">Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="87ab0-182">iconsVisible</span></span>|<span data-ttu-id="87ab0-183">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-183">Boolean</span></span>|<span data-ttu-id="87ab0-184">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="87ab0-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="87ab0-185">Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="87ab0-186">protectedApps</span></span>|<span data-ttu-id="87ab0-187">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="87ab0-188">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="87ab0-189">exemptApps</span></span>|<span data-ttu-id="87ab0-190">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="87ab0-191">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="87ab0-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="87ab0-192">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="87ab0-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="87ab0-193">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="87ab0-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="87ab0-195">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-196">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="87ab0-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="87ab0-197">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="87ab0-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="87ab0-199">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="87ab0-200">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="87ab0-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="87ab0-201">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="87ab0-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="87ab0-202">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="87ab0-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="87ab0-203">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="87ab0-204">enterpriseIPRanges</span></span>|<span data-ttu-id="87ab0-205">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="87ab0-206">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="87ab0-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="87ab0-207">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="87ab0-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="87ab0-208">Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="87ab0-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="87ab0-210">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-210">Boolean</span></span>|<span data-ttu-id="87ab0-211">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="87ab0-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="87ab0-212">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="87ab0-213">enterpriseProxyServers</span></span>|<span data-ttu-id="87ab0-214">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-215">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="87ab0-215">This is a list of proxy servers.</span></span> <span data-ttu-id="87ab0-216">Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="87ab0-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="87ab0-218">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-219">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="87ab0-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="87ab0-220">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="87ab0-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="87ab0-221">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="87ab0-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="87ab0-222">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="87ab0-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="87ab0-223">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="87ab0-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="87ab0-225">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-225">Boolean</span></span>|<span data-ttu-id="87ab0-226">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="87ab0-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="87ab0-227">Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="87ab0-228">neutralDomainResources</span></span>|<span data-ttu-id="87ab0-229">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-230">Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="87ab0-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="87ab0-232">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-232">Boolean</span></span>|<span data-ttu-id="87ab0-233">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="87ab0-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="87ab0-235">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="87ab0-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="87ab0-236">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="87ab0-237">isAssigned</span></span>|<span data-ttu-id="87ab0-238">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-238">Boolean</span></span>|<span data-ttu-id="87ab0-239">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="87ab0-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="87ab0-240">Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="87ab0-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="87ab0-241">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="87ab0-241">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="87ab0-242">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-242">Boolean</span></span>|<span data-ttu-id="87ab0-243">Новое свойство в RS2, документация готовится</span><span class="sxs-lookup"><span data-stu-id="87ab0-243">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="87ab0-244">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="87ab0-244">mdmEnrollmentUrl</span></span>|<span data-ttu-id="87ab0-245">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-245">String</span></span>|<span data-ttu-id="87ab0-246">URL-адрес регистрации в системе MDM</span><span class="sxs-lookup"><span data-stu-id="87ab0-246">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="87ab0-247">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="87ab0-247">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="87ab0-248">Логический</span><span class="sxs-lookup"><span data-stu-id="87ab0-248">Boolean</span></span>|<span data-ttu-id="87ab0-249">Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="87ab0-249">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="87ab0-250">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="87ab0-250">pinMinimumLength</span></span>|<span data-ttu-id="87ab0-251">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-251">Int32</span></span>|<span data-ttu-id="87ab0-252">Целое число, которое определяет минимальное количество символов в ПИН-коде.</span><span class="sxs-lookup"><span data-stu-id="87ab0-252">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="87ab0-253">Значение по умолчанию — 4.</span><span class="sxs-lookup"><span data-stu-id="87ab0-253">Default value is 4.</span></span> <span data-ttu-id="87ab0-254">Для этого параметра политики можно установить значение в диапазоне от 4</span><span class="sxs-lookup"><span data-stu-id="87ab0-254">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="87ab0-255">до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).</span><span class="sxs-lookup"><span data-stu-id="87ab0-255">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="87ab0-256">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="87ab0-256">pinUppercaseLetters</span></span>|<span data-ttu-id="87ab0-257">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-257">String</span></span>|<span data-ttu-id="87ab0-258">Целое число, которое настраивает использование прописных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="87ab0-258">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="87ab0-259">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="87ab0-259">Default is NotAllow.</span></span> <span data-ttu-id="87ab0-260">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="87ab0-260">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="87ab0-261">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="87ab0-261">pinLowercaseLetters</span></span>|<span data-ttu-id="87ab0-262">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-262">String</span></span>|<span data-ttu-id="87ab0-263">Целое число, которое настраивает использование строчных букв в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="87ab0-263">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="87ab0-264">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="87ab0-264">Default is NotAllow.</span></span> <span data-ttu-id="87ab0-265">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="87ab0-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="87ab0-266">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="87ab0-266">pinSpecialCharacters</span></span>|<span data-ttu-id="87ab0-267">Строка</span><span class="sxs-lookup"><span data-stu-id="87ab0-267">String</span></span>|<span data-ttu-id="87ab0-268">Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="87ab0-268">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="87ab0-269">Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса:</span><span class="sxs-lookup"><span data-stu-id="87ab0-269">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="87ab0-270">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="87ab0-270">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="87ab0-271">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="87ab0-271">/ : ; < = > ?</span></span><span data-ttu-id="87ab0-272"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="87ab0-272"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="87ab0-273">} ~.</span><span class="sxs-lookup"><span data-stu-id="87ab0-273">=, ==</span></span> <span data-ttu-id="87ab0-274">Значение по умолчанию — NotAllow.</span><span class="sxs-lookup"><span data-stu-id="87ab0-274">Default is NotAllow.</span></span> <span data-ttu-id="87ab0-275">Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="87ab0-275">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="87ab0-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="87ab0-276">pinExpirationDays</span></span>|<span data-ttu-id="87ab0-277">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-277">Int32</span></span>|<span data-ttu-id="87ab0-278">Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения.</span><span class="sxs-lookup"><span data-stu-id="87ab0-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="87ab0-279">Для этого параметра политики нельзя установить значение выше 730.</span><span class="sxs-lookup"><span data-stu-id="87ab0-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="87ab0-280">Для этого параметра политики нельзя установить значение ниже 0.</span><span class="sxs-lookup"><span data-stu-id="87ab0-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="87ab0-281">Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает.</span><span class="sxs-lookup"><span data-stu-id="87ab0-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="87ab0-282">Этот узел был добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="87ab0-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="87ab0-283">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="87ab0-283">Default is 0.</span></span>|
|<span data-ttu-id="87ab0-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="87ab0-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="87ab0-285">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-285">Int32</span></span>|<span data-ttu-id="87ab0-286">Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить.</span><span class="sxs-lookup"><span data-stu-id="87ab0-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="87ab0-287">Для этого параметра политики нельзя установить значение выше 50.</span><span class="sxs-lookup"><span data-stu-id="87ab0-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="87ab0-288">Для этого параметра политики нельзя установить значение ниже 0.</span><span class="sxs-lookup"><span data-stu-id="87ab0-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="87ab0-289">Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется.</span><span class="sxs-lookup"><span data-stu-id="87ab0-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="87ab0-290">Этот узел был добавлен в Windows 10 версии 1511.</span><span class="sxs-lookup"><span data-stu-id="87ab0-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="87ab0-291">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="87ab0-291">Default is 0.</span></span>|
|<span data-ttu-id="87ab0-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="87ab0-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="87ab0-293">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-293">Int32</span></span>|<span data-ttu-id="87ab0-294">Количество неудачных попыток аутентификации до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="87ab0-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="87ab0-295">Значение 0 отключает функцию очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="87ab0-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="87ab0-296">Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="87ab0-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="87ab0-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="87ab0-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="87ab0-298">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-298">Int32</span></span>|<span data-ttu-id="87ab0-299">Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.</span><span class="sxs-lookup"><span data-stu-id="87ab0-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="87ab0-300">Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="87ab0-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="87ab0-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="87ab0-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="87ab0-302">Int32</span><span class="sxs-lookup"><span data-stu-id="87ab0-302">Int32</span></span>|<span data-ttu-id="87ab0-303">Время с момента последнего подключения к Интернету до очистки данных приложения (в днях)</span><span class="sxs-lookup"><span data-stu-id="87ab0-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="87ab0-304">Ответ</span><span class="sxs-lookup"><span data-stu-id="87ab0-304">Response</span></span>
<span data-ttu-id="87ab0-305">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87ab0-305">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ab0-306">Пример</span><span class="sxs-lookup"><span data-stu-id="87ab0-306">Example</span></span>
### <a name="request"></a><span data-ttu-id="87ab0-307">Запрос</span><span class="sxs-lookup"><span data-stu-id="87ab0-307">Request</span></span>
<span data-ttu-id="87ab0-308">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87ab0-308">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4466

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="87ab0-309">Ответ</span><span class="sxs-lookup"><span data-stu-id="87ab0-309">Response</span></span>
<span data-ttu-id="87ab0-p130">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87ab0-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



