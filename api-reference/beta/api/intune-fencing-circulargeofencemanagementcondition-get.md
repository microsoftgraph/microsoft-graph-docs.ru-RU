---
title: Получение circularGeofenceManagementCondition
description: Чтение свойства и связи объекта circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c070e2f0fab9c215e8f50ce23cab75059037595a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816809"
---
# <a name="get-circulargeofencemanagementcondition"></a><span data-ttu-id="cdcaf-103">Получение circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cdcaf-103">Get circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="cdcaf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdcaf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdcaf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdcaf-107">Чтение свойства и связи объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cdcaf-107">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdcaf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cdcaf-108">Prerequisites</span></span>
<span data-ttu-id="cdcaf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdcaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcaf-111">Permission type</span></span>|<span data-ttu-id="cdcaf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdcaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdcaf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdcaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdcaf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdcaf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cdcaf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdcaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdcaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-116">Not supported.</span></span>|
|<span data-ttu-id="cdcaf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdcaf-117">Application</span></span>|<span data-ttu-id="cdcaf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdcaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdcaf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdcaf-120">Optional query parameters</span></span>
<span data-ttu-id="cdcaf-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdcaf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdcaf-122">Request headers</span></span>
|<span data-ttu-id="cdcaf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdcaf-123">Header</span></span>|<span data-ttu-id="cdcaf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cdcaf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdcaf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcaf-125">Authorization</span></span>|<span data-ttu-id="cdcaf-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cdcaf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdcaf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cdcaf-127">Accept</span></span>|<span data-ttu-id="cdcaf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cdcaf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdcaf-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdcaf-129">Request body</span></span>
<span data-ttu-id="cdcaf-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdcaf-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcaf-131">Response</span></span>
<span data-ttu-id="cdcaf-132">Успешно завершена, этот метод возвращает `200 OK` объект [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-132">If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdcaf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cdcaf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdcaf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcaf-134">Request</span></span>
<span data-ttu-id="cdcaf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="cdcaf-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcaf-136">Response</span></span>
<span data-ttu-id="cdcaf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cdcaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





