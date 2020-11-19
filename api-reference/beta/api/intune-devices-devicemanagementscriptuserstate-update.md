---
title: Обновление Девицеманажементскриптусерстате
description: Обновление свойств объекта Девицеманажементскриптусерстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08a557b4dbe1b1e83d333eecc049ea644a1d870e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228668"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="88e85-103">Обновление Девицеманажементскриптусерстате</span><span class="sxs-lookup"><span data-stu-id="88e85-103">Update deviceManagementScriptUserState</span></span>

<span data-ttu-id="88e85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88e85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88e85-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88e85-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88e85-107">Обновление свойств объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="88e85-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88e85-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88e85-108">Prerequisites</span></span>
<span data-ttu-id="88e85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e85-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88e85-111">Permission type</span></span>|<span data-ttu-id="88e85-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88e85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88e85-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88e85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88e85-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e85-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88e85-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88e85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88e85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e85-116">Not supported.</span></span>|
|<span data-ttu-id="88e85-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="88e85-117">Application</span></span>|<span data-ttu-id="88e85-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e85-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88e85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88e85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88e85-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88e85-120">Request headers</span></span>
|<span data-ttu-id="88e85-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88e85-121">Header</span></span>|<span data-ttu-id="88e85-122">Значение</span><span class="sxs-lookup"><span data-stu-id="88e85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88e85-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88e85-123">Authorization</span></span>|<span data-ttu-id="88e85-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88e85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88e85-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88e85-125">Accept</span></span>|<span data-ttu-id="88e85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88e85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88e85-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88e85-127">Request body</span></span>
<span data-ttu-id="88e85-128">В тексте запроса добавьте представление объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88e85-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="88e85-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="88e85-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="88e85-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="88e85-130">Property</span></span>|<span data-ttu-id="88e85-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88e85-131">Type</span></span>|<span data-ttu-id="88e85-132">Описание</span><span class="sxs-lookup"><span data-stu-id="88e85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88e85-133">id</span><span class="sxs-lookup"><span data-stu-id="88e85-133">id</span></span>|<span data-ttu-id="88e85-134">String</span><span class="sxs-lookup"><span data-stu-id="88e85-134">String</span></span>|<span data-ttu-id="88e85-135">Ключ объекта состояния пользователя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="88e85-135">Key of the device management script user state entity.</span></span> <span data-ttu-id="88e85-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88e85-136">This property is read-only.</span></span>|
|<span data-ttu-id="88e85-137">сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="88e85-137">successDeviceCount</span></span>|<span data-ttu-id="88e85-138">Int32</span><span class="sxs-lookup"><span data-stu-id="88e85-138">Int32</span></span>|<span data-ttu-id="88e85-139">Число устройств для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="88e85-139">Success device count for specific user.</span></span>|
|<span data-ttu-id="88e85-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88e85-140">errorDeviceCount</span></span>|<span data-ttu-id="88e85-141">Int32</span><span class="sxs-lookup"><span data-stu-id="88e85-141">Int32</span></span>|<span data-ttu-id="88e85-142">Количество устройств с ошибками для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="88e85-142">Error device count for specific user.</span></span>|
|<span data-ttu-id="88e85-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88e85-143">userPrincipalName</span></span>|<span data-ttu-id="88e85-144">String</span><span class="sxs-lookup"><span data-stu-id="88e85-144">String</span></span>|<span data-ttu-id="88e85-145">Имя участника, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="88e85-145">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="88e85-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="88e85-146">Response</span></span>
<span data-ttu-id="88e85-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88e85-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e85-148">Пример</span><span class="sxs-lookup"><span data-stu-id="88e85-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="88e85-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="88e85-149">Request</span></span>
<span data-ttu-id="88e85-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88e85-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="88e85-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="88e85-151">Response</span></span>
<span data-ttu-id="88e85-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88e85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




