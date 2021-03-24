---
title: Обновление объекта deviceInstallState
description: Обновление свойств объекта deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 940c2e88761aefa5bc18c71b7d785c5ceb0b9647
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131892"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="c3c03-103">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="c3c03-103">Update deviceInstallState</span></span>

<span data-ttu-id="c3c03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3c03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3c03-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3c03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3c03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3c03-107">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="c3c03-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3c03-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3c03-108">Prerequisites</span></span>
<span data-ttu-id="c3c03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c03-111">Permission type</span></span>|<span data-ttu-id="c3c03-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3c03-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c03-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3c03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c03-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c03-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3c03-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3c03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c03-116">Not supported.</span></span>|
|<span data-ttu-id="c3c03-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3c03-117">Application</span></span>|<span data-ttu-id="c3c03-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c03-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3c03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c3c03-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3c03-120">Request headers</span></span>
|<span data-ttu-id="c3c03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3c03-121">Header</span></span>|<span data-ttu-id="c3c03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3c03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3c03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3c03-123">Authorization</span></span>|<span data-ttu-id="c3c03-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3c03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3c03-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3c03-125">Accept</span></span>|<span data-ttu-id="c3c03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3c03-127">Request body</span></span>
<span data-ttu-id="c3c03-128">В тексте запроса добавьте представление объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3c03-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="c3c03-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="c3c03-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="c3c03-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3c03-130">Property</span></span>|<span data-ttu-id="c3c03-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3c03-131">Type</span></span>|<span data-ttu-id="c3c03-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3c03-133">id</span><span class="sxs-lookup"><span data-stu-id="c3c03-133">id</span></span>|<span data-ttu-id="c3c03-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3c03-134">String</span></span>|<span data-ttu-id="c3c03-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3c03-135">Key of the entity.</span></span>|
|<span data-ttu-id="c3c03-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c3c03-136">deviceName</span></span>|<span data-ttu-id="c3c03-137">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-137">String</span></span>|<span data-ttu-id="c3c03-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="c3c03-138">Device name.</span></span>|
|<span data-ttu-id="c3c03-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="c3c03-139">deviceId</span></span>|<span data-ttu-id="c3c03-140">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-140">String</span></span>|<span data-ttu-id="c3c03-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c3c03-141">Device Id.</span></span>|
|<span data-ttu-id="c3c03-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c3c03-142">lastSyncDateTime</span></span>|<span data-ttu-id="c3c03-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3c03-143">DateTimeOffset</span></span>|<span data-ttu-id="c3c03-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c3c03-144">Last sync date and time.</span></span>|
|<span data-ttu-id="c3c03-145">installState</span><span class="sxs-lookup"><span data-stu-id="c3c03-145">installState</span></span>|[<span data-ttu-id="c3c03-146">installState</span><span class="sxs-lookup"><span data-stu-id="c3c03-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="c3c03-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c3c03-147">The install state of the eBook.</span></span> <span data-ttu-id="c3c03-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c3c03-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="c3c03-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="c3c03-149">errorCode</span></span>|<span data-ttu-id="c3c03-150">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-150">String</span></span>|<span data-ttu-id="c3c03-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="c3c03-151">The error code for install failures.</span></span>|
|<span data-ttu-id="c3c03-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="c3c03-152">osVersion</span></span>|<span data-ttu-id="c3c03-153">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-153">String</span></span>|<span data-ttu-id="c3c03-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="c3c03-154">OS Version.</span></span>|
|<span data-ttu-id="c3c03-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="c3c03-155">osDescription</span></span>|<span data-ttu-id="c3c03-156">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-156">String</span></span>|<span data-ttu-id="c3c03-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="c3c03-157">OS Description.</span></span>|
|<span data-ttu-id="c3c03-158">userName</span><span class="sxs-lookup"><span data-stu-id="c3c03-158">userName</span></span>|<span data-ttu-id="c3c03-159">String</span><span class="sxs-lookup"><span data-stu-id="c3c03-159">String</span></span>|<span data-ttu-id="c3c03-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="c3c03-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="c3c03-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c03-161">Response</span></span>
<span data-ttu-id="c3c03-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3c03-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c03-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c3c03-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3c03-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3c03-164">Request</span></span>
<span data-ttu-id="c3c03-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3c03-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3c03-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c03-166">Response</span></span>
<span data-ttu-id="c3c03-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3c03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




