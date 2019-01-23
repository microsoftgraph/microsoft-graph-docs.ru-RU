---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bdede47f4aeda2d4dfc4558464b4760066fa7e18
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413159"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="e45d3-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="e45d3-103">Create deviceInstallState</span></span>

> <span data-ttu-id="e45d3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e45d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e45d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e45d3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e45d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45d3-107">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="e45d3-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e45d3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e45d3-108">Prerequisites</span></span>
<span data-ttu-id="e45d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e45d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e45d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e45d3-111">Permission type</span></span>|<span data-ttu-id="e45d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e45d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e45d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e45d3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45d3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e45d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e45d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45d3-116">Not supported.</span></span>|
|<span data-ttu-id="e45d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e45d3-117">Application</span></span>|<span data-ttu-id="e45d3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e45d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="e45d3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e45d3-120">Request headers</span></span>
|<span data-ttu-id="e45d3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e45d3-121">Header</span></span>|<span data-ttu-id="e45d3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e45d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e45d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e45d3-123">Authorization</span></span>|<span data-ttu-id="e45d3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e45d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e45d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e45d3-125">Accept</span></span>|<span data-ttu-id="e45d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e45d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e45d3-127">Request body</span></span>
<span data-ttu-id="e45d3-128">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e45d3-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="e45d3-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="e45d3-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="e45d3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45d3-130">Property</span></span>|<span data-ttu-id="e45d3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e45d3-131">Type</span></span>|<span data-ttu-id="e45d3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e45d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45d3-133">id</span><span class="sxs-lookup"><span data-stu-id="e45d3-133">id</span></span>|<span data-ttu-id="e45d3-134">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-134">String</span></span>|<span data-ttu-id="e45d3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e45d3-135">Key of the entity.</span></span>|
|<span data-ttu-id="e45d3-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e45d3-136">deviceName</span></span>|<span data-ttu-id="e45d3-137">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-137">String</span></span>|<span data-ttu-id="e45d3-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="e45d3-138">Device name.</span></span>|
|<span data-ttu-id="e45d3-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="e45d3-139">deviceId</span></span>|<span data-ttu-id="e45d3-140">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-140">String</span></span>|<span data-ttu-id="e45d3-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="e45d3-141">Device Id.</span></span>|
|<span data-ttu-id="e45d3-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e45d3-142">lastSyncDateTime</span></span>|<span data-ttu-id="e45d3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45d3-143">DateTimeOffset</span></span>|<span data-ttu-id="e45d3-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e45d3-144">Last sync date and time.</span></span>|
|<span data-ttu-id="e45d3-145">installState</span><span class="sxs-lookup"><span data-stu-id="e45d3-145">installState</span></span>|[<span data-ttu-id="e45d3-146">installState</span><span class="sxs-lookup"><span data-stu-id="e45d3-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="e45d3-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e45d3-147">The install state of the eBook.</span></span> <span data-ttu-id="e45d3-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e45d3-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="e45d3-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="e45d3-149">errorCode</span></span>|<span data-ttu-id="e45d3-150">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-150">String</span></span>|<span data-ttu-id="e45d3-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="e45d3-151">The error code for install failures.</span></span>|
|<span data-ttu-id="e45d3-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="e45d3-152">osVersion</span></span>|<span data-ttu-id="e45d3-153">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-153">String</span></span>|<span data-ttu-id="e45d3-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="e45d3-154">OS Version.</span></span>|
|<span data-ttu-id="e45d3-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="e45d3-155">osDescription</span></span>|<span data-ttu-id="e45d3-156">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-156">String</span></span>|<span data-ttu-id="e45d3-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="e45d3-157">OS Description.</span></span>|
|<span data-ttu-id="e45d3-158">userName</span><span class="sxs-lookup"><span data-stu-id="e45d3-158">userName</span></span>|<span data-ttu-id="e45d3-159">String</span><span class="sxs-lookup"><span data-stu-id="e45d3-159">String</span></span>|<span data-ttu-id="e45d3-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="e45d3-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="e45d3-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45d3-161">Response</span></span>
<span data-ttu-id="e45d3-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e45d3-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e45d3-163">Пример</span><span class="sxs-lookup"><span data-stu-id="e45d3-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="e45d3-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e45d3-164">Request</span></span>
<span data-ttu-id="e45d3-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e45d3-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e45d3-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e45d3-166">Response</span></span>
<span data-ttu-id="e45d3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e45d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




