---
title: Создание Девицеманажементинтентдевицестате
description: Создание нового объекта Девицеманажементинтентдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5de043e10960e54b9f8ba15c28380af9b003406
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49289491"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="2fa68-103">Создание Девицеманажементинтентдевицестате</span><span class="sxs-lookup"><span data-stu-id="2fa68-103">Create deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="2fa68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fa68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fa68-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fa68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fa68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fa68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa68-107">Создание нового объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="2fa68-107">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fa68-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2fa68-108">Prerequisites</span></span>
<span data-ttu-id="2fa68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fa68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fa68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fa68-111">Permission type</span></span>|<span data-ttu-id="2fa68-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fa68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fa68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fa68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fa68-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fa68-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fa68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fa68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fa68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fa68-116">Not supported.</span></span>|
|<span data-ttu-id="2fa68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fa68-117">Application</span></span>|<span data-ttu-id="2fa68-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fa68-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fa68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fa68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="2fa68-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2fa68-120">Request headers</span></span>
|<span data-ttu-id="2fa68-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fa68-121">Header</span></span>|<span data-ttu-id="2fa68-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2fa68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fa68-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fa68-123">Authorization</span></span>|<span data-ttu-id="2fa68-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fa68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fa68-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fa68-125">Accept</span></span>|<span data-ttu-id="2fa68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fa68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fa68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fa68-127">Request body</span></span>
<span data-ttu-id="2fa68-128">В тексте запроса добавьте представление объекта Девицеманажементинтентдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fa68-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="2fa68-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентдевицестате.</span><span class="sxs-lookup"><span data-stu-id="2fa68-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="2fa68-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fa68-130">Property</span></span>|<span data-ttu-id="2fa68-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2fa68-131">Type</span></span>|<span data-ttu-id="2fa68-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa68-133">id</span><span class="sxs-lookup"><span data-stu-id="2fa68-133">id</span></span>|<span data-ttu-id="2fa68-134">String</span><span class="sxs-lookup"><span data-stu-id="2fa68-134">String</span></span>|<span data-ttu-id="2fa68-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2fa68-135">The ID</span></span>|
|<span data-ttu-id="2fa68-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2fa68-136">userPrincipalName</span></span>|<span data-ttu-id="2fa68-137">String</span><span class="sxs-lookup"><span data-stu-id="2fa68-137">String</span></span>|<span data-ttu-id="2fa68-138">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="2fa68-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="2fa68-139">userName</span><span class="sxs-lookup"><span data-stu-id="2fa68-139">userName</span></span>|<span data-ttu-id="2fa68-140">String</span><span class="sxs-lookup"><span data-stu-id="2fa68-140">String</span></span>|<span data-ttu-id="2fa68-141">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="2fa68-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="2fa68-142">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2fa68-142">deviceDisplayName</span></span>|<span data-ttu-id="2fa68-143">String</span><span class="sxs-lookup"><span data-stu-id="2fa68-143">String</span></span>|<span data-ttu-id="2fa68-144">Имя устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="2fa68-144">Device name that is being reported</span></span>|
|<span data-ttu-id="2fa68-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa68-145">lastReportedDateTime</span></span>|<span data-ttu-id="2fa68-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa68-146">DateTimeOffset</span></span>|<span data-ttu-id="2fa68-147">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="2fa68-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="2fa68-148">state</span><span class="sxs-lookup"><span data-stu-id="2fa68-148">state</span></span>|[<span data-ttu-id="2fa68-149">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="2fa68-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2fa68-150">Состояние устройства для цели.</span><span class="sxs-lookup"><span data-stu-id="2fa68-150">Device state for an intent.</span></span> <span data-ttu-id="2fa68-151">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2fa68-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2fa68-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="2fa68-152">deviceId</span></span>|<span data-ttu-id="2fa68-153">String</span><span class="sxs-lookup"><span data-stu-id="2fa68-153">String</span></span>|<span data-ttu-id="2fa68-154">Идентификатор устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="2fa68-154">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="2fa68-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fa68-155">Response</span></span>
<span data-ttu-id="2fa68-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2fa68-156">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fa68-157">Пример</span><span class="sxs-lookup"><span data-stu-id="2fa68-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fa68-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fa68-158">Request</span></span>
<span data-ttu-id="2fa68-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fa68-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="2fa68-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fa68-160">Response</span></span>
<span data-ttu-id="2fa68-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fa68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "8db75881-5881-8db7-8158-b78d8158b78d",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```




