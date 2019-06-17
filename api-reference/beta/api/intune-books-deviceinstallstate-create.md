---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c27f63b6a8753335c0c95d496000f5ef23a6d32
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972536"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="b2e89-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b2e89-103">Create deviceInstallState</span></span>

> <span data-ttu-id="b2e89-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e89-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2e89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e89-106">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b2e89-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2e89-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2e89-107">Prerequisites</span></span>
<span data-ttu-id="b2e89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2e89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2e89-110">Permission type</span></span>|<span data-ttu-id="b2e89-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2e89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2e89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2e89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2e89-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e89-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2e89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2e89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2e89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e89-115">Not supported.</span></span>|
|<span data-ttu-id="b2e89-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2e89-116">Application</span></span>|<span data-ttu-id="b2e89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e89-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2e89-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2e89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="b2e89-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2e89-119">Request headers</span></span>
|<span data-ttu-id="b2e89-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2e89-120">Header</span></span>|<span data-ttu-id="b2e89-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2e89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2e89-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2e89-122">Authorization</span></span>|<span data-ttu-id="b2e89-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2e89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2e89-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2e89-124">Accept</span></span>|<span data-ttu-id="b2e89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2e89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e89-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2e89-126">Request body</span></span>
<span data-ttu-id="b2e89-127">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e89-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="b2e89-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="b2e89-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="b2e89-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e89-129">Property</span></span>|<span data-ttu-id="b2e89-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e89-130">Type</span></span>|<span data-ttu-id="b2e89-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e89-132">id</span><span class="sxs-lookup"><span data-stu-id="b2e89-132">id</span></span>|<span data-ttu-id="b2e89-133">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-133">String</span></span>|<span data-ttu-id="b2e89-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b2e89-134">Key of the entity.</span></span>|
|<span data-ttu-id="b2e89-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2e89-135">deviceName</span></span>|<span data-ttu-id="b2e89-136">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-136">String</span></span>|<span data-ttu-id="b2e89-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b2e89-137">Device name.</span></span>|
|<span data-ttu-id="b2e89-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="b2e89-138">deviceId</span></span>|<span data-ttu-id="b2e89-139">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-139">String</span></span>|<span data-ttu-id="b2e89-140">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="b2e89-140">Device Id.</span></span>|
|<span data-ttu-id="b2e89-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2e89-141">lastSyncDateTime</span></span>|<span data-ttu-id="b2e89-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e89-142">DateTimeOffset</span></span>|<span data-ttu-id="b2e89-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2e89-143">Last sync date and time.</span></span>|
|<span data-ttu-id="b2e89-144">installState</span><span class="sxs-lookup"><span data-stu-id="b2e89-144">installState</span></span>|[<span data-ttu-id="b2e89-145">installState</span><span class="sxs-lookup"><span data-stu-id="b2e89-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="b2e89-146">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b2e89-146">The install state of the eBook.</span></span> <span data-ttu-id="b2e89-147">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b2e89-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="b2e89-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="b2e89-148">errorCode</span></span>|<span data-ttu-id="b2e89-149">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-149">String</span></span>|<span data-ttu-id="b2e89-150">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="b2e89-150">The error code for install failures.</span></span>|
|<span data-ttu-id="b2e89-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="b2e89-151">osVersion</span></span>|<span data-ttu-id="b2e89-152">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-152">String</span></span>|<span data-ttu-id="b2e89-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="b2e89-153">OS Version.</span></span>|
|<span data-ttu-id="b2e89-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="b2e89-154">osDescription</span></span>|<span data-ttu-id="b2e89-155">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-155">String</span></span>|<span data-ttu-id="b2e89-156">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="b2e89-156">OS Description.</span></span>|
|<span data-ttu-id="b2e89-157">userName</span><span class="sxs-lookup"><span data-stu-id="b2e89-157">userName</span></span>|<span data-ttu-id="b2e89-158">String</span><span class="sxs-lookup"><span data-stu-id="b2e89-158">String</span></span>|<span data-ttu-id="b2e89-159">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="b2e89-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="b2e89-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e89-160">Response</span></span>
<span data-ttu-id="b2e89-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2e89-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e89-162">Пример</span><span class="sxs-lookup"><span data-stu-id="b2e89-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2e89-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2e89-163">Request</span></span>
<span data-ttu-id="b2e89-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2e89-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2e89-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e89-165">Response</span></span>
<span data-ttu-id="b2e89-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2e89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





