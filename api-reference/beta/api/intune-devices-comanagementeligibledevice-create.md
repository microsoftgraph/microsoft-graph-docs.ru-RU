---
title: Создание Команажементелигибледевице
description: Создание нового объекта Команажементелигибледевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98a57bdd62f292ba118d09c0c3c31f8d43626f99
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792550"
---
# <a name="create-comanagementeligibledevice"></a><span data-ttu-id="c1ffe-103">Создание Команажементелигибледевице</span><span class="sxs-lookup"><span data-stu-id="c1ffe-103">Create comanagementEligibleDevice</span></span>

<span data-ttu-id="c1ffe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1ffe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1ffe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1ffe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ffe-107">Создание нового объекта [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .</span><span class="sxs-lookup"><span data-stu-id="c1ffe-107">Create a new [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ffe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1ffe-108">Prerequisites</span></span>
<span data-ttu-id="c1ffe-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1ffe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ffe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ffe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1ffe-111">Permission type</span></span>|<span data-ttu-id="c1ffe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1ffe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ffe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1ffe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ffe-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ffe-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c1ffe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1ffe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ffe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-116">Not supported.</span></span>|
|<span data-ttu-id="c1ffe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1ffe-117">Application</span></span>|<span data-ttu-id="c1ffe-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ffe-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ffe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1ffe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="c1ffe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1ffe-120">Request headers</span></span>
|<span data-ttu-id="c1ffe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1ffe-121">Header</span></span>|<span data-ttu-id="c1ffe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1ffe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ffe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1ffe-123">Authorization</span></span>|<span data-ttu-id="c1ffe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ffe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1ffe-125">Accept</span></span>|<span data-ttu-id="c1ffe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ffe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ffe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1ffe-127">Request body</span></span>
<span data-ttu-id="c1ffe-128">В тексте запроса добавьте представление объекта Команажементелигибледевице в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-128">In the request body, supply a JSON representation for the comanagementEligibleDevice object.</span></span>

<span data-ttu-id="c1ffe-129">В следующей таблице приведены свойства, необходимые при создании Команажементелигибледевице.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-129">The following table shows the properties that are required when you create the comanagementEligibleDevice.</span></span>

|<span data-ttu-id="c1ffe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1ffe-130">Property</span></span>|<span data-ttu-id="c1ffe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1ffe-131">Type</span></span>|<span data-ttu-id="c1ffe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1ffe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ffe-133">id</span><span class="sxs-lookup"><span data-stu-id="c1ffe-133">id</span></span>|<span data-ttu-id="c1ffe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c1ffe-134">String</span></span>|<span data-ttu-id="c1ffe-135">Уникальный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="c1ffe-135">Unique Id for the device</span></span>|
|<span data-ttu-id="c1ffe-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c1ffe-136">deviceName</span></span>|<span data-ttu-id="c1ffe-137">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-137">String</span></span>|<span data-ttu-id="c1ffe-138">DeviceName</span><span class="sxs-lookup"><span data-stu-id="c1ffe-138">DeviceName</span></span>|
|<span data-ttu-id="c1ffe-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="c1ffe-139">deviceType</span></span>|[<span data-ttu-id="c1ffe-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="c1ffe-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c1ffe-141">DeviceType.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-141">DeviceType.</span></span> <span data-ttu-id="c1ffe-142">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c1ffe-143">клиентрегистратионстатус</span><span class="sxs-lookup"><span data-stu-id="c1ffe-143">clientRegistrationStatus</span></span>|[<span data-ttu-id="c1ffe-144">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c1ffe-144">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="c1ffe-145">Клиентрегистратионстатус.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-145">ClientRegistrationStatus.</span></span> <span data-ttu-id="c1ffe-146">Возможные значения: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-146">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="c1ffe-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="c1ffe-147">ownerType</span></span>|[<span data-ttu-id="c1ffe-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="c1ffe-148">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="c1ffe-149">OwnerType.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-149">OwnerType.</span></span> <span data-ttu-id="c1ffe-150">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c1ffe-151">managementAgents</span><span class="sxs-lookup"><span data-stu-id="c1ffe-151">managementAgents</span></span>|[<span data-ttu-id="c1ffe-152">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="c1ffe-152">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="c1ffe-153">ManagementAgents.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-153">ManagementAgents.</span></span> <span data-ttu-id="c1ffe-154">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-154">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="c1ffe-155">манажементстате</span><span class="sxs-lookup"><span data-stu-id="c1ffe-155">managementState</span></span>|[<span data-ttu-id="c1ffe-156">манажементстате</span><span class="sxs-lookup"><span data-stu-id="c1ffe-156">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="c1ffe-157">Манажементстате.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-157">ManagementState.</span></span> <span data-ttu-id="c1ffe-158">Возможные значения: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-158">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="c1ffe-159">референцеид</span><span class="sxs-lookup"><span data-stu-id="c1ffe-159">referenceId</span></span>|<span data-ttu-id="c1ffe-160">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-160">String</span></span>|<span data-ttu-id="c1ffe-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="c1ffe-161">ReferenceId</span></span>|
|<span data-ttu-id="c1ffe-162">мдмстатус</span><span class="sxs-lookup"><span data-stu-id="c1ffe-162">mdmStatus</span></span>|<span data-ttu-id="c1ffe-163">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-163">String</span></span>|<span data-ttu-id="c1ffe-164">мдмстатус</span><span class="sxs-lookup"><span data-stu-id="c1ffe-164">MDMStatus</span></span>|
|<span data-ttu-id="c1ffe-165">osVersion</span><span class="sxs-lookup"><span data-stu-id="c1ffe-165">osVersion</span></span>|<span data-ttu-id="c1ffe-166">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-166">String</span></span>|<span data-ttu-id="c1ffe-167">OSVersion</span><span class="sxs-lookup"><span data-stu-id="c1ffe-167">OSVersion</span></span>|
|<span data-ttu-id="c1ffe-168">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c1ffe-168">serialNumber</span></span>|<span data-ttu-id="c1ffe-169">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-169">String</span></span>|<span data-ttu-id="c1ffe-170">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="c1ffe-170">SerialNumber</span></span>|
|<span data-ttu-id="c1ffe-171">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c1ffe-171">manufacturer</span></span>|<span data-ttu-id="c1ffe-172">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-172">String</span></span>|<span data-ttu-id="c1ffe-173">Вычислитель</span><span class="sxs-lookup"><span data-stu-id="c1ffe-173">Manufacturer</span></span>|
|<span data-ttu-id="c1ffe-174">model</span><span class="sxs-lookup"><span data-stu-id="c1ffe-174">model</span></span>|<span data-ttu-id="c1ffe-175">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-175">String</span></span>|<span data-ttu-id="c1ffe-176">Модель</span><span class="sxs-lookup"><span data-stu-id="c1ffe-176">Model</span></span>|
|<span data-ttu-id="c1ffe-177">osDescription</span><span class="sxs-lookup"><span data-stu-id="c1ffe-177">osDescription</span></span>|<span data-ttu-id="c1ffe-178">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-178">String</span></span>|<span data-ttu-id="c1ffe-179">Свойства OSDescription</span><span class="sxs-lookup"><span data-stu-id="c1ffe-179">OSDescription</span></span>|
|<span data-ttu-id="c1ffe-180">ентитисаурце</span><span class="sxs-lookup"><span data-stu-id="c1ffe-180">entitySource</span></span>|<span data-ttu-id="c1ffe-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c1ffe-181">Int32</span></span>|<span data-ttu-id="c1ffe-182">ентитисаурце</span><span class="sxs-lookup"><span data-stu-id="c1ffe-182">EntitySource</span></span>|
|<span data-ttu-id="c1ffe-183">userId</span><span class="sxs-lookup"><span data-stu-id="c1ffe-183">userId</span></span>|<span data-ttu-id="c1ffe-184">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-184">String</span></span>|<span data-ttu-id="c1ffe-185">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="c1ffe-185">UserId</span></span>|
|<span data-ttu-id="c1ffe-186">Основное</span><span class="sxs-lookup"><span data-stu-id="c1ffe-186">upn</span></span>|<span data-ttu-id="c1ffe-187">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-187">String</span></span>|<span data-ttu-id="c1ffe-188">Имя участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="c1ffe-188">UPN</span></span>|
|<span data-ttu-id="c1ffe-189">userEmail</span><span class="sxs-lookup"><span data-stu-id="c1ffe-189">userEmail</span></span>|<span data-ttu-id="c1ffe-190">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-190">String</span></span>|<span data-ttu-id="c1ffe-191">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="c1ffe-191">UserEmail</span></span>|
|<span data-ttu-id="c1ffe-192">userName</span><span class="sxs-lookup"><span data-stu-id="c1ffe-192">userName</span></span>|<span data-ttu-id="c1ffe-193">String</span><span class="sxs-lookup"><span data-stu-id="c1ffe-193">String</span></span>|<span data-ttu-id="c1ffe-194">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="c1ffe-194">UserName</span></span>|
|<span data-ttu-id="c1ffe-195">status</span><span class="sxs-lookup"><span data-stu-id="c1ffe-195">status</span></span>|[<span data-ttu-id="c1ffe-196">команажементелигиблетипе</span><span class="sxs-lookup"><span data-stu-id="c1ffe-196">comanagementEligibleType</span></span>](../resources/intune-devices-comanagementeligibletype.md)|<span data-ttu-id="c1ffe-197">Команажементелигиблестатус.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-197">ComanagementEligibleStatus.</span></span> <span data-ttu-id="c1ffe-198">Возможные значения: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-198">Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1ffe-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ffe-199">Response</span></span>
<span data-ttu-id="c1ffe-200">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-200">If successful, this method returns a `201 Created` response code and a [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ffe-201">Пример</span><span class="sxs-lookup"><span data-stu-id="c1ffe-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ffe-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1ffe-202">Request</span></span>
<span data-ttu-id="c1ffe-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1ffe-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1ffe-204">Response</span></span>
<span data-ttu-id="c1ffe-205">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-205">Here is an example of the response.</span></span> <span data-ttu-id="c1ffe-206">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-206">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1ffe-207">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c1ffe-207">All of the properties will be returned from an actual call.</span></span>
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



