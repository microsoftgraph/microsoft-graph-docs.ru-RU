---
title: Обновление объекта deviceInstallState
description: Обновление свойств объекта deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1571508451dee371e5c000b8cc8d8234c1b661a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980441"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="b80c7-103">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b80c7-103">Update deviceInstallState</span></span>

> <span data-ttu-id="b80c7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b80c7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b80c7-105">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b80c7-105">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b80c7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b80c7-106">Prerequisites</span></span>
<span data-ttu-id="b80c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b80c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b80c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b80c7-109">Permission type</span></span>|<span data-ttu-id="b80c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b80c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b80c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b80c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b80c7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80c7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b80c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b80c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b80c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b80c7-114">Not supported.</span></span>|
|<span data-ttu-id="b80c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b80c7-115">Application</span></span>|<span data-ttu-id="b80c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b80c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b80c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b80c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b80c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b80c7-118">Request headers</span></span>
|<span data-ttu-id="b80c7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b80c7-119">Header</span></span>|<span data-ttu-id="b80c7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b80c7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b80c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b80c7-121">Authorization</span></span>|<span data-ttu-id="b80c7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b80c7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b80c7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b80c7-123">Accept</span></span>|<span data-ttu-id="b80c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b80c7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b80c7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b80c7-125">Request body</span></span>
<span data-ttu-id="b80c7-126">В тексте запроса добавьте представление объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b80c7-126">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="b80c7-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b80c7-127">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="b80c7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b80c7-128">Property</span></span>|<span data-ttu-id="b80c7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b80c7-129">Type</span></span>|<span data-ttu-id="b80c7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b80c7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b80c7-131">id</span><span class="sxs-lookup"><span data-stu-id="b80c7-131">id</span></span>|<span data-ttu-id="b80c7-132">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-132">String</span></span>|<span data-ttu-id="b80c7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b80c7-133">Key of the entity.</span></span>|
|<span data-ttu-id="b80c7-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="b80c7-134">deviceName</span></span>|<span data-ttu-id="b80c7-135">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-135">String</span></span>|<span data-ttu-id="b80c7-136">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b80c7-136">Device name.</span></span>|
|<span data-ttu-id="b80c7-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="b80c7-137">deviceId</span></span>|<span data-ttu-id="b80c7-138">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-138">String</span></span>|<span data-ttu-id="b80c7-139">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="b80c7-139">Device Id.</span></span>|
|<span data-ttu-id="b80c7-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b80c7-140">lastSyncDateTime</span></span>|<span data-ttu-id="b80c7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b80c7-141">DateTimeOffset</span></span>|<span data-ttu-id="b80c7-142">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b80c7-142">Last sync date and time.</span></span>|
|<span data-ttu-id="b80c7-143">installState</span><span class="sxs-lookup"><span data-stu-id="b80c7-143">installState</span></span>|[<span data-ttu-id="b80c7-144">installState</span><span class="sxs-lookup"><span data-stu-id="b80c7-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="b80c7-145">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b80c7-145">The install state of the eBook.</span></span> <span data-ttu-id="b80c7-146">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b80c7-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="b80c7-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="b80c7-147">errorCode</span></span>|<span data-ttu-id="b80c7-148">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-148">String</span></span>|<span data-ttu-id="b80c7-149">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="b80c7-149">The error code for install failures.</span></span>|
|<span data-ttu-id="b80c7-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="b80c7-150">osVersion</span></span>|<span data-ttu-id="b80c7-151">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-151">String</span></span>|<span data-ttu-id="b80c7-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="b80c7-152">OS Version.</span></span>|
|<span data-ttu-id="b80c7-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="b80c7-153">osDescription</span></span>|<span data-ttu-id="b80c7-154">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-154">String</span></span>|<span data-ttu-id="b80c7-155">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="b80c7-155">OS Description.</span></span>|
|<span data-ttu-id="b80c7-156">userName</span><span class="sxs-lookup"><span data-stu-id="b80c7-156">userName</span></span>|<span data-ttu-id="b80c7-157">String</span><span class="sxs-lookup"><span data-stu-id="b80c7-157">String</span></span>|<span data-ttu-id="b80c7-158">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="b80c7-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="b80c7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b80c7-159">Response</span></span>
<span data-ttu-id="b80c7-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b80c7-160">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b80c7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="b80c7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="b80c7-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="b80c7-162">Request</span></span>
<span data-ttu-id="b80c7-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b80c7-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
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

### <a name="response"></a><span data-ttu-id="b80c7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b80c7-164">Response</span></span>
<span data-ttu-id="b80c7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b80c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



