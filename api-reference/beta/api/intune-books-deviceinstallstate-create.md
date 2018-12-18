---
title: Создание объекта deviceInstallState
description: Создание объекта deviceInstallState.
author: tfitzmac
ms.openlocfilehash: 9f058dd32ca8f20864f5c7e143887b5191a7be8d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352418"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="3fb03-103">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3fb03-103">Create deviceInstallState</span></span>

> <span data-ttu-id="3fb03-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3fb03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fb03-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fb03-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3fb03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fb03-107">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="3fb03-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fb03-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3fb03-108">Prerequisites</span></span>
<span data-ttu-id="3fb03-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fb03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fb03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fb03-111">Permission type</span></span>|<span data-ttu-id="3fb03-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fb03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fb03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb03-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fb03-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3fb03-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fb03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb03-116">Not supported.</span></span>|
|<span data-ttu-id="3fb03-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fb03-117">Application</span></span>|<span data-ttu-id="3fb03-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb03-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fb03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="3fb03-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fb03-120">Request headers</span></span>
|<span data-ttu-id="3fb03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fb03-121">Header</span></span>|<span data-ttu-id="3fb03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3fb03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb03-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fb03-123">Authorization</span></span>|<span data-ttu-id="3fb03-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3fb03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb03-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fb03-125">Accept</span></span>|<span data-ttu-id="3fb03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fb03-127">Request body</span></span>
<span data-ttu-id="3fb03-128">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fb03-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="3fb03-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="3fb03-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="3fb03-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fb03-130">Property</span></span>|<span data-ttu-id="3fb03-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3fb03-131">Type</span></span>|<span data-ttu-id="3fb03-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3fb03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb03-133">id</span><span class="sxs-lookup"><span data-stu-id="3fb03-133">id</span></span>|<span data-ttu-id="3fb03-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3fb03-134">String</span></span>|<span data-ttu-id="3fb03-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3fb03-135">Key of the entity.</span></span>|
|<span data-ttu-id="3fb03-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="3fb03-136">deviceName</span></span>|<span data-ttu-id="3fb03-137">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-137">String</span></span>|<span data-ttu-id="3fb03-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="3fb03-138">Device name.</span></span>|
|<span data-ttu-id="3fb03-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="3fb03-139">deviceId</span></span>|<span data-ttu-id="3fb03-140">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-140">String</span></span>|<span data-ttu-id="3fb03-141">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="3fb03-141">Device Id.</span></span>|
|<span data-ttu-id="3fb03-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb03-142">lastSyncDateTime</span></span>|<span data-ttu-id="3fb03-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb03-143">DateTimeOffset</span></span>|<span data-ttu-id="3fb03-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3fb03-144">Last sync date and time.</span></span>|
|<span data-ttu-id="3fb03-145">installState</span><span class="sxs-lookup"><span data-stu-id="3fb03-145">installState</span></span>|[<span data-ttu-id="3fb03-146">installState</span><span class="sxs-lookup"><span data-stu-id="3fb03-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="3fb03-147">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3fb03-147">The install state of the eBook.</span></span> <span data-ttu-id="3fb03-148">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3fb03-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="3fb03-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="3fb03-149">errorCode</span></span>|<span data-ttu-id="3fb03-150">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-150">String</span></span>|<span data-ttu-id="3fb03-151">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="3fb03-151">The error code for install failures.</span></span>|
|<span data-ttu-id="3fb03-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="3fb03-152">osVersion</span></span>|<span data-ttu-id="3fb03-153">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-153">String</span></span>|<span data-ttu-id="3fb03-154">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="3fb03-154">OS Version.</span></span>|
|<span data-ttu-id="3fb03-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="3fb03-155">osDescription</span></span>|<span data-ttu-id="3fb03-156">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-156">String</span></span>|<span data-ttu-id="3fb03-157">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="3fb03-157">OS Description.</span></span>|
|<span data-ttu-id="3fb03-158">userName</span><span class="sxs-lookup"><span data-stu-id="3fb03-158">userName</span></span>|<span data-ttu-id="3fb03-159">String</span><span class="sxs-lookup"><span data-stu-id="3fb03-159">String</span></span>|<span data-ttu-id="3fb03-160">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="3fb03-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="3fb03-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fb03-161">Response</span></span>
<span data-ttu-id="3fb03-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fb03-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb03-163">Пример</span><span class="sxs-lookup"><span data-stu-id="3fb03-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fb03-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fb03-164">Request</span></span>
<span data-ttu-id="3fb03-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fb03-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fb03-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fb03-166">Response</span></span>
<span data-ttu-id="3fb03-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3fb03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





