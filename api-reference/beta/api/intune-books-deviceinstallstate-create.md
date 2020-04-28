---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f2d9ba02725310958f5ce52b6b0fb48a76e16a9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392839"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="c3a25-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="c3a25-103">Create deviceInstallState</span></span>

<span data-ttu-id="c3a25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3a25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3a25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a25-107">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="c3a25-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a25-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3a25-108">Prerequisites</span></span>
<span data-ttu-id="c3a25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3a25-111">Permission type</span></span>|<span data-ttu-id="c3a25-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3a25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3a25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3a25-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a25-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3a25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a25-116">Not supported.</span></span>|
|<span data-ttu-id="c3a25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3a25-117">Application</span></span>|<span data-ttu-id="c3a25-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a25-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3a25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c3a25-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3a25-120">Request headers</span></span>
|<span data-ttu-id="c3a25-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3a25-121">Header</span></span>|<span data-ttu-id="c3a25-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3a25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3a25-123">Authorization</span></span>|<span data-ttu-id="c3a25-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3a25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3a25-125">Accept</span></span>|<span data-ttu-id="c3a25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a25-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3a25-127">Request body</span></span>
<span data-ttu-id="c3a25-128">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3a25-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="c3a25-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="c3a25-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="c3a25-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3a25-130">Property</span></span>|<span data-ttu-id="c3a25-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3a25-131">Type</span></span>|<span data-ttu-id="c3a25-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a25-133">id</span><span class="sxs-lookup"><span data-stu-id="c3a25-133">id</span></span>|<span data-ttu-id="c3a25-134">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-134">String</span></span>|<span data-ttu-id="c3a25-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3a25-135">Key of the entity.</span></span>|
|<span data-ttu-id="c3a25-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c3a25-136">deviceName</span></span>|<span data-ttu-id="c3a25-137">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-137">String</span></span>|<span data-ttu-id="c3a25-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="c3a25-138">Device name.</span></span>|
|<span data-ttu-id="c3a25-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="c3a25-139">deviceId</span></span>|<span data-ttu-id="c3a25-140">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-140">String</span></span>|<span data-ttu-id="c3a25-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c3a25-141">Device Id.</span></span>|
|<span data-ttu-id="c3a25-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a25-142">lastSyncDateTime</span></span>|<span data-ttu-id="c3a25-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a25-143">DateTimeOffset</span></span>|<span data-ttu-id="c3a25-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c3a25-144">Last sync date and time.</span></span>|
|<span data-ttu-id="c3a25-145">installState</span><span class="sxs-lookup"><span data-stu-id="c3a25-145">installState</span></span>|[<span data-ttu-id="c3a25-146">installState</span><span class="sxs-lookup"><span data-stu-id="c3a25-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="c3a25-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c3a25-147">The install state of the eBook.</span></span> <span data-ttu-id="c3a25-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c3a25-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="c3a25-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="c3a25-149">errorCode</span></span>|<span data-ttu-id="c3a25-150">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-150">String</span></span>|<span data-ttu-id="c3a25-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="c3a25-151">The error code for install failures.</span></span>|
|<span data-ttu-id="c3a25-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="c3a25-152">osVersion</span></span>|<span data-ttu-id="c3a25-153">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-153">String</span></span>|<span data-ttu-id="c3a25-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="c3a25-154">OS Version.</span></span>|
|<span data-ttu-id="c3a25-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="c3a25-155">osDescription</span></span>|<span data-ttu-id="c3a25-156">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-156">String</span></span>|<span data-ttu-id="c3a25-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="c3a25-157">OS Description.</span></span>|
|<span data-ttu-id="c3a25-158">userName</span><span class="sxs-lookup"><span data-stu-id="c3a25-158">userName</span></span>|<span data-ttu-id="c3a25-159">String</span><span class="sxs-lookup"><span data-stu-id="c3a25-159">String</span></span>|<span data-ttu-id="c3a25-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="c3a25-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="c3a25-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a25-161">Response</span></span>
<span data-ttu-id="c3a25-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3a25-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a25-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a25-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a25-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a25-164">Request</span></span>
<span data-ttu-id="c3a25-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3a25-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3a25-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a25-166">Response</span></span>
<span data-ttu-id="c3a25-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3a25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



