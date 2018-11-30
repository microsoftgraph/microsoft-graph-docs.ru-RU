---
title: Обновление объекта deviceInstallState
description: Обновление свойств объекта deviceInstallState.
ms.openlocfilehash: bef58a3497a49fd027d67594ae8d8bcd26342d3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081190"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="0cbcf-103">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="0cbcf-103">Update deviceInstallState</span></span>

> <span data-ttu-id="0cbcf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cbcf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cbcf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cbcf-107">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="0cbcf-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cbcf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0cbcf-108">Prerequisites</span></span>
<span data-ttu-id="0cbcf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cbcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cbcf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cbcf-111">Permission type</span></span>|<span data-ttu-id="0cbcf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cbcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cbcf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cbcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cbcf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cbcf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0cbcf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cbcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cbcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-116">Not supported.</span></span>|
|<span data-ttu-id="0cbcf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cbcf-117">Application</span></span>|<span data-ttu-id="0cbcf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cbcf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cbcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0cbcf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cbcf-120">Request headers</span></span>
|<span data-ttu-id="0cbcf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cbcf-121">Header</span></span>|<span data-ttu-id="0cbcf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0cbcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cbcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cbcf-123">Authorization</span></span>|<span data-ttu-id="0cbcf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0cbcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cbcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cbcf-125">Accept</span></span>|<span data-ttu-id="0cbcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cbcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cbcf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cbcf-127">Request body</span></span>
<span data-ttu-id="0cbcf-128">В тексте запроса добавьте представление объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="0cbcf-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="0cbcf-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="0cbcf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cbcf-130">Property</span></span>|<span data-ttu-id="0cbcf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0cbcf-131">Type</span></span>|<span data-ttu-id="0cbcf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0cbcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cbcf-133">id</span><span class="sxs-lookup"><span data-stu-id="0cbcf-133">id</span></span>|<span data-ttu-id="0cbcf-134">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-134">String</span></span>|<span data-ttu-id="0cbcf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-135">Key of the entity.</span></span>|
|<span data-ttu-id="0cbcf-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0cbcf-136">deviceName</span></span>|<span data-ttu-id="0cbcf-137">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-137">String</span></span>|<span data-ttu-id="0cbcf-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-138">Device name.</span></span>|
|<span data-ttu-id="0cbcf-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0cbcf-139">deviceId</span></span>|<span data-ttu-id="0cbcf-140">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-140">String</span></span>|<span data-ttu-id="0cbcf-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-141">Device Id.</span></span>|
|<span data-ttu-id="0cbcf-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0cbcf-142">lastSyncDateTime</span></span>|<span data-ttu-id="0cbcf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cbcf-143">DateTimeOffset</span></span>|<span data-ttu-id="0cbcf-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-144">Last sync date and time.</span></span>|
|<span data-ttu-id="0cbcf-145">installState</span><span class="sxs-lookup"><span data-stu-id="0cbcf-145">installState</span></span>|[<span data-ttu-id="0cbcf-146">installState</span><span class="sxs-lookup"><span data-stu-id="0cbcf-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="0cbcf-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-147">The install state of the eBook.</span></span> <span data-ttu-id="0cbcf-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="0cbcf-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="0cbcf-149">errorCode</span></span>|<span data-ttu-id="0cbcf-150">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-150">String</span></span>|<span data-ttu-id="0cbcf-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-151">The error code for install failures.</span></span>|
|<span data-ttu-id="0cbcf-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="0cbcf-152">osVersion</span></span>|<span data-ttu-id="0cbcf-153">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-153">String</span></span>|<span data-ttu-id="0cbcf-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-154">OS Version.</span></span>|
|<span data-ttu-id="0cbcf-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="0cbcf-155">osDescription</span></span>|<span data-ttu-id="0cbcf-156">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-156">String</span></span>|<span data-ttu-id="0cbcf-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-157">OS Description.</span></span>|
|<span data-ttu-id="0cbcf-158">userName</span><span class="sxs-lookup"><span data-stu-id="0cbcf-158">userName</span></span>|<span data-ttu-id="0cbcf-159">String</span><span class="sxs-lookup"><span data-stu-id="0cbcf-159">String</span></span>|<span data-ttu-id="0cbcf-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0cbcf-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cbcf-161">Response</span></span>
<span data-ttu-id="0cbcf-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cbcf-163">Пример</span><span class="sxs-lookup"><span data-stu-id="0cbcf-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cbcf-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cbcf-164">Request</span></span>
<span data-ttu-id="0cbcf-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cbcf-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
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

### <a name="response"></a><span data-ttu-id="0cbcf-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cbcf-166">Response</span></span>
<span data-ttu-id="0cbcf-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0cbcf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





