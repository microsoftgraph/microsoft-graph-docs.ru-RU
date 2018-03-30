# <a name="create-manageddevice"></a><span data-ttu-id="bb175-101">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="bb175-101">Create managedDevice</span></span>

> <span data-ttu-id="bb175-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb175-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb175-103">Создание объекта [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="bb175-103">Create a new [plannerBucket](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb175-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bb175-104">Prerequisites</span></span>
<span data-ttu-id="bb175-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb175-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb175-107">Permission type</span></span>|<span data-ttu-id="bb175-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb175-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb175-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb175-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bb175-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb175-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb175-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb175-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb175-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb175-112">Not supported.</span></span>|
|<span data-ttu-id="bb175-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb175-113">Application</span></span>|<span data-ttu-id="bb175-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb175-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb175-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb175-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="bb175-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb175-116">Request headers</span></span>
|<span data-ttu-id="bb175-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb175-117">Header</span></span>|<span data-ttu-id="bb175-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bb175-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb175-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb175-119">Authorization</span></span>|<span data-ttu-id="bb175-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb175-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bb175-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bb175-121">Accept</span></span>|<span data-ttu-id="bb175-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bb175-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb175-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb175-123">Request body</span></span>
<span data-ttu-id="bb175-124">В тексте запроса добавьте представление объекта managedDevice в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb175-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="bb175-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedDevice.</span><span class="sxs-lookup"><span data-stu-id="bb175-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="bb175-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb175-126">Property</span></span>|<span data-ttu-id="bb175-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bb175-127">Type</span></span>|<span data-ttu-id="bb175-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bb175-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb175-129">id</span><span class="sxs-lookup"><span data-stu-id="bb175-129">id</span></span>|<span data-ttu-id="bb175-130">String</span><span class="sxs-lookup"><span data-stu-id="bb175-130">String</span></span>|<span data-ttu-id="bb175-131">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="bb175-132">userId</span><span class="sxs-lookup"><span data-stu-id="bb175-132">userID</span></span>|<span data-ttu-id="bb175-133">String</span><span class="sxs-lookup"><span data-stu-id="bb175-133">String</span></span>|<span data-ttu-id="bb175-134">Уникальный идентификатор пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="bb175-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="bb175-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="bb175-135">deviceName</span></span>|<span data-ttu-id="bb175-136">String</span><span class="sxs-lookup"><span data-stu-id="bb175-136">String</span></span>|<span data-ttu-id="bb175-137">Название устройства</span><span class="sxs-lookup"><span data-stu-id="bb175-137">Name of the device</span></span>|
|<span data-ttu-id="bb175-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="bb175-138">deviceActionResults</span></span>|<span data-ttu-id="bb175-139">Коллекция [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bb175-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="bb175-140">Список объектов deviceActionResult сложного типа.</span><span class="sxs-lookup"><span data-stu-id="bb175-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="bb175-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="bb175-141">enrolledDateTime</span></span>|<span data-ttu-id="bb175-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb175-142">DateTimeOffset</span></span>|<span data-ttu-id="bb175-143">Время регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="bb175-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bb175-144">lastSyncDateTime</span></span>|<span data-ttu-id="bb175-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb175-145">DateTimeOffset</span></span>|<span data-ttu-id="bb175-146">Дата и время последней успешной синхронизации устройства с Intune.</span><span class="sxs-lookup"><span data-stu-id="bb175-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="bb175-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb175-147">operatingSystem</span></span>|<span data-ttu-id="bb175-148">String</span><span class="sxs-lookup"><span data-stu-id="bb175-148">String</span></span>|<span data-ttu-id="bb175-149">Операционная система устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-149">Operating system of the device.</span></span> <span data-ttu-id="bb175-150">Windows, iOS и т. д.</span><span class="sxs-lookup"><span data-stu-id="bb175-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="bb175-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="bb175-151">complianceState</span></span>|<span data-ttu-id="bb175-152">String</span><span class="sxs-lookup"><span data-stu-id="bb175-152">String</span></span>|<span data-ttu-id="bb175-153">Состояние соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb175-153">Compliance state of the device.</span></span> <span data-ttu-id="bb175-154">Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="bb175-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="bb175-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="bb175-155">jailBroken</span></span>|<span data-ttu-id="bb175-156">String</span><span class="sxs-lookup"><span data-stu-id="bb175-156">String</span></span>|<span data-ttu-id="bb175-157">Указывает, является ли устройство взломанным или рутованным.</span><span class="sxs-lookup"><span data-stu-id="bb175-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="bb175-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="bb175-158">managementAgent</span></span>|<span data-ttu-id="bb175-159">String</span><span class="sxs-lookup"><span data-stu-id="bb175-159">String</span></span>|<span data-ttu-id="bb175-160">Канал управления устройством.</span><span class="sxs-lookup"><span data-stu-id="bb175-160">Management channel of the device.</span></span> <span data-ttu-id="bb175-161">Intune, EAS и т. д. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="bb175-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="bb175-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="bb175-162">osVersion</span></span>|<span data-ttu-id="bb175-163">String</span><span class="sxs-lookup"><span data-stu-id="bb175-163">String</span></span>|<span data-ttu-id="bb175-164">Версия операционной системы устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="bb175-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="bb175-165">easActivated</span></span>|<span data-ttu-id="bb175-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb175-166">Boolean</span></span>|<span data-ttu-id="bb175-167">Указывает, активировано ли устройство в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="bb175-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="bb175-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="bb175-168">easDeviceId</span></span>|<span data-ttu-id="bb175-169">String</span><span class="sxs-lookup"><span data-stu-id="bb175-169">String</span></span>|<span data-ttu-id="bb175-170">Идентификатор устройства в Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="bb175-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="bb175-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb175-171">easActivationDateTime</span></span>|<span data-ttu-id="bb175-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb175-172">DateTimeOffset</span></span>|<span data-ttu-id="bb175-173">Время активации устройства в Exchange ActivationSync.</span><span class="sxs-lookup"><span data-stu-id="bb175-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="bb175-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="bb175-174">azureADRegistered</span></span>|<span data-ttu-id="bb175-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb175-175">Boolean</span></span>|<span data-ttu-id="bb175-176">Указывает, зарегистрировано ли устройство в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb175-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="bb175-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb175-177">deviceEnrollmentType</span></span>|<span data-ttu-id="bb175-178">String</span><span class="sxs-lookup"><span data-stu-id="bb175-178">String</span></span>|<span data-ttu-id="bb175-179">Тип регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-179">Enrollment type of the device.</span></span> <span data-ttu-id="bb175-180">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="bb175-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="bb175-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="bb175-181">activationLockBypassCode</span></span>|<span data-ttu-id="bb175-182">String</span><span class="sxs-lookup"><span data-stu-id="bb175-182">String</span></span>|<span data-ttu-id="bb175-183">Код, позволяющий обойти блокировку активации на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb175-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="bb175-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb175-184">emailAddress</span></span>|<span data-ttu-id="bb175-185">String</span><span class="sxs-lookup"><span data-stu-id="bb175-185">String</span></span>|<span data-ttu-id="bb175-186">Электронные адреса пользователя, связанного с устройством</span><span class="sxs-lookup"><span data-stu-id="bb175-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="bb175-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="bb175-187">azureADDeviceId</span></span>|<span data-ttu-id="bb175-188">String</span><span class="sxs-lookup"><span data-stu-id="bb175-188">String</span></span>|<span data-ttu-id="bb175-189">Уникальный идентификатор устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb175-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="bb175-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb175-190">Read only.</span></span>|
|<span data-ttu-id="bb175-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bb175-191">deviceRegistrationState</span></span>|<span data-ttu-id="bb175-192">String</span><span class="sxs-lookup"><span data-stu-id="bb175-192">String</span></span>|<span data-ttu-id="bb175-193">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-193">Device registration state.</span></span> <span data-ttu-id="bb175-194">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bb175-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="bb175-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb175-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="bb175-196">String</span><span class="sxs-lookup"><span data-stu-id="bb175-196">String</span></span>|<span data-ttu-id="bb175-197">Отображаемое имя категории устройства</span><span class="sxs-lookup"><span data-stu-id="bb175-197">Device category display name</span></span>|
|<span data-ttu-id="bb175-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="bb175-198">isSupervised</span></span>|<span data-ttu-id="bb175-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb175-199">Boolean</span></span>|<span data-ttu-id="bb175-200">Состояние защиты устройства</span><span class="sxs-lookup"><span data-stu-id="bb175-200">Device supervised status</span></span>|
|<span data-ttu-id="bb175-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bb175-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="bb175-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb175-202">DateTimeOffset</span></span>|<span data-ttu-id="bb175-203">Время последнего подключения устройства к Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb175-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="bb175-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="bb175-204">exchangeAccessState</span></span>|<span data-ttu-id="bb175-205">String</span><span class="sxs-lookup"><span data-stu-id="bb175-205">String</span></span>|<span data-ttu-id="bb175-206">Состояние доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb175-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="bb175-207">Возможные значения: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="bb175-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="bb175-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="bb175-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="bb175-209">String</span><span class="sxs-lookup"><span data-stu-id="bb175-209">String</span></span>|<span data-ttu-id="bb175-210">Причина состояния доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb175-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="bb175-211">Возможные значения: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="bb175-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="bb175-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="bb175-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="bb175-213">String</span><span class="sxs-lookup"><span data-stu-id="bb175-213">String</span></span>|<span data-ttu-id="bb175-214">URL-адрес, позволяющий установить сеанс удаленного помощника с устройством.</span><span class="sxs-lookup"><span data-stu-id="bb175-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="bb175-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bb175-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="bb175-216">String</span><span class="sxs-lookup"><span data-stu-id="bb175-216">String</span></span>|<span data-ttu-id="bb175-217">Проблемы, возникающие при создании сеансов удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="bb175-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="bb175-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="bb175-218">isEncrypted</span></span>|<span data-ttu-id="bb175-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb175-219">Boolean</span></span>|<span data-ttu-id="bb175-220">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-220">Device encryption status</span></span>|
|<span data-ttu-id="bb175-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb175-221">userPrincipalName</span></span>|<span data-ttu-id="bb175-222">String</span><span class="sxs-lookup"><span data-stu-id="bb175-222">String</span></span>|<span data-ttu-id="bb175-223">Имя участника-пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-223">Device user principal name</span></span>|
|<span data-ttu-id="bb175-224">model</span><span class="sxs-lookup"><span data-stu-id="bb175-224">model</span></span>|<span data-ttu-id="bb175-225">String</span><span class="sxs-lookup"><span data-stu-id="bb175-225">String</span></span>|<span data-ttu-id="bb175-226">Модель устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-226">Model of the device</span></span>|
|<span data-ttu-id="bb175-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bb175-227">Camera manufacturer.</span></span>|<span data-ttu-id="bb175-228">String</span><span class="sxs-lookup"><span data-stu-id="bb175-228">String</span></span>|<span data-ttu-id="bb175-229">Производитель устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="bb175-230">imei</span><span class="sxs-lookup"><span data-stu-id="bb175-230">imei</span></span>|<span data-ttu-id="bb175-231">String</span><span class="sxs-lookup"><span data-stu-id="bb175-231">String</span></span>|<span data-ttu-id="bb175-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="bb175-232">IMEI</span></span>|
|<span data-ttu-id="bb175-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb175-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bb175-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb175-234">DateTimeOffset</span></span>|<span data-ttu-id="bb175-235">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb175-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bb175-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="bb175-236">serialNumber</span></span>|<span data-ttu-id="bb175-237">String</span><span class="sxs-lookup"><span data-stu-id="bb175-237">String</span></span>|<span data-ttu-id="bb175-238">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="bb175-238">SerialNumber Property</span></span>|
|<span data-ttu-id="bb175-239">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="bb175-239">PhoneNumber</span></span>|<span data-ttu-id="bb175-240">String</span><span class="sxs-lookup"><span data-stu-id="bb175-240">String</span></span>|<span data-ttu-id="bb175-241">Номер телефона устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-241">Phone number of the device</span></span>|
|<span data-ttu-id="bb175-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bb175-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="bb175-243">String</span><span class="sxs-lookup"><span data-stu-id="bb175-243">String</span></span>|<span data-ttu-id="bb175-244">Уровень исправления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="bb175-244">Android security patch level</span></span>|
|<span data-ttu-id="bb175-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb175-245">userDisplayName</span></span>|<span data-ttu-id="bb175-246">String</span><span class="sxs-lookup"><span data-stu-id="bb175-246">String</span></span>|<span data-ttu-id="bb175-247">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb175-247">user display name</span></span>|
|<span data-ttu-id="bb175-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bb175-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="bb175-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bb175-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="bb175-250">Включенные функции клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="bb175-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="bb175-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="bb175-251">wiFiMacAddress</span></span>|<span data-ttu-id="bb175-252">String</span><span class="sxs-lookup"><span data-stu-id="bb175-252">String</span></span>|<span data-ttu-id="bb175-253">MAC-адрес сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bb175-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="bb175-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bb175-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="bb175-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bb175-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="bb175-256">Состояние подтверждения работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-256">The device health attestation state.</span></span>|
|<span data-ttu-id="bb175-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="bb175-257">subscriberCarrier</span></span>|<span data-ttu-id="bb175-258">String</span><span class="sxs-lookup"><span data-stu-id="bb175-258">String</span></span>|<span data-ttu-id="bb175-259">Оператор сотовой связи, используемый абонентом.</span><span class="sxs-lookup"><span data-stu-id="bb175-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="bb175-260">meid</span><span class="sxs-lookup"><span data-stu-id="bb175-260">meid</span></span>|<span data-ttu-id="bb175-261">String</span><span class="sxs-lookup"><span data-stu-id="bb175-261">String</span></span>|<span data-ttu-id="bb175-262">MEID</span><span class="sxs-lookup"><span data-stu-id="bb175-262">MEID</span></span>|
|<span data-ttu-id="bb175-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bb175-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="bb175-264">Int64</span><span class="sxs-lookup"><span data-stu-id="bb175-264">Int64</span></span>|<span data-ttu-id="bb175-265">Общий объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="bb175-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="bb175-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bb175-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="bb175-267">Int64</span><span class="sxs-lookup"><span data-stu-id="bb175-267">Int64</span></span>|<span data-ttu-id="bb175-268">Свободный объем хранилища в байтах.</span><span class="sxs-lookup"><span data-stu-id="bb175-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="bb175-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="bb175-269">managedDeviceName</span></span>|<span data-ttu-id="bb175-270">String</span><span class="sxs-lookup"><span data-stu-id="bb175-270">String</span></span>|<span data-ttu-id="bb175-271">Автоматически созданное имя для идентификации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb175-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="bb175-272">Его можно заменить понятным именем.</span><span class="sxs-lookup"><span data-stu-id="bb175-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="bb175-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="bb175-273">partnerReportedThreatState</span></span>|<span data-ttu-id="bb175-274">String</span><span class="sxs-lookup"><span data-stu-id="bb175-274">String</span></span>|<span data-ttu-id="bb175-275">Указывает состояние угрозы со стороны устройства при использовании решения Mobile Threat Defense (в учетной записи и на устройстве).</span><span class="sxs-lookup"><span data-stu-id="bb175-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="bb175-276">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb175-276">Read only.</span></span> <span data-ttu-id="bb175-277">Возможные значения: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="bb175-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="bb175-278">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb175-278">Response</span></span>
<span data-ttu-id="bb175-279">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedDevice](../resources/intune_devices_manageddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb175-279">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb175-280">Пример</span><span class="sxs-lookup"><span data-stu-id="bb175-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb175-281">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb175-281">Request</span></span>
<span data-ttu-id="bb175-282">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb175-282">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4616

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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

### <a name="response"></a><span data-ttu-id="bb175-283">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb175-283">Response</span></span>
<span data-ttu-id="bb175-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb175-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4665

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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



