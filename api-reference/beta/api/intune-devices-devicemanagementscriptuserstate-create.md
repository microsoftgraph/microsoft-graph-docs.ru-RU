---
title: Создание Девицеманажементскриптусерстате
description: Создание нового объекта Девицеманажементскриптусерстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99237e256a181e58b8a4949f973e5f77aa1a9503
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530274"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="d3579-103">Создание Девицеманажементскриптусерстате</span><span class="sxs-lookup"><span data-stu-id="d3579-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="d3579-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3579-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3579-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3579-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3579-106">Создание нового объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="d3579-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3579-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3579-107">Prerequisites</span></span>
<span data-ttu-id="d3579-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3579-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3579-110">Permission type</span></span>|<span data-ttu-id="d3579-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3579-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3579-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3579-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3579-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3579-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3579-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3579-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3579-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3579-115">Not supported.</span></span>|
|<span data-ttu-id="d3579-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3579-116">Application</span></span>|<span data-ttu-id="d3579-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3579-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3579-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3579-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="d3579-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3579-119">Request headers</span></span>
|<span data-ttu-id="d3579-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3579-120">Header</span></span>|<span data-ttu-id="d3579-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d3579-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3579-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3579-122">Authorization</span></span>|<span data-ttu-id="d3579-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3579-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3579-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d3579-124">Accept</span></span>|<span data-ttu-id="d3579-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3579-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3579-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3579-126">Request body</span></span>
<span data-ttu-id="d3579-127">В тексте запроса добавьте представление объекта Девицеманажементскриптусерстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3579-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="d3579-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптусерстате.</span><span class="sxs-lookup"><span data-stu-id="d3579-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="d3579-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3579-129">Property</span></span>|<span data-ttu-id="d3579-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d3579-130">Type</span></span>|<span data-ttu-id="d3579-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d3579-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3579-132">id</span><span class="sxs-lookup"><span data-stu-id="d3579-132">id</span></span>|<span data-ttu-id="d3579-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d3579-133">String</span></span>|<span data-ttu-id="d3579-134">Ключ объекта состояния пользователя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d3579-134">Key of the device management script user state entity.</span></span> <span data-ttu-id="d3579-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3579-135">This property is read-only.</span></span>|
|<span data-ttu-id="d3579-136">сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="d3579-136">successDeviceCount</span></span>|<span data-ttu-id="d3579-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d3579-137">Int32</span></span>|<span data-ttu-id="d3579-138">Число устройств для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3579-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="d3579-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3579-139">errorDeviceCount</span></span>|<span data-ttu-id="d3579-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3579-140">Int32</span></span>|<span data-ttu-id="d3579-141">Количество устройств с ошибками для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3579-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="d3579-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3579-142">userPrincipalName</span></span>|<span data-ttu-id="d3579-143">String</span><span class="sxs-lookup"><span data-stu-id="d3579-143">String</span></span>|<span data-ttu-id="d3579-144">Имя участника, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="d3579-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="d3579-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3579-145">Response</span></span>
<span data-ttu-id="d3579-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3579-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3579-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d3579-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3579-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3579-148">Request</span></span>
<span data-ttu-id="d3579-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3579-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d3579-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3579-150">Response</span></span>
<span data-ttu-id="d3579-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3579-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```






