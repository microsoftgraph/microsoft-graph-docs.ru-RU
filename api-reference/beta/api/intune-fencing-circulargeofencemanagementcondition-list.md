---
title: Список circularGeofenceManagementConditions
description: Свойства списка и связей объектов circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: df8cc05ebc9e6b608232dd9b894968ca5f8b3234
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944616"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="45128-103">Список circularGeofenceManagementConditions</span><span class="sxs-lookup"><span data-stu-id="45128-103">List circularGeofenceManagementConditions</span></span>

> <span data-ttu-id="45128-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45128-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45128-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45128-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45128-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45128-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45128-107">Свойства списка и связей объектов [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="45128-107">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45128-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45128-108">Prerequisites</span></span>
<span data-ttu-id="45128-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45128-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45128-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45128-111">Permission type</span></span>|<span data-ttu-id="45128-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45128-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45128-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45128-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45128-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45128-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45128-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45128-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45128-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45128-116">Not supported.</span></span>|
|<span data-ttu-id="45128-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45128-117">Application</span></span>|<span data-ttu-id="45128-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45128-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45128-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45128-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="45128-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45128-120">Request headers</span></span>
|<span data-ttu-id="45128-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45128-121">Header</span></span>|<span data-ttu-id="45128-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45128-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45128-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45128-123">Authorization</span></span>|<span data-ttu-id="45128-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45128-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45128-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45128-125">Accept</span></span>|<span data-ttu-id="45128-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45128-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45128-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45128-127">Request body</span></span>
<span data-ttu-id="45128-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45128-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45128-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="45128-129">Response</span></span>
<span data-ttu-id="45128-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45128-130">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45128-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45128-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="45128-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45128-132">Request</span></span>
<span data-ttu-id="45128-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45128-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="45128-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="45128-134">Response</span></span>
<span data-ttu-id="45128-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45128-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





