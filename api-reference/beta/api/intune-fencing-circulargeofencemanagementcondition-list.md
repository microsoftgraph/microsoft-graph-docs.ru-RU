---
title: Список Циркуларжеофенцеманажементкондитионс
description: Список свойств и связей объектов Циркуларжеофенцеманажементкондитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14ab47410658484fda0898f74534ff0ae29fe009
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453971"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="4ae13-103">Список Циркуларжеофенцеманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="4ae13-103">List circularGeofenceManagementConditions</span></span>

<span data-ttu-id="4ae13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ae13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ae13-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ae13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ae13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ae13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ae13-107">Список свойств и связей объектов [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="4ae13-107">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ae13-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ae13-108">Prerequisites</span></span>
<span data-ttu-id="4ae13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ae13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae13-111">Permission type</span></span>|<span data-ttu-id="4ae13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ae13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ae13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ae13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ae13-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ae13-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ae13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ae13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ae13-116">Not supported.</span></span>|
|<span data-ttu-id="4ae13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ae13-117">Application</span></span>|<span data-ttu-id="4ae13-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ae13-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ae13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4ae13-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ae13-120">Request headers</span></span>
|<span data-ttu-id="4ae13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ae13-121">Header</span></span>|<span data-ttu-id="4ae13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ae13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ae13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae13-123">Authorization</span></span>|<span data-ttu-id="4ae13-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ae13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ae13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ae13-125">Accept</span></span>|<span data-ttu-id="4ae13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ae13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae13-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ae13-127">Request body</span></span>
<span data-ttu-id="4ae13-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ae13-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ae13-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ae13-129">Response</span></span>
<span data-ttu-id="4ae13-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae13-130">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae13-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4ae13-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ae13-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ae13-132">Request</span></span>
<span data-ttu-id="4ae13-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ae13-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="4ae13-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae13-134">Response</span></span>
<span data-ttu-id="4ae13-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ae13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

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
      "latitude": "<Unknown Primitive Type Edm.Double>",
      "longitude": "<Unknown Primitive Type Edm.Double>",
      "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
    }
  ]
}
```



