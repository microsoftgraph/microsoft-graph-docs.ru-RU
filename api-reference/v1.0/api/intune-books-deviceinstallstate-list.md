---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 122af650573b3a8b29ddf91e4859e5ce6b487c53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570557"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="b1310-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b1310-103">List deviceInstallStates</span></span>

> <span data-ttu-id="b1310-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1310-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1310-105">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="b1310-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1310-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1310-106">Prerequisites</span></span>
<span data-ttu-id="b1310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1310-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1310-109">Permission type</span></span>|<span data-ttu-id="b1310-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1310-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1310-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1310-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1310-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1310-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b1310-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1310-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1310-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1310-114">Not supported.</span></span>|
|<span data-ttu-id="b1310-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1310-115">Application</span></span>|<span data-ttu-id="b1310-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1310-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1310-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1310-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="b1310-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1310-118">Request headers</span></span>
|<span data-ttu-id="b1310-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1310-119">Header</span></span>|<span data-ttu-id="b1310-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b1310-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1310-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1310-121">Authorization</span></span>|<span data-ttu-id="b1310-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1310-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1310-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b1310-123">Accept</span></span>|<span data-ttu-id="b1310-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1310-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1310-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1310-125">Request body</span></span>
<span data-ttu-id="b1310-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1310-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1310-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1310-127">Response</span></span>
<span data-ttu-id="b1310-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1310-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1310-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b1310-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1310-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1310-130">Request</span></span>
<span data-ttu-id="b1310-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1310-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="b1310-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1310-132">Response</span></span>
<span data-ttu-id="b1310-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



