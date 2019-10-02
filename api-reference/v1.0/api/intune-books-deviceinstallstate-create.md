---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 373d0f62ce428bfe40b9058d7c21be2a533e35bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357999"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="dd364-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dd364-103">Create deviceInstallState</span></span>

> <span data-ttu-id="dd364-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd364-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd364-105">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="dd364-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd364-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd364-106">Prerequisites</span></span>
<span data-ttu-id="dd364-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd364-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd364-109">Permission type</span></span>|<span data-ttu-id="dd364-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd364-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd364-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd364-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd364-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd364-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd364-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd364-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd364-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd364-114">Not supported.</span></span>|
|<span data-ttu-id="dd364-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd364-115">Application</span></span>|<span data-ttu-id="dd364-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd364-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd364-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd364-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="dd364-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd364-118">Request headers</span></span>
|<span data-ttu-id="dd364-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd364-119">Header</span></span>|<span data-ttu-id="dd364-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dd364-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd364-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd364-121">Authorization</span></span>|<span data-ttu-id="dd364-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd364-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd364-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dd364-123">Accept</span></span>|<span data-ttu-id="dd364-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd364-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd364-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd364-125">Request body</span></span>
<span data-ttu-id="dd364-126">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd364-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="dd364-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="dd364-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="dd364-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd364-128">Property</span></span>|<span data-ttu-id="dd364-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dd364-129">Type</span></span>|<span data-ttu-id="dd364-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dd364-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd364-131">id</span><span class="sxs-lookup"><span data-stu-id="dd364-131">id</span></span>|<span data-ttu-id="dd364-132">String</span><span class="sxs-lookup"><span data-stu-id="dd364-132">String</span></span>|<span data-ttu-id="dd364-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd364-133">Key of the entity.</span></span>|
|<span data-ttu-id="dd364-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="dd364-134">deviceName</span></span>|<span data-ttu-id="dd364-135">String</span><span class="sxs-lookup"><span data-stu-id="dd364-135">String</span></span>|<span data-ttu-id="dd364-136">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="dd364-136">Device name.</span></span>|
|<span data-ttu-id="dd364-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="dd364-137">deviceId</span></span>|<span data-ttu-id="dd364-138">String</span><span class="sxs-lookup"><span data-stu-id="dd364-138">String</span></span>|<span data-ttu-id="dd364-139">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="dd364-139">Device Id.</span></span>|
|<span data-ttu-id="dd364-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dd364-140">lastSyncDateTime</span></span>|<span data-ttu-id="dd364-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd364-141">DateTimeOffset</span></span>|<span data-ttu-id="dd364-142">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dd364-142">Last sync date and time.</span></span>|
|<span data-ttu-id="dd364-143">installState</span><span class="sxs-lookup"><span data-stu-id="dd364-143">installState</span></span>|[<span data-ttu-id="dd364-144">installState</span><span class="sxs-lookup"><span data-stu-id="dd364-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="dd364-145">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="dd364-145">The install state of the eBook.</span></span> <span data-ttu-id="dd364-146">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dd364-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="dd364-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="dd364-147">errorCode</span></span>|<span data-ttu-id="dd364-148">String</span><span class="sxs-lookup"><span data-stu-id="dd364-148">String</span></span>|<span data-ttu-id="dd364-149">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="dd364-149">The error code for install failures.</span></span>|
|<span data-ttu-id="dd364-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="dd364-150">osVersion</span></span>|<span data-ttu-id="dd364-151">String</span><span class="sxs-lookup"><span data-stu-id="dd364-151">String</span></span>|<span data-ttu-id="dd364-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="dd364-152">OS Version.</span></span>|
|<span data-ttu-id="dd364-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="dd364-153">osDescription</span></span>|<span data-ttu-id="dd364-154">String</span><span class="sxs-lookup"><span data-stu-id="dd364-154">String</span></span>|<span data-ttu-id="dd364-155">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="dd364-155">OS Description.</span></span>|
|<span data-ttu-id="dd364-156">userName</span><span class="sxs-lookup"><span data-stu-id="dd364-156">userName</span></span>|<span data-ttu-id="dd364-157">String</span><span class="sxs-lookup"><span data-stu-id="dd364-157">String</span></span>|<span data-ttu-id="dd364-158">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="dd364-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="dd364-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd364-159">Response</span></span>
<span data-ttu-id="dd364-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd364-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd364-161">Пример</span><span class="sxs-lookup"><span data-stu-id="dd364-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd364-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd364-162">Request</span></span>
<span data-ttu-id="dd364-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd364-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd364-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd364-164">Response</span></span>
<span data-ttu-id="dd364-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd364-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




