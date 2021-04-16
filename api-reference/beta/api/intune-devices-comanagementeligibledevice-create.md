---
title: Создание comanagementEligibleDevice
description: Создайте новый объект comanagementEligibleDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cd89881d3d76e0f64f2b33f5008f5b2b66e1043
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863494"
---
# <a name="create-comanagementeligibledevice"></a><span data-ttu-id="bf24c-103">Создание comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="bf24c-103">Create comanagementEligibleDevice</span></span>

<span data-ttu-id="bf24c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf24c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf24c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf24c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf24c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf24c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf24c-107">Создайте новый [объект comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)</span><span class="sxs-lookup"><span data-stu-id="bf24c-107">Create a new [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf24c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf24c-108">Prerequisites</span></span>
<span data-ttu-id="bf24c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf24c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf24c-111">Permission type</span></span>|<span data-ttu-id="bf24c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf24c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf24c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf24c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf24c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf24c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bf24c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf24c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf24c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf24c-116">Not supported.</span></span>|
|<span data-ttu-id="bf24c-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="bf24c-117">Application</span></span>|<span data-ttu-id="bf24c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf24c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf24c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf24c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="bf24c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf24c-120">Request headers</span></span>
|<span data-ttu-id="bf24c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf24c-121">Header</span></span>|<span data-ttu-id="bf24c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf24c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf24c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf24c-123">Authorization</span></span>|<span data-ttu-id="bf24c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf24c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf24c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf24c-125">Accept</span></span>|<span data-ttu-id="bf24c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf24c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf24c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf24c-127">Request body</span></span>
<span data-ttu-id="bf24c-128">В теле запроса поставляем представление JSON для объекта comanagementEligibleDevice.</span><span class="sxs-lookup"><span data-stu-id="bf24c-128">In the request body, supply a JSON representation for the comanagementEligibleDevice object.</span></span>

<span data-ttu-id="bf24c-129">В следующей таблице показаны свойства, необходимые при создании comanagementEligibleDevice.</span><span class="sxs-lookup"><span data-stu-id="bf24c-129">The following table shows the properties that are required when you create the comanagementEligibleDevice.</span></span>

|<span data-ttu-id="bf24c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf24c-130">Property</span></span>|<span data-ttu-id="bf24c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf24c-131">Type</span></span>|<span data-ttu-id="bf24c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf24c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf24c-133">id</span><span class="sxs-lookup"><span data-stu-id="bf24c-133">id</span></span>|<span data-ttu-id="bf24c-134">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-134">String</span></span>|<span data-ttu-id="bf24c-135">Уникальный ID для устройства</span><span class="sxs-lookup"><span data-stu-id="bf24c-135">Unique Id for the device</span></span>|
|<span data-ttu-id="bf24c-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="bf24c-136">deviceName</span></span>|<span data-ttu-id="bf24c-137">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-137">String</span></span>|<span data-ttu-id="bf24c-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="bf24c-138">DeviceName</span></span>|
|<span data-ttu-id="bf24c-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="bf24c-139">deviceType</span></span>|[<span data-ttu-id="bf24c-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="bf24c-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="bf24c-141">DeviceType.</span><span class="sxs-lookup"><span data-stu-id="bf24c-141">DeviceType.</span></span> <span data-ttu-id="bf24c-142">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` . `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="bf24c-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="bf24c-143">clientRegistrationStatus</span><span class="sxs-lookup"><span data-stu-id="bf24c-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="bf24c-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bf24c-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="bf24c-145">ClientRegistrationStatus.</span><span class="sxs-lookup"><span data-stu-id="bf24c-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="bf24c-146">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bf24c-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="bf24c-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="bf24c-147">ownerType</span></span>|[<span data-ttu-id="bf24c-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="bf24c-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="bf24c-149">OwnerType.</span><span class="sxs-lookup"><span data-stu-id="bf24c-149">OwnerType.</span></span> <span data-ttu-id="bf24c-150">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="bf24c-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="bf24c-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="bf24c-151">managementAgents</span></span>|[<span data-ttu-id="bf24c-152">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="bf24c-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="bf24c-153">ManagementAgents.</span><span class="sxs-lookup"><span data-stu-id="bf24c-153">ManagementAgents.</span></span> <span data-ttu-id="bf24c-154">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`.</span><span class="sxs-lookup"><span data-stu-id="bf24c-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`.</span></span>|
|<span data-ttu-id="bf24c-155">managementState</span><span class="sxs-lookup"><span data-stu-id="bf24c-155">managementState</span></span>|[<span data-ttu-id="bf24c-156">managementState</span><span class="sxs-lookup"><span data-stu-id="bf24c-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="bf24c-157">ManagementState.</span><span class="sxs-lookup"><span data-stu-id="bf24c-157">ManagementState.</span></span> <span data-ttu-id="bf24c-158">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="bf24c-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="bf24c-159">referenceId</span><span class="sxs-lookup"><span data-stu-id="bf24c-159">referenceId</span></span>|<span data-ttu-id="bf24c-160">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-160">String</span></span>|<span data-ttu-id="bf24c-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="bf24c-161">ReferenceId</span></span>|
|<span data-ttu-id="bf24c-162">mdmStatus</span><span class="sxs-lookup"><span data-stu-id="bf24c-162">mdmStatus</span></span>|<span data-ttu-id="bf24c-163">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-163">String</span></span>|<span data-ttu-id="bf24c-164">MDMStatus</span><span class="sxs-lookup"><span data-stu-id="bf24c-164">MDMStatus</span></span>|
|<span data-ttu-id="bf24c-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="bf24c-165">osVersion</span></span>|<span data-ttu-id="bf24c-166">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-166">String</span></span>|<span data-ttu-id="bf24c-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="bf24c-167">OSVersion</span></span>|
|<span data-ttu-id="bf24c-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="bf24c-168">serialNumber</span></span>|<span data-ttu-id="bf24c-169">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-169">String</span></span>|<span data-ttu-id="bf24c-170">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="bf24c-170">SerialNumber</span></span>|
|<span data-ttu-id="bf24c-171">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bf24c-171">manufacturer</span></span>|<span data-ttu-id="bf24c-172">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-172">String</span></span>|<span data-ttu-id="bf24c-173">Производитель</span><span class="sxs-lookup"><span data-stu-id="bf24c-173">Manufacturer</span></span>|
|<span data-ttu-id="bf24c-174">model</span><span class="sxs-lookup"><span data-stu-id="bf24c-174">model</span></span>|<span data-ttu-id="bf24c-175">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-175">String</span></span>|<span data-ttu-id="bf24c-176">Модель</span><span class="sxs-lookup"><span data-stu-id="bf24c-176">Model</span></span>|
|<span data-ttu-id="bf24c-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="bf24c-177">osDescription</span></span>|<span data-ttu-id="bf24c-178">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-178">String</span></span>|<span data-ttu-id="bf24c-179">OSDescription</span><span class="sxs-lookup"><span data-stu-id="bf24c-179">OSDescription</span></span>|
|<span data-ttu-id="bf24c-180">entitySource</span><span class="sxs-lookup"><span data-stu-id="bf24c-180">entitySource</span></span>|<span data-ttu-id="bf24c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="bf24c-181">Int32</span></span>|<span data-ttu-id="bf24c-182">EntitySource</span><span class="sxs-lookup"><span data-stu-id="bf24c-182">EntitySource</span></span>|
|<span data-ttu-id="bf24c-183">userId</span><span class="sxs-lookup"><span data-stu-id="bf24c-183">userId</span></span>|<span data-ttu-id="bf24c-184">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-184">String</span></span>|<span data-ttu-id="bf24c-185">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="bf24c-185">UserId</span></span>|
|<span data-ttu-id="bf24c-186">upn</span><span class="sxs-lookup"><span data-stu-id="bf24c-186">upn</span></span>|<span data-ttu-id="bf24c-187">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-187">String</span></span>|<span data-ttu-id="bf24c-188">Имя участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="bf24c-188">UPN</span></span>|
|<span data-ttu-id="bf24c-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="bf24c-189">userEmail</span></span>|<span data-ttu-id="bf24c-190">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-190">String</span></span>|<span data-ttu-id="bf24c-191">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="bf24c-191">UserEmail</span></span>|
|<span data-ttu-id="bf24c-192">userName</span><span class="sxs-lookup"><span data-stu-id="bf24c-192">userName</span></span>|<span data-ttu-id="bf24c-193">String</span><span class="sxs-lookup"><span data-stu-id="bf24c-193">String</span></span>|<span data-ttu-id="bf24c-194">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="bf24c-194">UserName</span></span>|
|<span data-ttu-id="bf24c-195">status</span><span class="sxs-lookup"><span data-stu-id="bf24c-195">status</span></span>|[<span data-ttu-id="bf24c-196">comanagementEligibleType</span><span class="sxs-lookup"><span data-stu-id="bf24c-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="bf24c-197">ComanagementEligibleStatus.</span><span class="sxs-lookup"><span data-stu-id="bf24c-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="bf24c-198">Возможные значения: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span><span class="sxs-lookup"><span data-stu-id="bf24c-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="bf24c-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf24c-199">Response</span></span>
<span data-ttu-id="bf24c-200">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bf24c-200">If successful, this method returns a `201 Created` response code and a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf24c-201">Пример</span><span class="sxs-lookup"><span data-stu-id="bf24c-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf24c-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf24c-202">Request</span></span>
<span data-ttu-id="bf24c-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf24c-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bf24c-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf24c-204">Response</span></span>
<span data-ttu-id="bf24c-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf24c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




