---
title: Создание Девицеманажементинтентдевицестате
description: Создание нового объекта Девицеманажементинтентдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f70b2f77808fe4c2b4f15b54198d77d39a484486
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960295"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="7c977-103">Создание Девицеманажементинтентдевицестате</span><span class="sxs-lookup"><span data-stu-id="7c977-103">Create deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="7c977-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c977-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c977-106">Создание нового объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7c977-106">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c977-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c977-107">Prerequisites</span></span>
<span data-ttu-id="7c977-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c977-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c977-110">Permission type</span></span>|<span data-ttu-id="7c977-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c977-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c977-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c977-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c977-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c977-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c977-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c977-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c977-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c977-115">Not supported.</span></span>|
|<span data-ttu-id="7c977-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c977-116">Application</span></span>|<span data-ttu-id="7c977-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c977-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c977-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c977-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="7c977-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c977-119">Request headers</span></span>
|<span data-ttu-id="7c977-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c977-120">Header</span></span>|<span data-ttu-id="7c977-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c977-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c977-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c977-122">Authorization</span></span>|<span data-ttu-id="7c977-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c977-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c977-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c977-124">Accept</span></span>|<span data-ttu-id="7c977-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c977-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c977-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c977-126">Request body</span></span>
<span data-ttu-id="7c977-127">В тексте запроса добавьте представление объекта Девицеманажементинтентдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c977-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="7c977-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентдевицестате.</span><span class="sxs-lookup"><span data-stu-id="7c977-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="7c977-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c977-129">Property</span></span>|<span data-ttu-id="7c977-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c977-130">Type</span></span>|<span data-ttu-id="7c977-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c977-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c977-132">id</span><span class="sxs-lookup"><span data-stu-id="7c977-132">id</span></span>|<span data-ttu-id="7c977-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7c977-133">String</span></span>|<span data-ttu-id="7c977-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="7c977-134">The ID</span></span>|
|<span data-ttu-id="7c977-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c977-135">userPrincipalName</span></span>|<span data-ttu-id="7c977-136">String</span><span class="sxs-lookup"><span data-stu-id="7c977-136">String</span></span>|<span data-ttu-id="7c977-137">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="7c977-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="7c977-138">userName</span><span class="sxs-lookup"><span data-stu-id="7c977-138">userName</span></span>|<span data-ttu-id="7c977-139">String</span><span class="sxs-lookup"><span data-stu-id="7c977-139">String</span></span>|<span data-ttu-id="7c977-140">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="7c977-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="7c977-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c977-141">deviceDisplayName</span></span>|<span data-ttu-id="7c977-142">String</span><span class="sxs-lookup"><span data-stu-id="7c977-142">String</span></span>|<span data-ttu-id="7c977-143">Имя устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="7c977-143">Device name that is being reported</span></span>|
|<span data-ttu-id="7c977-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c977-144">lastReportedDateTime</span></span>|<span data-ttu-id="7c977-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c977-145">DateTimeOffset</span></span>|<span data-ttu-id="7c977-146">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="7c977-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="7c977-147">состояние</span><span class="sxs-lookup"><span data-stu-id="7c977-147">state</span></span>|[<span data-ttu-id="7c977-148">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="7c977-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7c977-149">Состояние устройства для цели.</span><span class="sxs-lookup"><span data-stu-id="7c977-149">Device state for an intent.</span></span> <span data-ttu-id="7c977-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7c977-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7c977-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="7c977-151">deviceId</span></span>|<span data-ttu-id="7c977-152">String</span><span class="sxs-lookup"><span data-stu-id="7c977-152">String</span></span>|<span data-ttu-id="7c977-153">Идентификатор устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="7c977-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="7c977-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c977-154">Response</span></span>
<span data-ttu-id="7c977-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c977-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c977-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7c977-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c977-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c977-157">Request</span></span>
<span data-ttu-id="7c977-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c977-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c977-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c977-159">Response</span></span>
<span data-ttu-id="7c977-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c977-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





