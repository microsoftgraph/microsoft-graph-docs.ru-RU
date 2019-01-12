---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7e37857cfa7d7c8820844f506b59d50933c5866
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962543"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="cedba-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="cedba-103">Create deviceInstallState</span></span>

> <span data-ttu-id="cedba-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cedba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cedba-105">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="cedba-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cedba-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cedba-106">Prerequisites</span></span>
<span data-ttu-id="cedba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cedba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cedba-109">Permission type</span></span>|<span data-ttu-id="cedba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cedba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cedba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cedba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cedba-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cedba-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cedba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cedba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cedba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cedba-114">Not supported.</span></span>|
|<span data-ttu-id="cedba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cedba-115">Application</span></span>|<span data-ttu-id="cedba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cedba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cedba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cedba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="cedba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cedba-118">Request headers</span></span>
|<span data-ttu-id="cedba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cedba-119">Header</span></span>|<span data-ttu-id="cedba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cedba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cedba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cedba-121">Authorization</span></span>|<span data-ttu-id="cedba-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cedba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cedba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cedba-123">Accept</span></span>|<span data-ttu-id="cedba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cedba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedba-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cedba-125">Request body</span></span>
<span data-ttu-id="cedba-126">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cedba-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="cedba-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="cedba-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="cedba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cedba-128">Property</span></span>|<span data-ttu-id="cedba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cedba-129">Type</span></span>|<span data-ttu-id="cedba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cedba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cedba-131">id</span><span class="sxs-lookup"><span data-stu-id="cedba-131">id</span></span>|<span data-ttu-id="cedba-132">String</span><span class="sxs-lookup"><span data-stu-id="cedba-132">String</span></span>|<span data-ttu-id="cedba-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cedba-133">Key of the entity.</span></span>|
|<span data-ttu-id="cedba-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="cedba-134">deviceName</span></span>|<span data-ttu-id="cedba-135">String</span><span class="sxs-lookup"><span data-stu-id="cedba-135">String</span></span>|<span data-ttu-id="cedba-136">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="cedba-136">Device name.</span></span>|
|<span data-ttu-id="cedba-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="cedba-137">deviceId</span></span>|<span data-ttu-id="cedba-138">String</span><span class="sxs-lookup"><span data-stu-id="cedba-138">String</span></span>|<span data-ttu-id="cedba-139">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="cedba-139">Device Id.</span></span>|
|<span data-ttu-id="cedba-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cedba-140">lastSyncDateTime</span></span>|<span data-ttu-id="cedba-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cedba-141">DateTimeOffset</span></span>|<span data-ttu-id="cedba-142">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cedba-142">Last sync date and time.</span></span>|
|<span data-ttu-id="cedba-143">installState</span><span class="sxs-lookup"><span data-stu-id="cedba-143">installState</span></span>|[<span data-ttu-id="cedba-144">installState</span><span class="sxs-lookup"><span data-stu-id="cedba-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="cedba-145">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cedba-145">The install state of the eBook.</span></span> <span data-ttu-id="cedba-146">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cedba-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="cedba-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="cedba-147">errorCode</span></span>|<span data-ttu-id="cedba-148">String</span><span class="sxs-lookup"><span data-stu-id="cedba-148">String</span></span>|<span data-ttu-id="cedba-149">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="cedba-149">The error code for install failures.</span></span>|
|<span data-ttu-id="cedba-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="cedba-150">osVersion</span></span>|<span data-ttu-id="cedba-151">String</span><span class="sxs-lookup"><span data-stu-id="cedba-151">String</span></span>|<span data-ttu-id="cedba-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="cedba-152">OS Version.</span></span>|
|<span data-ttu-id="cedba-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="cedba-153">osDescription</span></span>|<span data-ttu-id="cedba-154">String</span><span class="sxs-lookup"><span data-stu-id="cedba-154">String</span></span>|<span data-ttu-id="cedba-155">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="cedba-155">OS Description.</span></span>|
|<span data-ttu-id="cedba-156">userName</span><span class="sxs-lookup"><span data-stu-id="cedba-156">userName</span></span>|<span data-ttu-id="cedba-157">String</span><span class="sxs-lookup"><span data-stu-id="cedba-157">String</span></span>|<span data-ttu-id="cedba-158">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="cedba-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="cedba-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="cedba-159">Response</span></span>
<span data-ttu-id="cedba-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cedba-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedba-161">Пример</span><span class="sxs-lookup"><span data-stu-id="cedba-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="cedba-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="cedba-162">Request</span></span>
<span data-ttu-id="cedba-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cedba-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cedba-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="cedba-164">Response</span></span>
<span data-ttu-id="cedba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cedba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



