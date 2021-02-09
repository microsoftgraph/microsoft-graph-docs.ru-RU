---
title: Get assignmentFilterEvaluationStatusDetails
description: Чтение свойств и связей объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c2beeeaf12fb8f2edbb842f658e9a2a48b8be47
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160799"
---
# <a name="get-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="8f85f-103">Get assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="8f85f-103">Get assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="8f85f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f85f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f85f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f85f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f85f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f85f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f85f-107">Чтение свойств и связей объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="8f85f-107">Read properties and relationships of the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f85f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f85f-108">Prerequisites</span></span>
<span data-ttu-id="8f85f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f85f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f85f-111">Permission type</span></span>|<span data-ttu-id="8f85f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f85f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f85f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f85f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f85f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f85f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8f85f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f85f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f85f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f85f-116">Not supported.</span></span>|
|<span data-ttu-id="8f85f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f85f-117">Application</span></span>|<span data-ttu-id="8f85f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f85f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f85f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f85f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f85f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f85f-120">Optional query parameters</span></span>
<span data-ttu-id="8f85f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f85f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f85f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f85f-122">Request headers</span></span>
|<span data-ttu-id="8f85f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f85f-123">Header</span></span>|<span data-ttu-id="8f85f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8f85f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f85f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f85f-125">Authorization</span></span>|<span data-ttu-id="8f85f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f85f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f85f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8f85f-127">Accept</span></span>|<span data-ttu-id="8f85f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f85f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f85f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f85f-129">Request body</span></span>
<span data-ttu-id="8f85f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f85f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f85f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f85f-131">Response</span></span>
<span data-ttu-id="8f85f-132">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f85f-132">If successful, this method returns a `200 OK` response code and [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f85f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8f85f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f85f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f85f-134">Request</span></span>
<span data-ttu-id="8f85f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f85f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

### <a name="response"></a><span data-ttu-id="8f85f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f85f-136">Response</span></span>
<span data-ttu-id="8f85f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f85f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 191

{
  "value": {
    "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
    "id": "820ef068-f068-820e-68f0-0e8268f00e82",
    "payloadId": "Payload Id value"
  }
}
```




