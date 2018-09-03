# <a name="create-manageddevice"></a><span data-ttu-id="03f12-101">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="03f12-101">Create managedDevice</span></span>

> <span data-ttu-id="03f12-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03f12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03f12-103">Создание объекта [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="03f12-103">Create a new [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03f12-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="03f12-104">Prerequisites</span></span>
<span data-ttu-id="03f12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03f12-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03f12-107">Permission type</span></span>|<span data-ttu-id="03f12-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03f12-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03f12-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03f12-109">Delegated (work or school account)</span></span>|<span data-ttu-id="03f12-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f12-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03f12-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03f12-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03f12-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f12-112">Not supported.</span></span>|
|<span data-ttu-id="03f12-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03f12-113">Application</span></span>|<span data-ttu-id="03f12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f12-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03f12-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03f12-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="03f12-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03f12-116">Request headers</span></span>
|<span data-ttu-id="03f12-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03f12-117">Header</span></span>|<span data-ttu-id="03f12-118">Значение</span><span class="sxs-lookup"><span data-stu-id="03f12-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03f12-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03f12-119">Authorization</span></span>|<span data-ttu-id="03f12-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="03f12-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03f12-121">Accept</span><span class="sxs-lookup"><span data-stu-id="03f12-121">Accept</span></span>|<span data-ttu-id="03f12-122">application/json</span><span class="sxs-lookup"><span data-stu-id="03f12-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03f12-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03f12-123">Request body</span></span>
<span data-ttu-id="03f12-124">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03f12-124">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="03f12-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="03f12-125">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="03f12-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="03f12-126">Property</span></span>|<span data-ttu-id="03f12-127">Тип</span><span class="sxs-lookup"><span data-stu-id="03f12-127">Type</span></span>|<span data-ttu-id="03f12-128">Описание</span><span class="sxs-lookup"><span data-stu-id="03f12-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f12-129">id</span><span class="sxs-lookup"><span data-stu-id="03f12-129">id</span></span>|<span data-ttu-id="03f12-130">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-130">String</span></span>|<span data-ttu-id="03f12-131">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="03f12-132">userId</span><span class="sxs-lookup"><span data-stu-id="03f12-132">userId</span></span>|<span data-ttu-id="03f12-133">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-133">String</span></span>|<span data-ttu-id="03f12-134">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="03f12-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="03f12-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="03f12-135">deviceName</span></span>|<span data-ttu-id="03f12-136">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-136">String</span></span>|<span data-ttu-id="03f12-137">Название устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-137">Name of the device</span></span>|
|<span data-ttu-id="03f12-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="03f12-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="03f12-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="03f12-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="03f12-140">Владение устройством.</span><span class="sxs-lookup"><span data-stu-id="03f12-140">Ownership of the device.</span></span> <span data-ttu-id="03f12-141">Может быть "company" (компании) или "personal" (личное).</span><span class="sxs-lookup"><span data-stu-id="03f12-141">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="03f12-142">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="03f12-142">The possible values are `unknown`, `company`, `personal`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="03f12-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="03f12-143">deviceActionResults</span></span>|<span data-ttu-id="03f12-144">Коллекция [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="03f12-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="03f12-145">Список объектов deviceActionResult сложного типа.</span><span class="sxs-lookup"><span data-stu-id="03f12-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="03f12-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="03f12-146">enrolledDateTime</span></span>|<span data-ttu-id="03f12-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f12-147">DateTimeOffset</span></span>|<span data-ttu-id="03f12-148">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="03f12-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="03f12-149">lastSyncDateTime</span></span>|<span data-ttu-id="03f12-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f12-150">DateTimeOffset</span></span>|<span data-ttu-id="03f12-151">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="03f12-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="03f12-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="03f12-152">operatingSystem</span></span>|<span data-ttu-id="03f12-153">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-153">String</span></span>|<span data-ttu-id="03f12-154">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-154">Operating system of the device.</span></span> <span data-ttu-id="03f12-155">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="03f12-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="03f12-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="03f12-156">complianceState</span></span>|[<span data-ttu-id="03f12-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="03f12-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="03f12-158">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="03f12-158">Compliance state of the device.</span></span> <span data-ttu-id="03f12-159">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="03f12-159">The possible values are `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`, , , , , or .</span></span>|
|<span data-ttu-id="03f12-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="03f12-160">jailBroken</span></span>|<span data-ttu-id="03f12-161">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-161">String</span></span>|<span data-ttu-id="03f12-162">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="03f12-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="03f12-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="03f12-163">managementAgent</span></span>|[<span data-ttu-id="03f12-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="03f12-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="03f12-165">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="03f12-165">Management channel of the device.</span></span> <span data-ttu-id="03f12-166">Intune, EAS, и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="03f12-166">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="03f12-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="03f12-167">osVersion</span></span>|<span data-ttu-id="03f12-168">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-168">String</span></span>|<span data-ttu-id="03f12-169">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="03f12-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="03f12-170">easActivated</span></span>|<span data-ttu-id="03f12-171">Логический</span><span class="sxs-lookup"><span data-stu-id="03f12-171">Boolean</span></span>|<span data-ttu-id="03f12-172">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="03f12-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="03f12-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="03f12-173">easDeviceId</span></span>|<span data-ttu-id="03f12-174">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-174">String</span></span>|<span data-ttu-id="03f12-175">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="03f12-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="03f12-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="03f12-176">easActivationDateTime</span></span>|<span data-ttu-id="03f12-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f12-177">DateTimeOffset</span></span>|<span data-ttu-id="03f12-178">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="03f12-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="03f12-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="03f12-179">azureADRegistered</span></span>|<span data-ttu-id="03f12-180">Логический</span><span class="sxs-lookup"><span data-stu-id="03f12-180">Boolean</span></span>|<span data-ttu-id="03f12-181">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03f12-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="03f12-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="03f12-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="03f12-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="03f12-183">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="03f12-184">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-184">Enrollment type of the device.</span></span> <span data-ttu-id="03f12-185">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="03f12-185">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="03f12-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="03f12-186">activationLockBypassCode</span></span>|<span data-ttu-id="03f12-187">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-187">String</span></span>|<span data-ttu-id="03f12-188">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="03f12-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="03f12-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="03f12-189">emailAddress</span></span>|<span data-ttu-id="03f12-190">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-190">String</span></span>|<span data-ttu-id="03f12-191">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="03f12-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="03f12-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="03f12-192">azureADDeviceId</span></span>|<span data-ttu-id="03f12-193">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-193">String</span></span>|<span data-ttu-id="03f12-194">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03f12-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="03f12-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03f12-195">Read only.</span></span>|
|<span data-ttu-id="03f12-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="03f12-196">deviceRegistrationState</span></span>|[<span data-ttu-id="03f12-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="03f12-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="03f12-198">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-198">Device registration state.</span></span> <span data-ttu-id="03f12-199">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="03f12-199">The possible values are `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`, , , , or .</span></span>|
|<span data-ttu-id="03f12-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="03f12-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="03f12-201">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-201">String</span></span>|<span data-ttu-id="03f12-202">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-202">Device category display name</span></span>|
|<span data-ttu-id="03f12-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="03f12-203">isSupervised</span></span>|<span data-ttu-id="03f12-204">Логический</span><span class="sxs-lookup"><span data-stu-id="03f12-204">Boolean</span></span>|<span data-ttu-id="03f12-205">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-205">Device supervised status</span></span>|
|<span data-ttu-id="03f12-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="03f12-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="03f12-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f12-207">DateTimeOffset</span></span>|<span data-ttu-id="03f12-208">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="03f12-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="03f12-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="03f12-209">exchangeAccessState</span></span>|[<span data-ttu-id="03f12-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="03f12-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="03f12-211">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="03f12-211">The Access State of the device in Exchange.</span></span> <span data-ttu-id="03f12-212">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="03f12-212">The possible values are `none`, `unknown`, `allowed`, `blocked`, `quarantined`, , , , , , , or .</span></span>|
|<span data-ttu-id="03f12-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="03f12-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="03f12-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="03f12-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="03f12-215">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="03f12-215">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="03f12-216">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="03f12-216">The possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="03f12-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="03f12-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="03f12-218">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-218">String</span></span>|<span data-ttu-id="03f12-219">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="03f12-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="03f12-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="03f12-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="03f12-221">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-221">String</span></span>|<span data-ttu-id="03f12-222">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="03f12-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="03f12-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="03f12-223">isEncrypted</span></span>|<span data-ttu-id="03f12-224">Логический</span><span class="sxs-lookup"><span data-stu-id="03f12-224">Boolean</span></span>|<span data-ttu-id="03f12-225">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-225">Device encryption status</span></span>|
|<span data-ttu-id="03f12-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03f12-226">userPrincipalName</span></span>|<span data-ttu-id="03f12-227">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-227">String</span></span>|<span data-ttu-id="03f12-228">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-228">Device user principal name</span></span>|
|<span data-ttu-id="03f12-229">model</span><span class="sxs-lookup"><span data-stu-id="03f12-229">model</span></span>|<span data-ttu-id="03f12-230">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-230">String</span></span>|<span data-ttu-id="03f12-231">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-231">Model of the device</span></span>|
|<span data-ttu-id="03f12-232">manufacturer</span><span class="sxs-lookup"><span data-stu-id="03f12-232">manufacturer</span></span>|<span data-ttu-id="03f12-233">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-233">String</span></span>|<span data-ttu-id="03f12-234">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="03f12-235">imei</span><span class="sxs-lookup"><span data-stu-id="03f12-235">imei</span></span>|<span data-ttu-id="03f12-236">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-236">String</span></span>|<span data-ttu-id="03f12-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="03f12-237">IMEI</span></span>|
|<span data-ttu-id="03f12-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="03f12-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="03f12-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f12-239">DateTimeOffset</span></span>|<span data-ttu-id="03f12-240">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="03f12-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="03f12-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="03f12-241">serialNumber</span></span>|<span data-ttu-id="03f12-242">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-242">String</span></span>|<span data-ttu-id="03f12-243">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="03f12-243">SerialNumber</span></span>|
|<span data-ttu-id="03f12-244">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="03f12-244">phoneNumber</span></span>|<span data-ttu-id="03f12-245">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-245">String</span></span>|<span data-ttu-id="03f12-246">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="03f12-246">Phone number of the device</span></span>|
|<span data-ttu-id="03f12-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="03f12-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="03f12-248">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-248">String</span></span>|<span data-ttu-id="03f12-249">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="03f12-249">Android security patch level</span></span>|
|<span data-ttu-id="03f12-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="03f12-250">userDisplayName</span></span>|<span data-ttu-id="03f12-251">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-251">String</span></span>|<span data-ttu-id="03f12-252">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="03f12-252">User display name</span></span>|
|<span data-ttu-id="03f12-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="03f12-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="03f12-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="03f12-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="03f12-255">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="03f12-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="03f12-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="03f12-256">wiFiMacAddress</span></span>|<span data-ttu-id="03f12-257">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-257">String</span></span>|<span data-ttu-id="03f12-258">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="03f12-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="03f12-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="03f12-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="03f12-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="03f12-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="03f12-261">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-261">The device health attestation state.</span></span>|
|<span data-ttu-id="03f12-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="03f12-262">subscriberCarrier</span></span>|<span data-ttu-id="03f12-263">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-263">String</span></span>|<span data-ttu-id="03f12-264">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="03f12-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="03f12-265">meid</span><span class="sxs-lookup"><span data-stu-id="03f12-265">meid</span></span>|<span data-ttu-id="03f12-266">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-266">String</span></span>|<span data-ttu-id="03f12-267">MEID</span><span class="sxs-lookup"><span data-stu-id="03f12-267">MEID</span></span>|
|<span data-ttu-id="03f12-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="03f12-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="03f12-269">Int64</span><span class="sxs-lookup"><span data-stu-id="03f12-269">Int64</span></span>|<span data-ttu-id="03f12-270">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="03f12-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="03f12-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="03f12-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="03f12-272">Int64</span><span class="sxs-lookup"><span data-stu-id="03f12-272">Int64</span></span>|<span data-ttu-id="03f12-273">Свободный объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="03f12-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="03f12-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="03f12-274">managedDeviceName</span></span>|<span data-ttu-id="03f12-275">Строка​</span><span class="sxs-lookup"><span data-stu-id="03f12-275">String</span></span>|<span data-ttu-id="03f12-276">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="03f12-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="03f12-277">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="03f12-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="03f12-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="03f12-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="03f12-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="03f12-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="03f12-280">Указывает состояние подверженности устройства угрозам при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).</span><span class="sxs-lookup"><span data-stu-id="03f12-280">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="03f12-281">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03f12-281">Read Only.</span></span> <span data-ttu-id="03f12-282">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="03f12-282">The possible values are `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="03f12-283">Ответ</span><span class="sxs-lookup"><span data-stu-id="03f12-283">Response</span></span>
<span data-ttu-id="03f12-284">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune_devices_manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03f12-284">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03f12-285">Пример</span><span class="sxs-lookup"><span data-stu-id="03f12-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="03f12-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="03f12-286">Request</span></span>
<span data-ttu-id="03f12-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03f12-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="03f12-288">Ответ</span><span class="sxs-lookup"><span data-stu-id="03f12-288">Response</span></span>
<span data-ttu-id="03f12-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03f12-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```



