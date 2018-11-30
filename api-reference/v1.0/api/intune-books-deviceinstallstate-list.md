---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
ms.openlocfilehash: 609686153c42f04b56fd2226b56d7edad7b6cb79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027764"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="5b656-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="5b656-103">List deviceInstallStates</span></span>

> <span data-ttu-id="5b656-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5b656-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b656-105">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="5b656-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b656-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b656-106">Prerequisites</span></span>
<span data-ttu-id="5b656-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b656-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b656-109">Permission type</span></span>|<span data-ttu-id="5b656-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b656-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b656-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b656-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b656-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b656-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b656-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b656-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b656-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b656-114">Not supported.</span></span>|
|<span data-ttu-id="5b656-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b656-115">Application</span></span>|<span data-ttu-id="5b656-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b656-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b656-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b656-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="5b656-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b656-118">Request headers</span></span>
|<span data-ttu-id="5b656-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b656-119">Header</span></span>|<span data-ttu-id="5b656-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5b656-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b656-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b656-121">Authorization</span></span>|<span data-ttu-id="5b656-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b656-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b656-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b656-123">Accept</span></span>|<span data-ttu-id="5b656-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b656-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b656-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b656-125">Request body</span></span>
<span data-ttu-id="5b656-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b656-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b656-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b656-127">Response</span></span>
<span data-ttu-id="5b656-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b656-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b656-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5b656-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b656-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b656-130">Request</span></span>
<span data-ttu-id="5b656-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b656-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="5b656-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b656-132">Response</span></span>
<span data-ttu-id="5b656-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5b656-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



