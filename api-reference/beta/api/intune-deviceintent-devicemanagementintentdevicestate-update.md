---
title: Обновление Девицеманажементинтентдевицестате
description: Обновление свойств объекта Девицеманажементинтентдевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4711d0942ea1d0bb3dd6a328b747373bcf3e52c9
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522603"
---
# <a name="update-devicemanagementintentdevicestate"></a><span data-ttu-id="4a33f-103">Обновление Девицеманажементинтентдевицестате</span><span class="sxs-lookup"><span data-stu-id="4a33f-103">Update deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="4a33f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a33f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a33f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a33f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a33f-106">Обновление свойств объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4a33f-106">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a33f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a33f-107">Prerequisites</span></span>
<span data-ttu-id="4a33f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a33f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a33f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a33f-110">Permission type</span></span>|<span data-ttu-id="4a33f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a33f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a33f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a33f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a33f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a33f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a33f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a33f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a33f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a33f-115">Not supported.</span></span>|
|<span data-ttu-id="4a33f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a33f-116">Application</span></span>|<span data-ttu-id="4a33f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a33f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a33f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a33f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4a33f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a33f-119">Request headers</span></span>
|<span data-ttu-id="4a33f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a33f-120">Header</span></span>|<span data-ttu-id="4a33f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a33f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a33f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a33f-122">Authorization</span></span>|<span data-ttu-id="4a33f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a33f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a33f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a33f-124">Accept</span></span>|<span data-ttu-id="4a33f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a33f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a33f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a33f-126">Request body</span></span>
<span data-ttu-id="4a33f-127">В тексте запроса добавьте представление объекта [Девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a33f-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

<span data-ttu-id="4a33f-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="4a33f-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

|<span data-ttu-id="4a33f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a33f-129">Property</span></span>|<span data-ttu-id="4a33f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a33f-130">Type</span></span>|<span data-ttu-id="4a33f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a33f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a33f-132">id</span><span class="sxs-lookup"><span data-stu-id="4a33f-132">id</span></span>|<span data-ttu-id="4a33f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4a33f-133">String</span></span>|<span data-ttu-id="4a33f-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="4a33f-134">The ID</span></span>|
|<span data-ttu-id="4a33f-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a33f-135">userPrincipalName</span></span>|<span data-ttu-id="4a33f-136">String</span><span class="sxs-lookup"><span data-stu-id="4a33f-136">String</span></span>|<span data-ttu-id="4a33f-137">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="4a33f-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="4a33f-138">userName</span><span class="sxs-lookup"><span data-stu-id="4a33f-138">userName</span></span>|<span data-ttu-id="4a33f-139">String</span><span class="sxs-lookup"><span data-stu-id="4a33f-139">String</span></span>|<span data-ttu-id="4a33f-140">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="4a33f-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="4a33f-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a33f-141">deviceDisplayName</span></span>|<span data-ttu-id="4a33f-142">String</span><span class="sxs-lookup"><span data-stu-id="4a33f-142">String</span></span>|<span data-ttu-id="4a33f-143">Имя устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="4a33f-143">Device name that is being reported</span></span>|
|<span data-ttu-id="4a33f-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a33f-144">lastReportedDateTime</span></span>|<span data-ttu-id="4a33f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a33f-145">DateTimeOffset</span></span>|<span data-ttu-id="4a33f-146">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="4a33f-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="4a33f-147">state</span><span class="sxs-lookup"><span data-stu-id="4a33f-147">state</span></span>|[<span data-ttu-id="4a33f-148">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="4a33f-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4a33f-149">Состояние устройства для цели.</span><span class="sxs-lookup"><span data-stu-id="4a33f-149">Device state for an intent.</span></span> <span data-ttu-id="4a33f-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4a33f-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="4a33f-151">deviceId</span></span>|<span data-ttu-id="4a33f-152">String</span><span class="sxs-lookup"><span data-stu-id="4a33f-152">String</span></span>|<span data-ttu-id="4a33f-153">Идентификатор устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="4a33f-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="4a33f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a33f-154">Response</span></span>
<span data-ttu-id="4a33f-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a33f-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a33f-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4a33f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a33f-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a33f-157">Request</span></span>
<span data-ttu-id="4a33f-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a33f-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="4a33f-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a33f-159">Response</span></span>
<span data-ttu-id="4a33f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a33f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







