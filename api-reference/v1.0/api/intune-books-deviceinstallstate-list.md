---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13732a4573a05e407c62a2771ff8ebb45a87dc65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757257"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="72e66-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="72e66-103">List deviceInstallStates</span></span>

<span data-ttu-id="72e66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72e66-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72e66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e66-106">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="72e66-106">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72e66-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="72e66-107">Prerequisites</span></span>
<span data-ttu-id="72e66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e66-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72e66-110">Permission type</span></span>|<span data-ttu-id="72e66-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72e66-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72e66-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72e66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72e66-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e66-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72e66-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72e66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72e66-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72e66-115">Not supported.</span></span>|
|<span data-ttu-id="72e66-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="72e66-116">Application</span></span>|<span data-ttu-id="72e66-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72e66-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72e66-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72e66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="72e66-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72e66-119">Request headers</span></span>
|<span data-ttu-id="72e66-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72e66-120">Header</span></span>|<span data-ttu-id="72e66-121">Значение</span><span class="sxs-lookup"><span data-stu-id="72e66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72e66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e66-122">Authorization</span></span>|<span data-ttu-id="72e66-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72e66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72e66-124">Accept</span><span class="sxs-lookup"><span data-stu-id="72e66-124">Accept</span></span>|<span data-ttu-id="72e66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72e66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72e66-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72e66-126">Request body</span></span>
<span data-ttu-id="72e66-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72e66-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72e66-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="72e66-128">Response</span></span>
<span data-ttu-id="72e66-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72e66-129">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72e66-130">Пример</span><span class="sxs-lookup"><span data-stu-id="72e66-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72e66-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72e66-131">Request</span></span>
<span data-ttu-id="72e66-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72e66-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="72e66-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="72e66-133">Response</span></span>
<span data-ttu-id="72e66-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72e66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
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
  ]
}
```




