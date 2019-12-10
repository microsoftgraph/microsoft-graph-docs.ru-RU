---
title: Получение Циркуларжеофенцеманажементкондитион
description: Чтение свойств и связей объекта Циркуларжеофенцеманажементкондитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fd7981c7a01c8a3c459c0742ec9ae2335531ed8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943511"
---
# <a name="get-circulargeofencemanagementcondition"></a><span data-ttu-id="6c6d4-103">Получение Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="6c6d4-103">Get circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="6c6d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c6d4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c6d4-106">Чтение свойств и связей объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="6c6d4-106">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c6d4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c6d4-107">Prerequisites</span></span>
<span data-ttu-id="6c6d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c6d4-110">Permission type</span></span>|<span data-ttu-id="6c6d4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c6d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c6d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c6d4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c6d4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c6d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c6d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-115">Not supported.</span></span>|
|<span data-ttu-id="6c6d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c6d4-116">Application</span></span>|<span data-ttu-id="6c6d4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c6d4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c6d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c6d4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c6d4-119">Optional query parameters</span></span>
<span data-ttu-id="6c6d4-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c6d4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c6d4-121">Request headers</span></span>
|<span data-ttu-id="6c6d4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c6d4-122">Header</span></span>|<span data-ttu-id="6c6d4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6c6d4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c6d4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c6d4-124">Authorization</span></span>|<span data-ttu-id="6c6d4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c6d4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6c6d4-126">Accept</span></span>|<span data-ttu-id="6c6d4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c6d4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6d4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c6d4-128">Request body</span></span>
<span data-ttu-id="6c6d4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c6d4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c6d4-130">Response</span></span>
<span data-ttu-id="6c6d4-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-131">If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6d4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6c6d4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c6d4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c6d4-133">Request</span></span>
<span data-ttu-id="6c6d4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="6c6d4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6d4-135">Response</span></span>
<span data-ttu-id="6c6d4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c6d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

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
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
  }
}
```





