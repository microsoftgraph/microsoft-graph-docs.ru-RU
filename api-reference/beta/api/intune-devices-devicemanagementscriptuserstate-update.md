---
title: Обновление deviceManagementScriptUserState
description: Обновление свойств объекта deviceManagementScriptUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5b36ac8f035cf9d4b204a40dfe749f57a004643
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150320"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="53630-103">Обновление deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="53630-103">Update deviceManagementScriptUserState</span></span>

<span data-ttu-id="53630-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53630-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53630-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53630-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53630-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53630-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53630-107">Обновление свойств объекта [deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="53630-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53630-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53630-108">Prerequisites</span></span>
<span data-ttu-id="53630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53630-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53630-111">Permission type</span></span>|<span data-ttu-id="53630-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53630-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53630-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53630-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53630-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53630-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53630-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53630-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53630-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53630-116">Not supported.</span></span>|
|<span data-ttu-id="53630-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="53630-117">Application</span></span>|<span data-ttu-id="53630-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53630-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53630-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53630-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="53630-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53630-120">Request headers</span></span>
|<span data-ttu-id="53630-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53630-121">Header</span></span>|<span data-ttu-id="53630-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53630-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53630-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53630-123">Authorization</span></span>|<span data-ttu-id="53630-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53630-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53630-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53630-125">Accept</span></span>|<span data-ttu-id="53630-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53630-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53630-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53630-127">Request body</span></span>
<span data-ttu-id="53630-128">В теле запроса укажи представление JSON для [объекта deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="53630-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="53630-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="53630-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="53630-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53630-130">Property</span></span>|<span data-ttu-id="53630-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53630-131">Type</span></span>|<span data-ttu-id="53630-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53630-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53630-133">id</span><span class="sxs-lookup"><span data-stu-id="53630-133">id</span></span>|<span data-ttu-id="53630-134">Строка</span><span class="sxs-lookup"><span data-stu-id="53630-134">String</span></span>|<span data-ttu-id="53630-135">Ключ пользовательского состояния скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="53630-135">Key of the device management script user state entity.</span></span> <span data-ttu-id="53630-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53630-136">This property is read-only.</span></span>|
|<span data-ttu-id="53630-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53630-137">successDeviceCount</span></span>|<span data-ttu-id="53630-138">Int32</span><span class="sxs-lookup"><span data-stu-id="53630-138">Int32</span></span>|<span data-ttu-id="53630-139">Количество устройств успешности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="53630-139">Success device count for specific user.</span></span>|
|<span data-ttu-id="53630-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53630-140">errorDeviceCount</span></span>|<span data-ttu-id="53630-141">Int32</span><span class="sxs-lookup"><span data-stu-id="53630-141">Int32</span></span>|<span data-ttu-id="53630-142">Количество устройств ошибки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="53630-142">Error device count for specific user.</span></span>|
|<span data-ttu-id="53630-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53630-143">userPrincipalName</span></span>|<span data-ttu-id="53630-144">String</span><span class="sxs-lookup"><span data-stu-id="53630-144">String</span></span>|<span data-ttu-id="53630-145">Имя принципа пользователя конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="53630-145">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="53630-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="53630-146">Response</span></span>
<span data-ttu-id="53630-147">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="53630-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53630-148">Пример</span><span class="sxs-lookup"><span data-stu-id="53630-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="53630-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="53630-149">Request</span></span>
<span data-ttu-id="53630-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53630-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53630-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="53630-151">Response</span></span>
<span data-ttu-id="53630-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53630-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




