---
title: Получение Девицеманажементскриптусерстате
description: Чтение свойств и связей объекта Девицеманажементскриптусерстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9107ba0e966c8a19341d964f1c41ba332fca28e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155589"
---
# <a name="get-devicemanagementscriptuserstate"></a><span data-ttu-id="4ed56-103">Получение Девицеманажементскриптусерстате</span><span class="sxs-lookup"><span data-stu-id="4ed56-103">Get deviceManagementScriptUserState</span></span>

> <span data-ttu-id="4ed56-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed56-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ed56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed56-106">Чтение свойств и связей объекта [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="4ed56-106">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ed56-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ed56-107">Prerequisites</span></span>
<span data-ttu-id="4ed56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ed56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4ed56-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ed56-110">Permission type</span></span>|<span data-ttu-id="4ed56-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ed56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed56-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ed56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed56-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ed56-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4ed56-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ed56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed56-115">Not supported.</span></span>|
|<span data-ttu-id="4ed56-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ed56-116">Application</span></span>|<span data-ttu-id="4ed56-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed56-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ed56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ed56-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ed56-119">Optional query parameters</span></span>
<span data-ttu-id="4ed56-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ed56-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ed56-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ed56-121">Request headers</span></span>
|<span data-ttu-id="4ed56-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ed56-122">Header</span></span>|<span data-ttu-id="4ed56-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4ed56-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed56-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ed56-124">Authorization</span></span>|<span data-ttu-id="4ed56-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4ed56-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed56-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4ed56-126">Accept</span></span>|<span data-ttu-id="4ed56-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed56-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed56-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ed56-128">Request body</span></span>
<span data-ttu-id="4ed56-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ed56-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ed56-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ed56-130">Response</span></span>
<span data-ttu-id="4ed56-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ed56-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed56-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4ed56-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ed56-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ed56-133">Request</span></span>
<span data-ttu-id="4ed56-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ed56-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="4ed56-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ed56-135">Response</span></span>
<span data-ttu-id="4ed56-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ed56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




