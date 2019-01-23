---
title: Get deviceInstallState
description: Чтение свойств и связей объекта deviceInstallState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b584e2e168727b13608f3bac8920db389cfac09
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424471"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="77835-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="77835-103">Get deviceInstallState</span></span>

> <span data-ttu-id="77835-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77835-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77835-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77835-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77835-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77835-107">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="77835-107">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77835-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="77835-108">Prerequisites</span></span>
<span data-ttu-id="77835-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77835-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77835-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77835-111">Permission type</span></span>|<span data-ttu-id="77835-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77835-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77835-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77835-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77835-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77835-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77835-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77835-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77835-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77835-116">Not supported.</span></span>|
|<span data-ttu-id="77835-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77835-117">Application</span></span>|<span data-ttu-id="77835-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77835-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77835-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77835-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77835-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77835-120">Optional query parameters</span></span>
<span data-ttu-id="77835-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77835-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77835-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77835-122">Request headers</span></span>
|<span data-ttu-id="77835-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77835-123">Header</span></span>|<span data-ttu-id="77835-124">Значение</span><span class="sxs-lookup"><span data-stu-id="77835-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77835-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77835-125">Authorization</span></span>|<span data-ttu-id="77835-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77835-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77835-127">Accept</span><span class="sxs-lookup"><span data-stu-id="77835-127">Accept</span></span>|<span data-ttu-id="77835-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77835-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77835-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77835-129">Request body</span></span>
<span data-ttu-id="77835-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77835-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77835-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="77835-131">Response</span></span>
<span data-ttu-id="77835-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77835-132">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77835-133">Пример</span><span class="sxs-lookup"><span data-stu-id="77835-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="77835-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="77835-134">Request</span></span>
<span data-ttu-id="77835-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77835-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="77835-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77835-136">Response</span></span>
<span data-ttu-id="77835-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="77835-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": {
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
}
```




