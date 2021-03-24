---
title: Перечисление объектов deviceInstallState
description: Список свойств и связей объектов deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd0e953d98b591876f4e1ac060ac5eaad56dfa5b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133691"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="ad4dd-103">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ad4dd-103">List deviceInstallStates</span></span>

<span data-ttu-id="ad4dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad4dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad4dd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad4dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad4dd-107">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="ad4dd-107">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad4dd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad4dd-108">Prerequisites</span></span>
<span data-ttu-id="ad4dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad4dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad4dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad4dd-111">Permission type</span></span>|<span data-ttu-id="ad4dd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad4dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad4dd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad4dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad4dd-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4dd-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad4dd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad4dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad4dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-116">Not supported.</span></span>|
|<span data-ttu-id="ad4dd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad4dd-117">Application</span></span>|<span data-ttu-id="ad4dd-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4dd-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad4dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad4dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="ad4dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad4dd-120">Request headers</span></span>
|<span data-ttu-id="ad4dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad4dd-121">Header</span></span>|<span data-ttu-id="ad4dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad4dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad4dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4dd-123">Authorization</span></span>|<span data-ttu-id="ad4dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad4dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad4dd-125">Accept</span></span>|<span data-ttu-id="ad4dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad4dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad4dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad4dd-127">Request body</span></span>
<span data-ttu-id="ad4dd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad4dd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad4dd-129">Response</span></span>
<span data-ttu-id="ad4dd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-130">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad4dd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad4dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad4dd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad4dd-132">Request</span></span>
<span data-ttu-id="ad4dd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="ad4dd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad4dd-134">Response</span></span>
<span data-ttu-id="ad4dd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad4dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




