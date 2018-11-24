# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="ed06d-101">Тип ресурса windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed06d-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="ed06d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed06d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed06d-103">Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.</span><span class="sxs-lookup"><span data-stu-id="ed06d-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="ed06d-104">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ed06d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ed06d-105">Methods</span></span>
|<span data-ttu-id="ed06d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ed06d-106">Method</span></span>|<span data-ttu-id="ed06d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed06d-107">Return Type</span></span>|<span data-ttu-id="ed06d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ed06d-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed06d-109">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed06d-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="ed06d-110">Коллекция объектов [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="ed06d-111">Список свойств и связей объектов [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="ed06d-112">Получение объекта windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed06d-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="ed06d-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="ed06d-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="ed06d-114">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-114">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="ed06d-115">Действие assign</span><span class="sxs-lookup"><span data-stu-id="ed06d-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="ed06d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ed06d-116">None</span></span>|<span data-ttu-id="ed06d-117">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ed06d-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ed06d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed06d-118">Properties</span></span>
|<span data-ttu-id="ed06d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed06d-119">Property</span></span>|<span data-ttu-id="ed06d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ed06d-120">Type</span></span>|<span data-ttu-id="ed06d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ed06d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed06d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ed06d-122">displayName</span></span>|<span data-ttu-id="ed06d-123">String</span><span class="sxs-lookup"><span data-stu-id="ed06d-123">String</span></span>|<span data-ttu-id="ed06d-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="ed06d-124">Policy display name.</span></span> <span data-ttu-id="ed06d-125">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-126">description</span><span class="sxs-lookup"><span data-stu-id="ed06d-126">description</span></span>|<span data-ttu-id="ed06d-127">String</span><span class="sxs-lookup"><span data-stu-id="ed06d-127">String</span></span>|<span data-ttu-id="ed06d-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="ed06d-128">The policy's description.</span></span> <span data-ttu-id="ed06d-129">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed06d-130">createdDateTime</span></span>|<span data-ttu-id="ed06d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed06d-131">DateTimeOffset</span></span>|<span data-ttu-id="ed06d-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="ed06d-132">The date and time the policy was created.</span></span> <span data-ttu-id="ed06d-133">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed06d-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ed06d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed06d-135">DateTimeOffset</span></span>|<span data-ttu-id="ed06d-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="ed06d-136">Last time the policy was modified.</span></span> <span data-ttu-id="ed06d-137">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-138">id</span><span class="sxs-lookup"><span data-stu-id="ed06d-138">id</span></span>|<span data-ttu-id="ed06d-139">String</span><span class="sxs-lookup"><span data-stu-id="ed06d-139">String</span></span>|<span data-ttu-id="ed06d-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed06d-140">Key of the entity.</span></span> <span data-ttu-id="ed06d-141">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-142">version</span><span class="sxs-lookup"><span data-stu-id="ed06d-142">version</span></span>|<span data-ttu-id="ed06d-143">String</span><span class="sxs-lookup"><span data-stu-id="ed06d-143">String</span></span>|<span data-ttu-id="ed06d-144">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ed06d-144">Version of the entity.</span></span> <span data-ttu-id="ed06d-145">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ed06d-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ed06d-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="ed06d-146">enforcementLevel</span></span>|[<span data-ttu-id="ed06d-147">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="ed06d-147">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="ed06d-148">Принудительное применение уровень НЗП. В разделе Определение перечисления для поддерживаемых значений.</span><span class="sxs-lookup"><span data-stu-id="ed06d-148">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="ed06d-149">Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="ed06d-149">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="ed06d-150">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="ed06d-150">enterpriseDomain</span></span>|<span data-ttu-id="ed06d-151">String</span><span class="sxs-lookup"><span data-stu-id="ed06d-151">String</span></span>|<span data-ttu-id="ed06d-152">Основной корпоративный домен.</span><span class="sxs-lookup"><span data-stu-id="ed06d-152">Primary enterprise domain</span></span>|
|<span data-ttu-id="ed06d-153">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="ed06d-153">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="ed06d-154">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-155">Список корпоративных доменов, которые необходимо защитить.</span><span class="sxs-lookup"><span data-stu-id="ed06d-155">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="ed06d-156">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="ed06d-156">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="ed06d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed06d-157">Boolean</span></span>|<span data-ttu-id="ed06d-158">Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом).</span><span class="sxs-lookup"><span data-stu-id="ed06d-158">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="ed06d-159">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ed06d-159">dataRecoveryCertificate</span></span>|[<span data-ttu-id="ed06d-160">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ed06d-160">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="ed06d-161">Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов.</span><span class="sxs-lookup"><span data-stu-id="ed06d-161">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="ed06d-162">То же, что сертификат DRA для шифрованной файловой системы (EFS).</span><span class="sxs-lookup"><span data-stu-id="ed06d-162">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="ed06d-163">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="ed06d-163">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="ed06d-164">Логический</span><span class="sxs-lookup"><span data-stu-id="ed06d-164">Boolean</span></span>|<span data-ttu-id="ed06d-165">Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления.</span><span class="sxs-lookup"><span data-stu-id="ed06d-165">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="ed06d-166">Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации.</span><span class="sxs-lookup"><span data-stu-id="ed06d-166">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="ed06d-167">Если ключи не отзываются, файлы не очищаются.</span><span class="sxs-lookup"><span data-stu-id="ed06d-167">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="ed06d-168">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="ed06d-168">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="ed06d-169">Guid</span><span class="sxs-lookup"><span data-stu-id="ed06d-169">Guid</span></span>|<span data-ttu-id="ed06d-170">GUID шаблона, используемый для шифрования RMS.</span><span class="sxs-lookup"><span data-stu-id="ed06d-170">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="ed06d-171">Шаблон RMS позволяет ИТ-администратору настроить доступ (и его длительность) к защищенному RMS файлу для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="ed06d-171">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="ed06d-172">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="ed06d-172">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="ed06d-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed06d-173">Boolean</span></span>|<span data-ttu-id="ed06d-174">Указывает, разрешать ли шифрование Azure RMS для WIP.</span><span class="sxs-lookup"><span data-stu-id="ed06d-174">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="ed06d-175">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="ed06d-175">iconsVisible</span></span>|<span data-ttu-id="ed06d-176">Логический</span><span class="sxs-lookup"><span data-stu-id="ed06d-176">Boolean</span></span>|<span data-ttu-id="ed06d-177">Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов WIP в Проводнике и плиток приложений только для предприятий в меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="ed06d-177">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="ed06d-178">Начиная с Windows 10 версии 1703, этот параметр также определяет, отображается ли значок WIP в заголовке окна защищенного приложения.</span><span class="sxs-lookup"><span data-stu-id="ed06d-178">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="ed06d-179">protectedApps</span><span class="sxs-lookup"><span data-stu-id="ed06d-179">protectedApps</span></span>|<span data-ttu-id="ed06d-180">Коллекция объектов [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="ed06d-181">Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются.</span><span class="sxs-lookup"><span data-stu-id="ed06d-181">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="ed06d-182">exemptApps</span><span class="sxs-lookup"><span data-stu-id="ed06d-182">exemptApps</span></span>|<span data-ttu-id="ed06d-183">Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="ed06d-184">Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются.</span><span class="sxs-lookup"><span data-stu-id="ed06d-184">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="ed06d-185">Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.</span><span class="sxs-lookup"><span data-stu-id="ed06d-185">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="ed06d-186">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="ed06d-186">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="ed06d-187">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-188">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="ed06d-188">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="ed06d-189">Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно.</span><span class="sxs-lookup"><span data-stu-id="ed06d-189">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="ed06d-190">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="ed06d-190">enterpriseProxiedDomains</span></span>|<span data-ttu-id="ed06d-191">Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="ed06d-192">Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать.</span><span class="sxs-lookup"><span data-stu-id="ed06d-192">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="ed06d-193">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="ed06d-193">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="ed06d-194">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="ed06d-194">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="ed06d-195">Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="ed06d-195">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="ed06d-196">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="ed06d-196">enterpriseIPRanges</span></span>|<span data-ttu-id="ed06d-197">Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="ed06d-198">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="ed06d-198">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="ed06d-199">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="ed06d-199">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="ed06d-200">Считается, что отправлять корпоративные данные на эти компьютеры безопасно.</span><span class="sxs-lookup"><span data-stu-id="ed06d-200">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="ed06d-201">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="ed06d-201">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="ed06d-202">Логический</span><span class="sxs-lookup"><span data-stu-id="ed06d-202">Boolean</span></span>|<span data-ttu-id="ed06d-203">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="ed06d-203">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="ed06d-204">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="ed06d-204">Default is false</span></span>|
|<span data-ttu-id="ed06d-205">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="ed06d-205">enterpriseProxyServers</span></span>|<span data-ttu-id="ed06d-206">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-207">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="ed06d-207">This is a list of proxy servers.</span></span> <span data-ttu-id="ed06d-208">Сервер, который не входит в этот список, не считается корпоративным.</span><span class="sxs-lookup"><span data-stu-id="ed06d-208">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="ed06d-209">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="ed06d-209">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="ed06d-210">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-211">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="ed06d-211">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="ed06d-212">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="ed06d-212">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="ed06d-213">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ed06d-213">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="ed06d-214">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="ed06d-214">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="ed06d-215">Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="ed06d-215">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="ed06d-216">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="ed06d-216">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="ed06d-217">Логический</span><span class="sxs-lookup"><span data-stu-id="ed06d-217">Boolean</span></span>|<span data-ttu-id="ed06d-218">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="ed06d-218">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="ed06d-219">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="ed06d-219">Default is false</span></span>|
|<span data-ttu-id="ed06d-220">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="ed06d-220">neutralDomainResources</span></span>|<span data-ttu-id="ed06d-221">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-222">Список доменных имен, которые можно использовать для рабочих или личных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ed06d-222">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="ed06d-223">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="ed06d-223">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="ed06d-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed06d-224">Boolean</span></span>|<span data-ttu-id="ed06d-225">Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы.</span><span class="sxs-lookup"><span data-stu-id="ed06d-225">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="ed06d-226">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="ed06d-226">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="ed06d-227">Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="ed06d-228">Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия.</span><span class="sxs-lookup"><span data-stu-id="ed06d-228">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="ed06d-229">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ed06d-229">isAssigned</span></span>|<span data-ttu-id="ed06d-230">Логический</span><span class="sxs-lookup"><span data-stu-id="ed06d-230">Boolean</span></span>|<span data-ttu-id="ed06d-231">Указывает, применена ли политика к группам включения.</span><span class="sxs-lookup"><span data-stu-id="ed06d-231">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed06d-232">Связи</span><span class="sxs-lookup"><span data-stu-id="ed06d-232">Relationships</span></span>
|<span data-ttu-id="ed06d-233">Связь</span><span class="sxs-lookup"><span data-stu-id="ed06d-233">Relationship</span></span>|<span data-ttu-id="ed06d-234">Тип</span><span class="sxs-lookup"><span data-stu-id="ed06d-234">Type</span></span>|<span data-ttu-id="ed06d-235">Описание</span><span class="sxs-lookup"><span data-stu-id="ed06d-235">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed06d-236">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="ed06d-236">protectedAppLockerFiles</span></span>|<span data-ttu-id="ed06d-237">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="ed06d-238">Еще один способ ввести данные о защищенных приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="ed06d-238">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="ed06d-239">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="ed06d-239">exemptAppLockerFiles</span></span>|<span data-ttu-id="ed06d-240">Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="ed06d-241">Еще один способ ввести данные об исключаемых приложениях с помощью XML-файлов.</span><span class="sxs-lookup"><span data-stu-id="ed06d-241">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="ed06d-242">assignments</span><span class="sxs-lookup"><span data-stu-id="ed06d-242">assignments</span></span>|<span data-ttu-id="ed06d-243">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ed06d-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="ed06d-244">Список групп безопасности, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="ed06d-244">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed06d-245">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed06d-245">JSON Representation</span></span>
<span data-ttu-id="ed06d-246">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed06d-246">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



