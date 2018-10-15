# <a name="update-manageddevice"></a><span data-ttu-id="61870-101">Обновление managedDevice</span><span class="sxs-lookup"><span data-stu-id="61870-101">Update managedDevice</span></span>

> <span data-ttu-id="61870-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="61870-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61870-103">Обновление свойств объекта [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="61870-103">Update the properties of a [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61870-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61870-104">Prerequisites</span></span>
<span data-ttu-id="61870-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61870-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61870-107">Permission type</span></span>|<span data-ttu-id="61870-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61870-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61870-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61870-109">Delegated (work or school account)</span></span>|<span data-ttu-id="61870-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61870-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61870-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61870-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61870-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61870-112">Not supported.</span></span>|
|<span data-ttu-id="61870-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61870-113">Application</span></span>|<span data-ttu-id="61870-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61870-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61870-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61870-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="61870-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61870-116">Request headers</span></span>
|<span data-ttu-id="61870-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61870-117">Header</span></span>|<span data-ttu-id="61870-118">Значение</span><span class="sxs-lookup"><span data-stu-id="61870-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61870-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61870-119">Authorization</span></span>|<span data-ttu-id="61870-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="61870-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61870-121">Принять</span><span class="sxs-lookup"><span data-stu-id="61870-121">Accept</span></span>|<span data-ttu-id="61870-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="61870-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61870-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61870-123">Request body</span></span>
<span data-ttu-id="61870-124">В теле запроса добавьте представление объекта [managedDevice](../resources/intune_devices_manageddevice.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61870-124">In the request body, supply a JSON representation for the [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="61870-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="61870-125">The following table shows the properties that are required when you create the [managedDevice](../resources/intune_devices_manageddevice.md).</span></span>

|<span data-ttu-id="61870-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="61870-126">Property</span></span>|<span data-ttu-id="61870-127">Тип</span><span class="sxs-lookup"><span data-stu-id="61870-127">Type</span></span>|<span data-ttu-id="61870-128">Описание</span><span class="sxs-lookup"><span data-stu-id="61870-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61870-129">ИД</span><span class="sxs-lookup"><span data-stu-id="61870-129">id</span></span>|<span data-ttu-id="61870-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-130">String</span></span>|<span data-ttu-id="61870-131">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="61870-132">userId</span><span class="sxs-lookup"><span data-stu-id="61870-132">userId</span></span>|<span data-ttu-id="61870-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-133">String</span></span>|<span data-ttu-id="61870-134">Уникальный идентификатор пользователя, связанного с устройством.</span><span class="sxs-lookup"><span data-stu-id="61870-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="61870-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="61870-135">deviceName</span></span>|<span data-ttu-id="61870-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-136">String</span></span>|<span data-ttu-id="61870-137">Название устройства</span><span class="sxs-lookup"><span data-stu-id="61870-137">Name of the device</span></span>|
|<span data-ttu-id="61870-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="61870-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="61870-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="61870-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="61870-p102">Владение устройством. Может быть "компания" или "личное". Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="61870-p102">Ownership of the device. Can be 'company' or 'personal'. The possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="61870-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="61870-143">deviceActionResults</span></span>|<span data-ttu-id="61870-144">Коллекция [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="61870-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="61870-145">Список объектов deviceActionResult сложного типа.</span><span class="sxs-lookup"><span data-stu-id="61870-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="61870-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="61870-146">enrolledDateTime</span></span>|<span data-ttu-id="61870-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61870-147">DateTimeOffset</span></span>|<span data-ttu-id="61870-148">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="61870-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="61870-149">lastSyncDateTime</span></span>|<span data-ttu-id="61870-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61870-150">DateTimeOffset</span></span>|<span data-ttu-id="61870-151">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="61870-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="61870-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="61870-152">operatingSystem</span></span>|<span data-ttu-id="61870-153">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-153">String</span></span>|<span data-ttu-id="61870-154">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-154">Operating system of the device.</span></span> <span data-ttu-id="61870-155">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="61870-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="61870-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="61870-156">complianceState</span></span>|[<span data-ttu-id="61870-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="61870-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="61870-p104">Состояние соответствия устройства требованиям. Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="61870-p104">Compliance state of the device. The possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="61870-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="61870-160">jailBroken</span></span>|<span data-ttu-id="61870-161">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-161">String</span></span>|<span data-ttu-id="61870-162">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="61870-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="61870-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="61870-163">managementAgent</span></span>|[<span data-ttu-id="61870-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="61870-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="61870-p105">Канал управления устройством. Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="61870-p105">Management channel of the device. Intune, EAS, etc. The possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="61870-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="61870-167">osVersion</span></span>|<span data-ttu-id="61870-168">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-168">String</span></span>|<span data-ttu-id="61870-169">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="61870-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="61870-170">easActivated</span></span>|<span data-ttu-id="61870-171">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="61870-171">Boolean</span></span>|<span data-ttu-id="61870-172">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="61870-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="61870-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="61870-173">easDeviceId</span></span>|<span data-ttu-id="61870-174">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-174">String</span></span>|<span data-ttu-id="61870-175">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="61870-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="61870-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="61870-176">easActivationDateTime</span></span>|<span data-ttu-id="61870-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61870-177">DateTimeOffset</span></span>|<span data-ttu-id="61870-178">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="61870-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="61870-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="61870-179">azureADRegistered</span></span>|<span data-ttu-id="61870-180">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="61870-180">Boolean</span></span>|<span data-ttu-id="61870-181">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61870-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="61870-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="61870-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="61870-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="61870-183">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="61870-p106">Тип регистрации устройства. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="61870-p106">Enrollment type of the device. The possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="61870-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="61870-186">activationLockBypassCode</span></span>|<span data-ttu-id="61870-187">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-187">String</span></span>|<span data-ttu-id="61870-188">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="61870-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="61870-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="61870-189">emailAddress</span></span>|<span data-ttu-id="61870-190">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-190">String</span></span>|<span data-ttu-id="61870-191">Адреса электронной почты пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="61870-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="61870-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="61870-192">azureADDeviceId</span></span>|<span data-ttu-id="61870-193">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-193">String</span></span>|<span data-ttu-id="61870-194">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61870-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="61870-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61870-195">Read only.</span></span>|
|<span data-ttu-id="61870-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="61870-196">deviceRegistrationState</span></span>|[<span data-ttu-id="61870-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="61870-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="61870-p108">Состояние совмещения устройства. Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="61870-p108">Device registration state. The possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="61870-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="61870-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="61870-201">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-201">String</span></span>|<span data-ttu-id="61870-202">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="61870-202">Device category display name</span></span>|
|<span data-ttu-id="61870-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="61870-203">isSupervised</span></span>|<span data-ttu-id="61870-204">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="61870-204">Boolean</span></span>|<span data-ttu-id="61870-205">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="61870-205">Device supervised status</span></span>|
|<span data-ttu-id="61870-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="61870-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="61870-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61870-207">DateTimeOffset</span></span>|<span data-ttu-id="61870-208">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="61870-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="61870-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="61870-209">exchangeAccessState</span></span>|[<span data-ttu-id="61870-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="61870-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="61870-p109">Состояние доступа устройства в Exchange. Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="61870-p109">The Access State of the device in Exchange. The possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="61870-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="61870-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="61870-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="61870-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="61870-p110">Причина состояния доступа к устройству в Exchange. Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="61870-p110">The reason for the device's access state in Exchange. The possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="61870-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="61870-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="61870-218">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-218">String</span></span>|<span data-ttu-id="61870-219">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="61870-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="61870-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="61870-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="61870-221">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-221">String</span></span>|<span data-ttu-id="61870-222">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="61870-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="61870-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="61870-223">isEncrypted</span></span>|<span data-ttu-id="61870-224">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="61870-224">Boolean</span></span>|<span data-ttu-id="61870-225">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="61870-225">Device encryption status</span></span>|
|<span data-ttu-id="61870-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="61870-226">userPrincipalName</span></span>|<span data-ttu-id="61870-227">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-227">String</span></span>|<span data-ttu-id="61870-228">Имя участника-пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="61870-228">Device user principal name</span></span>|
|<span data-ttu-id="61870-229">модель</span><span class="sxs-lookup"><span data-stu-id="61870-229">model</span></span>|<span data-ttu-id="61870-230">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-230">String</span></span>|<span data-ttu-id="61870-231">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="61870-231">Model of the device</span></span>|
|<span data-ttu-id="61870-232">производитель</span><span class="sxs-lookup"><span data-stu-id="61870-232">manufacturer</span></span>|<span data-ttu-id="61870-233">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-233">String</span></span>|<span data-ttu-id="61870-234">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="61870-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="61870-235">imei</span><span class="sxs-lookup"><span data-stu-id="61870-235">imei</span></span>|<span data-ttu-id="61870-236">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-236">String</span></span>|<span data-ttu-id="61870-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="61870-237">IMEI</span></span>|
|<span data-ttu-id="61870-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="61870-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="61870-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61870-239">DateTimeOffset</span></span>|<span data-ttu-id="61870-240">Дата и время истечения льготного периода соответствия устройства требованиям</span><span class="sxs-lookup"><span data-stu-id="61870-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="61870-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="61870-241">serialNumber</span></span>|<span data-ttu-id="61870-242">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-242">String</span></span>|<span data-ttu-id="61870-243">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="61870-243">SerialNumber</span></span>|
|<span data-ttu-id="61870-244">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="61870-244">phoneNumber</span></span>|<span data-ttu-id="61870-245">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-245">String</span></span>|<span data-ttu-id="61870-246">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="61870-246">Phone number of the device</span></span>|
|<span data-ttu-id="61870-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="61870-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="61870-248">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-248">String</span></span>|<span data-ttu-id="61870-249">Уровень обновления для системы безопасности Android</span><span class="sxs-lookup"><span data-stu-id="61870-249">Android security patch level</span></span>|
|<span data-ttu-id="61870-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="61870-250">userDisplayName</span></span>|<span data-ttu-id="61870-251">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-251">String</span></span>|<span data-ttu-id="61870-252">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="61870-252">User display name</span></span>|
|<span data-ttu-id="61870-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="61870-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="61870-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="61870-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="61870-255">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="61870-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="61870-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="61870-256">wiFiMacAddress</span></span>|<span data-ttu-id="61870-257">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-257">String</span></span>|<span data-ttu-id="61870-258">MAC-адрес сети Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="61870-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="61870-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="61870-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="61870-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="61870-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="61870-261">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-261">The device health attestation state.</span></span>|
|<span data-ttu-id="61870-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="61870-262">subscriberCarrier</span></span>|<span data-ttu-id="61870-263">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-263">String</span></span>|<span data-ttu-id="61870-264">Оператор сотовой связи, используемый абонентом</span><span class="sxs-lookup"><span data-stu-id="61870-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="61870-265">meid</span><span class="sxs-lookup"><span data-stu-id="61870-265">meid</span></span>|<span data-ttu-id="61870-266">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-266">String</span></span>|<span data-ttu-id="61870-267">MEID</span><span class="sxs-lookup"><span data-stu-id="61870-267">MEID</span></span>|
|<span data-ttu-id="61870-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="61870-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="61870-269">Int64</span><span class="sxs-lookup"><span data-stu-id="61870-269">Int64</span></span>|<span data-ttu-id="61870-270">Общий объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="61870-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="61870-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="61870-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="61870-272">Int64</span><span class="sxs-lookup"><span data-stu-id="61870-272">Int64</span></span>|<span data-ttu-id="61870-273">Свободный объем хранилища в байтах</span><span class="sxs-lookup"><span data-stu-id="61870-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="61870-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="61870-274">managedDeviceName</span></span>|<span data-ttu-id="61870-275">String (строка)</span><span class="sxs-lookup"><span data-stu-id="61870-275">String</span></span>|<span data-ttu-id="61870-276">Автоматически созданный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="61870-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="61870-277">Может быть заменен понятным именем.</span><span class="sxs-lookup"><span data-stu-id="61870-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="61870-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="61870-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="61870-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="61870-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="61870-p112">Указывает состояние угроз для устройства, когда учетная запись и устройство использует партнер мобильной защиты от угроз. Только для чтения. Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="61870-p112">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span>|



## <a name="response"></a><span data-ttu-id="61870-283">Ответ</span><span class="sxs-lookup"><span data-stu-id="61870-283">Response</span></span>
<span data-ttu-id="61870-284">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDevice](../resources/intune_devices_manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61870-284">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61870-285">Пример</span><span class="sxs-lookup"><span data-stu-id="61870-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="61870-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="61870-286">Request</span></span>
<span data-ttu-id="61870-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61870-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4604

{
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

### <a name="response"></a><span data-ttu-id="61870-288">Ответ</span><span class="sxs-lookup"><span data-stu-id="61870-288">Response</span></span>
<span data-ttu-id="61870-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61870-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








