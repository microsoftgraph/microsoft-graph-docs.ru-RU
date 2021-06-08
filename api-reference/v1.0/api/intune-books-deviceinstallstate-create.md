---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95822b40cb5be71994730c0c9fdf258f9af6d695
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759415"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="9fa44-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9fa44-103">Create deviceInstallState</span></span>

<span data-ttu-id="9fa44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa44-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fa44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa44-106">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="9fa44-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fa44-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9fa44-107">Prerequisites</span></span>
<span data-ttu-id="9fa44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fa44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fa44-110">Permission type</span></span>|<span data-ttu-id="9fa44-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fa44-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fa44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fa44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fa44-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa44-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fa44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fa44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fa44-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa44-115">Not supported.</span></span>|
|<span data-ttu-id="9fa44-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9fa44-116">Application</span></span>|<span data-ttu-id="9fa44-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa44-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fa44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fa44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="9fa44-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fa44-119">Request headers</span></span>
|<span data-ttu-id="9fa44-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fa44-120">Header</span></span>|<span data-ttu-id="9fa44-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9fa44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fa44-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fa44-122">Authorization</span></span>|<span data-ttu-id="9fa44-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fa44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fa44-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9fa44-124">Accept</span></span>|<span data-ttu-id="9fa44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fa44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fa44-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fa44-126">Request body</span></span>
<span data-ttu-id="9fa44-127">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fa44-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="9fa44-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="9fa44-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="9fa44-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fa44-129">Property</span></span>|<span data-ttu-id="9fa44-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9fa44-130">Type</span></span>|<span data-ttu-id="9fa44-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa44-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa44-132">id</span><span class="sxs-lookup"><span data-stu-id="9fa44-132">id</span></span>|<span data-ttu-id="9fa44-133">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-133">String</span></span>|<span data-ttu-id="9fa44-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9fa44-134">Key of the entity.</span></span>|
|<span data-ttu-id="9fa44-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="9fa44-135">deviceName</span></span>|<span data-ttu-id="9fa44-136">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-136">String</span></span>|<span data-ttu-id="9fa44-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="9fa44-137">Device name.</span></span>|
|<span data-ttu-id="9fa44-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="9fa44-138">deviceId</span></span>|<span data-ttu-id="9fa44-139">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-139">String</span></span>|<span data-ttu-id="9fa44-140">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="9fa44-140">Device Id.</span></span>|
|<span data-ttu-id="9fa44-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9fa44-141">lastSyncDateTime</span></span>|<span data-ttu-id="9fa44-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fa44-142">DateTimeOffset</span></span>|<span data-ttu-id="9fa44-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9fa44-143">Last sync date and time.</span></span>|
|<span data-ttu-id="9fa44-144">installState</span><span class="sxs-lookup"><span data-stu-id="9fa44-144">installState</span></span>|[<span data-ttu-id="9fa44-145">installState</span><span class="sxs-lookup"><span data-stu-id="9fa44-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9fa44-146">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9fa44-146">The install state of the eBook.</span></span> <span data-ttu-id="9fa44-147">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9fa44-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9fa44-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="9fa44-148">errorCode</span></span>|<span data-ttu-id="9fa44-149">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-149">String</span></span>|<span data-ttu-id="9fa44-150">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="9fa44-150">The error code for install failures.</span></span>|
|<span data-ttu-id="9fa44-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="9fa44-151">osVersion</span></span>|<span data-ttu-id="9fa44-152">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-152">String</span></span>|<span data-ttu-id="9fa44-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="9fa44-153">OS Version.</span></span>|
|<span data-ttu-id="9fa44-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="9fa44-154">osDescription</span></span>|<span data-ttu-id="9fa44-155">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-155">String</span></span>|<span data-ttu-id="9fa44-156">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="9fa44-156">OS Description.</span></span>|
|<span data-ttu-id="9fa44-157">userName</span><span class="sxs-lookup"><span data-stu-id="9fa44-157">userName</span></span>|<span data-ttu-id="9fa44-158">String</span><span class="sxs-lookup"><span data-stu-id="9fa44-158">String</span></span>|<span data-ttu-id="9fa44-159">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="9fa44-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="9fa44-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fa44-160">Response</span></span>
<span data-ttu-id="9fa44-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fa44-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fa44-162">Пример</span><span class="sxs-lookup"><span data-stu-id="9fa44-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fa44-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fa44-163">Request</span></span>
<span data-ttu-id="9fa44-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fa44-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="9fa44-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fa44-165">Response</span></span>
<span data-ttu-id="9fa44-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fa44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




