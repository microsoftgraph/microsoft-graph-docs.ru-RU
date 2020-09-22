---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f789dbde14ad59b587e6f0c8bfe87038eb0a0ac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975873"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="f22ec-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f22ec-103">Create deviceInstallState</span></span>

<span data-ttu-id="f22ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f22ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f22ec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f22ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f22ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f22ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f22ec-107">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f22ec-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f22ec-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f22ec-108">Prerequisites</span></span>
<span data-ttu-id="f22ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f22ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f22ec-111">Permission type</span></span>|<span data-ttu-id="f22ec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f22ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f22ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f22ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f22ec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22ec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f22ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f22ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f22ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f22ec-116">Not supported.</span></span>|
|<span data-ttu-id="f22ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f22ec-117">Application</span></span>|<span data-ttu-id="f22ec-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22ec-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f22ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f22ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="f22ec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f22ec-120">Request headers</span></span>
|<span data-ttu-id="f22ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f22ec-121">Header</span></span>|<span data-ttu-id="f22ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f22ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f22ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f22ec-123">Authorization</span></span>|<span data-ttu-id="f22ec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f22ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f22ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f22ec-125">Accept</span></span>|<span data-ttu-id="f22ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f22ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f22ec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f22ec-127">Request body</span></span>
<span data-ttu-id="f22ec-128">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f22ec-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="f22ec-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="f22ec-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="f22ec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f22ec-130">Property</span></span>|<span data-ttu-id="f22ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f22ec-131">Type</span></span>|<span data-ttu-id="f22ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f22ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f22ec-133">id</span><span class="sxs-lookup"><span data-stu-id="f22ec-133">id</span></span>|<span data-ttu-id="f22ec-134">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-134">String</span></span>|<span data-ttu-id="f22ec-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f22ec-135">Key of the entity.</span></span>|
|<span data-ttu-id="f22ec-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f22ec-136">deviceName</span></span>|<span data-ttu-id="f22ec-137">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-137">String</span></span>|<span data-ttu-id="f22ec-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f22ec-138">Device name.</span></span>|
|<span data-ttu-id="f22ec-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f22ec-139">deviceId</span></span>|<span data-ttu-id="f22ec-140">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-140">String</span></span>|<span data-ttu-id="f22ec-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f22ec-141">Device Id.</span></span>|
|<span data-ttu-id="f22ec-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f22ec-142">lastSyncDateTime</span></span>|<span data-ttu-id="f22ec-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f22ec-143">DateTimeOffset</span></span>|<span data-ttu-id="f22ec-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f22ec-144">Last sync date and time.</span></span>|
|<span data-ttu-id="f22ec-145">installState</span><span class="sxs-lookup"><span data-stu-id="f22ec-145">installState</span></span>|[<span data-ttu-id="f22ec-146">installState</span><span class="sxs-lookup"><span data-stu-id="f22ec-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="f22ec-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f22ec-147">The install state of the eBook.</span></span> <span data-ttu-id="f22ec-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f22ec-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="f22ec-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="f22ec-149">errorCode</span></span>|<span data-ttu-id="f22ec-150">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-150">String</span></span>|<span data-ttu-id="f22ec-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="f22ec-151">The error code for install failures.</span></span>|
|<span data-ttu-id="f22ec-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="f22ec-152">osVersion</span></span>|<span data-ttu-id="f22ec-153">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-153">String</span></span>|<span data-ttu-id="f22ec-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="f22ec-154">OS Version.</span></span>|
|<span data-ttu-id="f22ec-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="f22ec-155">osDescription</span></span>|<span data-ttu-id="f22ec-156">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-156">String</span></span>|<span data-ttu-id="f22ec-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="f22ec-157">OS Description.</span></span>|
|<span data-ttu-id="f22ec-158">userName</span><span class="sxs-lookup"><span data-stu-id="f22ec-158">userName</span></span>|<span data-ttu-id="f22ec-159">String</span><span class="sxs-lookup"><span data-stu-id="f22ec-159">String</span></span>|<span data-ttu-id="f22ec-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="f22ec-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f22ec-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f22ec-161">Response</span></span>
<span data-ttu-id="f22ec-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f22ec-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f22ec-163">Пример</span><span class="sxs-lookup"><span data-stu-id="f22ec-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f22ec-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f22ec-164">Request</span></span>
<span data-ttu-id="f22ec-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f22ec-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="f22ec-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f22ec-166">Response</span></span>
<span data-ttu-id="f22ec-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f22ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






