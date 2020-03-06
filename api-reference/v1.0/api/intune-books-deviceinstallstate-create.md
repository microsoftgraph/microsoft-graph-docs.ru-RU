---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5d57957517f78949ce166f70cbd083a6dafec07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515723"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="227bd-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="227bd-103">Create deviceInstallState</span></span>

<span data-ttu-id="227bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="227bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="227bd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="227bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="227bd-106">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="227bd-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="227bd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="227bd-107">Prerequisites</span></span>
<span data-ttu-id="227bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="227bd-110">Permission type</span></span>|<span data-ttu-id="227bd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="227bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="227bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="227bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="227bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="227bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="227bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="227bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227bd-115">Not supported.</span></span>|
|<span data-ttu-id="227bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="227bd-116">Application</span></span>|<span data-ttu-id="227bd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="227bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="227bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="227bd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="227bd-119">Request headers</span></span>
|<span data-ttu-id="227bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="227bd-120">Header</span></span>|<span data-ttu-id="227bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="227bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="227bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="227bd-122">Authorization</span></span>|<span data-ttu-id="227bd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="227bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="227bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="227bd-124">Accept</span></span>|<span data-ttu-id="227bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="227bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="227bd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="227bd-126">Request body</span></span>
<span data-ttu-id="227bd-127">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="227bd-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="227bd-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="227bd-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="227bd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="227bd-129">Property</span></span>|<span data-ttu-id="227bd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="227bd-130">Type</span></span>|<span data-ttu-id="227bd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="227bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227bd-132">id</span><span class="sxs-lookup"><span data-stu-id="227bd-132">id</span></span>|<span data-ttu-id="227bd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-133">String</span></span>|<span data-ttu-id="227bd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="227bd-134">Key of the entity.</span></span>|
|<span data-ttu-id="227bd-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="227bd-135">deviceName</span></span>|<span data-ttu-id="227bd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-136">String</span></span>|<span data-ttu-id="227bd-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="227bd-137">Device name.</span></span>|
|<span data-ttu-id="227bd-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="227bd-138">deviceId</span></span>|<span data-ttu-id="227bd-139">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-139">String</span></span>|<span data-ttu-id="227bd-140">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="227bd-140">Device Id.</span></span>|
|<span data-ttu-id="227bd-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="227bd-141">lastSyncDateTime</span></span>|<span data-ttu-id="227bd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="227bd-142">DateTimeOffset</span></span>|<span data-ttu-id="227bd-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="227bd-143">Last sync date and time.</span></span>|
|<span data-ttu-id="227bd-144">installState</span><span class="sxs-lookup"><span data-stu-id="227bd-144">installState</span></span>|[<span data-ttu-id="227bd-145">installState</span><span class="sxs-lookup"><span data-stu-id="227bd-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="227bd-146">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="227bd-146">The install state of the eBook.</span></span> <span data-ttu-id="227bd-147">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="227bd-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="227bd-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="227bd-148">errorCode</span></span>|<span data-ttu-id="227bd-149">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-149">String</span></span>|<span data-ttu-id="227bd-150">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="227bd-150">The error code for install failures.</span></span>|
|<span data-ttu-id="227bd-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="227bd-151">osVersion</span></span>|<span data-ttu-id="227bd-152">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-152">String</span></span>|<span data-ttu-id="227bd-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="227bd-153">OS Version.</span></span>|
|<span data-ttu-id="227bd-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="227bd-154">osDescription</span></span>|<span data-ttu-id="227bd-155">Строка</span><span class="sxs-lookup"><span data-stu-id="227bd-155">String</span></span>|<span data-ttu-id="227bd-156">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="227bd-156">OS Description.</span></span>|
|<span data-ttu-id="227bd-157">userName</span><span class="sxs-lookup"><span data-stu-id="227bd-157">userName</span></span>|<span data-ttu-id="227bd-158">String</span><span class="sxs-lookup"><span data-stu-id="227bd-158">String</span></span>|<span data-ttu-id="227bd-159">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="227bd-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="227bd-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="227bd-160">Response</span></span>
<span data-ttu-id="227bd-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="227bd-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="227bd-162">Пример</span><span class="sxs-lookup"><span data-stu-id="227bd-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="227bd-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="227bd-163">Request</span></span>
<span data-ttu-id="227bd-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="227bd-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="227bd-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="227bd-165">Response</span></span>
<span data-ttu-id="227bd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="227bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




