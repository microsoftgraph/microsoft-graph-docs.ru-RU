---
title: Обновление объекта deviceInstallState
description: Обновление свойств объекта deviceInstallState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcf4b192bfca5af888cd22b563cb15fd80a9d546
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760531"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="fc914-103">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="fc914-103">Update deviceInstallState</span></span>

> <span data-ttu-id="fc914-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc914-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc914-106">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="fc914-106">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc914-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc914-107">Prerequisites</span></span>
<span data-ttu-id="fc914-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc914-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc914-110">Permission type</span></span>|<span data-ttu-id="fc914-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc914-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc914-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc914-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc914-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc914-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc914-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc914-115">Not supported.</span></span>|
|<span data-ttu-id="fc914-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc914-116">Application</span></span>|<span data-ttu-id="fc914-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc914-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc914-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="fc914-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc914-119">Request headers</span></span>
|<span data-ttu-id="fc914-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc914-120">Header</span></span>|<span data-ttu-id="fc914-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc914-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc914-122">Authorization</span></span>|<span data-ttu-id="fc914-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc914-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc914-124">Accept</span></span>|<span data-ttu-id="fc914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc914-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc914-126">Request body</span></span>
<span data-ttu-id="fc914-127">В тексте запроса добавьте представление объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc914-127">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="fc914-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="fc914-128">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="fc914-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc914-129">Property</span></span>|<span data-ttu-id="fc914-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc914-130">Type</span></span>|<span data-ttu-id="fc914-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc914-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc914-132">id</span><span class="sxs-lookup"><span data-stu-id="fc914-132">id</span></span>|<span data-ttu-id="fc914-133">String</span><span class="sxs-lookup"><span data-stu-id="fc914-133">String</span></span>|<span data-ttu-id="fc914-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc914-134">Key of the entity.</span></span>|
|<span data-ttu-id="fc914-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="fc914-135">deviceName</span></span>|<span data-ttu-id="fc914-136">String</span><span class="sxs-lookup"><span data-stu-id="fc914-136">String</span></span>|<span data-ttu-id="fc914-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fc914-137">Device name.</span></span>|
|<span data-ttu-id="fc914-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="fc914-138">deviceId</span></span>|<span data-ttu-id="fc914-139">String</span><span class="sxs-lookup"><span data-stu-id="fc914-139">String</span></span>|<span data-ttu-id="fc914-140">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="fc914-140">Device Id.</span></span>|
|<span data-ttu-id="fc914-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fc914-141">lastSyncDateTime</span></span>|<span data-ttu-id="fc914-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc914-142">DateTimeOffset</span></span>|<span data-ttu-id="fc914-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fc914-143">Last sync date and time.</span></span>|
|<span data-ttu-id="fc914-144">installState</span><span class="sxs-lookup"><span data-stu-id="fc914-144">installState</span></span>|[<span data-ttu-id="fc914-145">installState</span><span class="sxs-lookup"><span data-stu-id="fc914-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="fc914-146">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fc914-146">The install state of the eBook.</span></span> <span data-ttu-id="fc914-147">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fc914-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="fc914-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="fc914-148">errorCode</span></span>|<span data-ttu-id="fc914-149">String</span><span class="sxs-lookup"><span data-stu-id="fc914-149">String</span></span>|<span data-ttu-id="fc914-150">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="fc914-150">The error code for install failures.</span></span>|
|<span data-ttu-id="fc914-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="fc914-151">osVersion</span></span>|<span data-ttu-id="fc914-152">String</span><span class="sxs-lookup"><span data-stu-id="fc914-152">String</span></span>|<span data-ttu-id="fc914-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="fc914-153">OS Version.</span></span>|
|<span data-ttu-id="fc914-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="fc914-154">osDescription</span></span>|<span data-ttu-id="fc914-155">String</span><span class="sxs-lookup"><span data-stu-id="fc914-155">String</span></span>|<span data-ttu-id="fc914-156">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="fc914-156">OS Description.</span></span>|
|<span data-ttu-id="fc914-157">userName</span><span class="sxs-lookup"><span data-stu-id="fc914-157">userName</span></span>|<span data-ttu-id="fc914-158">String</span><span class="sxs-lookup"><span data-stu-id="fc914-158">String</span></span>|<span data-ttu-id="fc914-159">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="fc914-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="fc914-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc914-160">Response</span></span>
<span data-ttu-id="fc914-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc914-161">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc914-162">Пример</span><span class="sxs-lookup"><span data-stu-id="fc914-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc914-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc914-163">Request</span></span>
<span data-ttu-id="fc914-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc914-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="fc914-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc914-165">Response</span></span>
<span data-ttu-id="fc914-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc914-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```




