---
title: Создание comanagementEligibleDevice
description: Создание объекта comanagementEligibleDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e62e518f87472fde54dfb98cb0de25c68d39db0c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156030"
---
# <a name="create-comanagementeligibledevice"></a><span data-ttu-id="18965-103">Создание comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="18965-103">Create comanagementEligibleDevice</span></span>

<span data-ttu-id="18965-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18965-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18965-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18965-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18965-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18965-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18965-107">Создание объекта [comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)</span><span class="sxs-lookup"><span data-stu-id="18965-107">Create a new [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18965-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18965-108">Prerequisites</span></span>
<span data-ttu-id="18965-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18965-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18965-111">Permission type</span></span>|<span data-ttu-id="18965-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18965-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18965-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18965-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18965-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18965-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="18965-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18965-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18965-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18965-116">Not supported.</span></span>|
|<span data-ttu-id="18965-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18965-117">Application</span></span>|<span data-ttu-id="18965-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18965-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18965-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18965-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="18965-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18965-120">Request headers</span></span>
|<span data-ttu-id="18965-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18965-121">Header</span></span>|<span data-ttu-id="18965-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18965-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18965-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18965-123">Authorization</span></span>|<span data-ttu-id="18965-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18965-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18965-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18965-125">Accept</span></span>|<span data-ttu-id="18965-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18965-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18965-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18965-127">Request body</span></span>
<span data-ttu-id="18965-128">В теле запроса укажете представление объекта comanagementEligibleDevice в JSON.</span><span class="sxs-lookup"><span data-stu-id="18965-128">In the request body, supply a JSON representation for the comanagementEligibleDevice object.</span></span>

<span data-ttu-id="18965-129">В следующей таблице показаны свойства, необходимые при создании объекта comanagementEligibleDevice.</span><span class="sxs-lookup"><span data-stu-id="18965-129">The following table shows the properties that are required when you create the comanagementEligibleDevice.</span></span>

|<span data-ttu-id="18965-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18965-130">Property</span></span>|<span data-ttu-id="18965-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18965-131">Type</span></span>|<span data-ttu-id="18965-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18965-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18965-133">id</span><span class="sxs-lookup"><span data-stu-id="18965-133">id</span></span>|<span data-ttu-id="18965-134">String</span><span class="sxs-lookup"><span data-stu-id="18965-134">String</span></span>|<span data-ttu-id="18965-135">Уникальный ИД устройства</span><span class="sxs-lookup"><span data-stu-id="18965-135">Unique Id for the device</span></span>|
|<span data-ttu-id="18965-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="18965-136">deviceName</span></span>|<span data-ttu-id="18965-137">String</span><span class="sxs-lookup"><span data-stu-id="18965-137">String</span></span>|<span data-ttu-id="18965-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="18965-138">DeviceName</span></span>|
|<span data-ttu-id="18965-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="18965-139">deviceType</span></span>|[<span data-ttu-id="18965-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="18965-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="18965-141">DeviceType.</span><span class="sxs-lookup"><span data-stu-id="18965-141">DeviceType.</span></span> <span data-ttu-id="18965-142">Возможные значения: `desktop` , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` , , `winEmbedded` , `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .</span><span class="sxs-lookup"><span data-stu-id="18965-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="18965-143">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="18965-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="18965-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="18965-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="18965-145">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="18965-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="18965-146">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="18965-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="18965-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="18965-147">ownerType</span></span>|[<span data-ttu-id="18965-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="18965-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="18965-149">OwnerType.</span><span class="sxs-lookup"><span data-stu-id="18965-149">OwnerType.</span></span> <span data-ttu-id="18965-150">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="18965-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="18965-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="18965-151">managementAgents</span></span>|[<span data-ttu-id="18965-152">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="18965-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="18965-153">ManagementAgents.</span><span class="sxs-lookup"><span data-stu-id="18965-153">ManagementAgents.</span></span> <span data-ttu-id="18965-154">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="18965-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="18965-155">managementState</span><span class="sxs-lookup"><span data-stu-id="18965-155">managementState</span></span>|[<span data-ttu-id="18965-156">managementState</span><span class="sxs-lookup"><span data-stu-id="18965-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="18965-157">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="18965-157">ManagementState.</span></span> <span data-ttu-id="18965-158">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="18965-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="18965-159">referenceId</span><span class="sxs-lookup"><span data-stu-id="18965-159">referenceId</span></span>|<span data-ttu-id="18965-160">String</span><span class="sxs-lookup"><span data-stu-id="18965-160">String</span></span>|<span data-ttu-id="18965-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="18965-161">ReferenceId</span></span>|
|<span data-ttu-id="18965-162">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="18965-162">mdmStatus</span></span>|<span data-ttu-id="18965-163">String</span><span class="sxs-lookup"><span data-stu-id="18965-163">String</span></span>|<span data-ttu-id="18965-164">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="18965-164">MDMStatus</span></span>|
|<span data-ttu-id="18965-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="18965-165">osVersion</span></span>|<span data-ttu-id="18965-166">String</span><span class="sxs-lookup"><span data-stu-id="18965-166">String</span></span>|<span data-ttu-id="18965-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="18965-167">OSVersion</span></span>|
|<span data-ttu-id="18965-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="18965-168">serialNumber</span></span>|<span data-ttu-id="18965-169">String</span><span class="sxs-lookup"><span data-stu-id="18965-169">String</span></span>|<span data-ttu-id="18965-170">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="18965-170">SerialNumber</span></span>|
|<span data-ttu-id="18965-171">manufacturer</span><span class="sxs-lookup"><span data-stu-id="18965-171">manufacturer</span></span>|<span data-ttu-id="18965-172">String</span><span class="sxs-lookup"><span data-stu-id="18965-172">String</span></span>|<span data-ttu-id="18965-173">Изготовитель</span><span class="sxs-lookup"><span data-stu-id="18965-173">Manufacturer</span></span>|
|<span data-ttu-id="18965-174">model</span><span class="sxs-lookup"><span data-stu-id="18965-174">model</span></span>|<span data-ttu-id="18965-175">String</span><span class="sxs-lookup"><span data-stu-id="18965-175">String</span></span>|<span data-ttu-id="18965-176">Модель</span><span class="sxs-lookup"><span data-stu-id="18965-176">Model</span></span>|
|<span data-ttu-id="18965-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="18965-177">osDescription</span></span>|<span data-ttu-id="18965-178">String</span><span class="sxs-lookup"><span data-stu-id="18965-178">String</span></span>|<span data-ttu-id="18965-179">OSDescription</span><span class="sxs-lookup"><span data-stu-id="18965-179">OSDescription</span></span>|
|<span data-ttu-id="18965-180">entitySource</span><span class="sxs-lookup"><span data-stu-id="18965-180">entitySource</span></span>|<span data-ttu-id="18965-181">Int32</span><span class="sxs-lookup"><span data-stu-id="18965-181">Int32</span></span>|<span data-ttu-id="18965-182">EntitySource</span><span class="sxs-lookup"><span data-stu-id="18965-182">EntitySource</span></span>|
|<span data-ttu-id="18965-183">userId</span><span class="sxs-lookup"><span data-stu-id="18965-183">userId</span></span>|<span data-ttu-id="18965-184">String</span><span class="sxs-lookup"><span data-stu-id="18965-184">String</span></span>|<span data-ttu-id="18965-185">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="18965-185">UserId</span></span>|
|<span data-ttu-id="18965-186">upn</span><span class="sxs-lookup"><span data-stu-id="18965-186">upn</span></span>|<span data-ttu-id="18965-187">String</span><span class="sxs-lookup"><span data-stu-id="18965-187">String</span></span>|<span data-ttu-id="18965-188">UPN</span><span class="sxs-lookup"><span data-stu-id="18965-188">UPN</span></span>|
|<span data-ttu-id="18965-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="18965-189">userEmail</span></span>|<span data-ttu-id="18965-190">String</span><span class="sxs-lookup"><span data-stu-id="18965-190">String</span></span>|<span data-ttu-id="18965-191">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="18965-191">UserEmail</span></span>|
|<span data-ttu-id="18965-192">userName</span><span class="sxs-lookup"><span data-stu-id="18965-192">userName</span></span>|<span data-ttu-id="18965-193">String</span><span class="sxs-lookup"><span data-stu-id="18965-193">String</span></span>|<span data-ttu-id="18965-194">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="18965-194">UserName</span></span>|
|<span data-ttu-id="18965-195">status</span><span class="sxs-lookup"><span data-stu-id="18965-195">status</span></span>|[<span data-ttu-id="18965-196">comanagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="18965-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="18965-197">ComanagementEligibleStatus.</span><span class="sxs-lookup"><span data-stu-id="18965-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="18965-198">Возможные значения: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span><span class="sxs-lookup"><span data-stu-id="18965-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="18965-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="18965-199">Response</span></span>
<span data-ttu-id="18965-200">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18965-200">If successful, this method returns a `201 Created` response code and a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18965-201">Пример</span><span class="sxs-lookup"><span data-stu-id="18965-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="18965-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="18965-202">Request</span></span>
<span data-ttu-id="18965-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18965-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
Content-type: application/json
Content-length: 714

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```

### <a name="response"></a><span data-ttu-id="18965-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="18965-204">Response</span></span>
<span data-ttu-id="18965-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18965-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
  "deviceName": "Device Name value",
  "deviceType": "windowsRT",
  "clientRegistrationStatus": "registered",
  "ownerType": "company",
  "managementAgents": "mdm",
  "managementState": "retirePending",
  "referenceId": "Reference Id value",
  "mdmStatus": "Mdm Status value",
  "osVersion": "Os Version value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "osDescription": "Os Description value",
  "entitySource": 12,
  "userId": "User Id value",
  "upn": "Upn value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "status": "eligible"
}
```




