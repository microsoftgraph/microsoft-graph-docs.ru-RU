---
title: Список Циркуларжеофенцеманажементкондитионс
description: Список свойств и связей объектов Циркуларжеофенцеманажементкондитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99da6ebc0bfbe890ed1b67b676138f0874316255
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201396"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="fe840-103">Список Циркуларжеофенцеманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="fe840-103">List circularGeofenceManagementConditions</span></span>

<span data-ttu-id="fe840-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe840-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe840-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe840-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe840-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe840-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe840-107">Список свойств и связей объектов [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="fe840-107">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe840-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe840-108">Prerequisites</span></span>
<span data-ttu-id="fe840-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe840-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe840-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe840-111">Permission type</span></span>|<span data-ttu-id="fe840-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe840-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe840-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe840-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe840-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe840-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fe840-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe840-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe840-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe840-116">Not supported.</span></span>|
|<span data-ttu-id="fe840-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe840-117">Application</span></span>|<span data-ttu-id="fe840-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe840-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe840-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe840-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="fe840-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe840-120">Request headers</span></span>
|<span data-ttu-id="fe840-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe840-121">Header</span></span>|<span data-ttu-id="fe840-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe840-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe840-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe840-123">Authorization</span></span>|<span data-ttu-id="fe840-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe840-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe840-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe840-125">Accept</span></span>|<span data-ttu-id="fe840-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe840-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe840-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe840-127">Request body</span></span>
<span data-ttu-id="fe840-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe840-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe840-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe840-129">Response</span></span>
<span data-ttu-id="fe840-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe840-130">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe840-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fe840-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe840-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe840-132">Request</span></span>
<span data-ttu-id="fe840-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe840-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="fe840-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe840-134">Response</span></span>
<span data-ttu-id="fe840-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe840-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
      "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "latitude": 2.6666666666666665,
      "longitude": 3.0,
      "radiusInMeters": 4.666666666666667
    }
  ]
}
```




