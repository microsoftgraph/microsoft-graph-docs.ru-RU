---
title: Get circularGeofenceManagementCondition
description: Чтение свойств и связей объекта circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23ffc010c611e80df71e6e78303cb46cc1556d11
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157549"
---
# <a name="get-circulargeofencemanagementcondition"></a><span data-ttu-id="4ef56-103">Get circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="4ef56-103">Get circularGeofenceManagementCondition</span></span>

<span data-ttu-id="4ef56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef56-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ef56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef56-107">Чтение свойств и связей объекта [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4ef56-107">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ef56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ef56-108">Prerequisites</span></span>
<span data-ttu-id="4ef56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ef56-111">Permission type</span></span>|<span data-ttu-id="4ef56-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ef56-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ef56-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ef56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ef56-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef56-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ef56-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ef56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ef56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef56-116">Not supported.</span></span>|
|<span data-ttu-id="4ef56-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ef56-117">Application</span></span>|<span data-ttu-id="4ef56-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef56-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ef56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ef56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ef56-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ef56-120">Optional query parameters</span></span>
<span data-ttu-id="4ef56-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ef56-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ef56-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ef56-122">Request headers</span></span>
|<span data-ttu-id="4ef56-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ef56-123">Header</span></span>|<span data-ttu-id="4ef56-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4ef56-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ef56-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef56-125">Authorization</span></span>|<span data-ttu-id="4ef56-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef56-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ef56-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4ef56-127">Accept</span></span>|<span data-ttu-id="4ef56-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4ef56-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef56-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ef56-129">Request body</span></span>
<span data-ttu-id="4ef56-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ef56-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ef56-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef56-131">Response</span></span>
<span data-ttu-id="4ef56-132">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ef56-132">If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef56-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ef56-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ef56-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ef56-134">Request</span></span>
<span data-ttu-id="4ef56-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ef56-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="4ef56-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef56-136">Response</span></span>
<span data-ttu-id="4ef56-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ef56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 586

{
  "value": {
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
}
```




