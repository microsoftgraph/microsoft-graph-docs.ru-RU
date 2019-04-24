---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16af56e2bf82b5e15d259229ae9a2416fa20e92c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32484040"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="c68b4-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="c68b4-103">Create deviceInstallState</span></span>

> <span data-ttu-id="c68b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c68b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c68b4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c68b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c68b4-106">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="c68b4-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c68b4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c68b4-107">Prerequisites</span></span>
<span data-ttu-id="c68b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c68b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c68b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c68b4-110">Permission type</span></span>|<span data-ttu-id="c68b4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c68b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c68b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c68b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c68b4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68b4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c68b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c68b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c68b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c68b4-115">Not supported.</span></span>|
|<span data-ttu-id="c68b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c68b4-116">Application</span></span>|<span data-ttu-id="c68b4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c68b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c68b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c68b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c68b4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c68b4-119">Request headers</span></span>
|<span data-ttu-id="c68b4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c68b4-120">Header</span></span>|<span data-ttu-id="c68b4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c68b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c68b4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c68b4-122">Authorization</span></span>|<span data-ttu-id="c68b4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c68b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c68b4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c68b4-124">Accept</span></span>|<span data-ttu-id="c68b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c68b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c68b4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c68b4-126">Request body</span></span>
<span data-ttu-id="c68b4-127">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c68b4-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="c68b4-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="c68b4-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="c68b4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c68b4-129">Property</span></span>|<span data-ttu-id="c68b4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c68b4-130">Type</span></span>|<span data-ttu-id="c68b4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c68b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c68b4-132">id</span><span class="sxs-lookup"><span data-stu-id="c68b4-132">id</span></span>|<span data-ttu-id="c68b4-133">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-133">String</span></span>|<span data-ttu-id="c68b4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c68b4-134">Key of the entity.</span></span>|
|<span data-ttu-id="c68b4-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="c68b4-135">deviceName</span></span>|<span data-ttu-id="c68b4-136">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-136">String</span></span>|<span data-ttu-id="c68b4-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="c68b4-137">Device name.</span></span>|
|<span data-ttu-id="c68b4-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="c68b4-138">deviceId</span></span>|<span data-ttu-id="c68b4-139">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-139">String</span></span>|<span data-ttu-id="c68b4-140">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c68b4-140">Device Id.</span></span>|
|<span data-ttu-id="c68b4-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c68b4-141">lastSyncDateTime</span></span>|<span data-ttu-id="c68b4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c68b4-142">DateTimeOffset</span></span>|<span data-ttu-id="c68b4-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c68b4-143">Last sync date and time.</span></span>|
|<span data-ttu-id="c68b4-144">installState</span><span class="sxs-lookup"><span data-stu-id="c68b4-144">installState</span></span>|[<span data-ttu-id="c68b4-145">installState</span><span class="sxs-lookup"><span data-stu-id="c68b4-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="c68b4-146">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c68b4-146">The install state of the eBook.</span></span> <span data-ttu-id="c68b4-147">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c68b4-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="c68b4-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="c68b4-148">errorCode</span></span>|<span data-ttu-id="c68b4-149">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-149">String</span></span>|<span data-ttu-id="c68b4-150">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="c68b4-150">The error code for install failures.</span></span>|
|<span data-ttu-id="c68b4-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="c68b4-151">osVersion</span></span>|<span data-ttu-id="c68b4-152">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-152">String</span></span>|<span data-ttu-id="c68b4-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="c68b4-153">OS Version.</span></span>|
|<span data-ttu-id="c68b4-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="c68b4-154">osDescription</span></span>|<span data-ttu-id="c68b4-155">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-155">String</span></span>|<span data-ttu-id="c68b4-156">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="c68b4-156">OS Description.</span></span>|
|<span data-ttu-id="c68b4-157">userName</span><span class="sxs-lookup"><span data-stu-id="c68b4-157">userName</span></span>|<span data-ttu-id="c68b4-158">String</span><span class="sxs-lookup"><span data-stu-id="c68b4-158">String</span></span>|<span data-ttu-id="c68b4-159">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="c68b4-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="c68b4-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c68b4-160">Response</span></span>
<span data-ttu-id="c68b4-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c68b4-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c68b4-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c68b4-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c68b4-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c68b4-163">Request</span></span>
<span data-ttu-id="c68b4-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c68b4-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c68b4-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c68b4-165">Response</span></span>
<span data-ttu-id="c68b4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c68b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





