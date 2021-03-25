---
title: Get deviceManagementScriptUserState
description: Чтение свойств и связей объекта deviceManagementScriptUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6762518a2400a13041bccff9ed0f550878cec23e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150341"
---
# <a name="get-devicemanagementscriptuserstate"></a><span data-ttu-id="f64cf-103">Get deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f64cf-103">Get deviceManagementScriptUserState</span></span>

<span data-ttu-id="f64cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f64cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f64cf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f64cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f64cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f64cf-107">Чтение свойств и связей [объекта deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)</span><span class="sxs-lookup"><span data-stu-id="f64cf-107">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f64cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f64cf-108">Prerequisites</span></span>
<span data-ttu-id="f64cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f64cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f64cf-111">Permission type</span></span>|<span data-ttu-id="f64cf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f64cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f64cf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f64cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f64cf-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64cf-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f64cf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f64cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f64cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64cf-116">Not supported.</span></span>|
|<span data-ttu-id="f64cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f64cf-117">Application</span></span>|<span data-ttu-id="f64cf-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64cf-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f64cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f64cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f64cf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f64cf-120">Optional query parameters</span></span>
<span data-ttu-id="f64cf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f64cf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f64cf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f64cf-122">Request headers</span></span>
|<span data-ttu-id="f64cf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f64cf-123">Header</span></span>|<span data-ttu-id="f64cf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f64cf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f64cf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f64cf-125">Authorization</span></span>|<span data-ttu-id="f64cf-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f64cf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f64cf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f64cf-127">Accept</span></span>|<span data-ttu-id="f64cf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f64cf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f64cf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f64cf-129">Request body</span></span>
<span data-ttu-id="f64cf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f64cf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f64cf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f64cf-131">Response</span></span>
<span data-ttu-id="f64cf-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f64cf-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64cf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f64cf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f64cf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f64cf-134">Request</span></span>
<span data-ttu-id="f64cf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f64cf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="f64cf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f64cf-136">Response</span></span>
<span data-ttu-id="f64cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f64cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 258

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
    "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "userPrincipalName": "User Principal Name value"
  }
}
```




