---
title: Обновление назначенияFilterEvaluationStatusDetails
description: Обновление свойств объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b80c5a40c930633e54e590a117fc7bcd9ead4e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125333"
---
# <a name="update-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="03cf9-103">Обновление назначенияFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="03cf9-103">Update assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="03cf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03cf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03cf9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03cf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03cf9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03cf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03cf9-107">Обновление свойств объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="03cf9-107">Update the properties of a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03cf9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03cf9-108">Prerequisites</span></span>
<span data-ttu-id="03cf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03cf9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03cf9-111">Permission type</span></span>|<span data-ttu-id="03cf9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03cf9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03cf9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03cf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03cf9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03cf9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03cf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03cf9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03cf9-116">Not supported.</span></span>|
|<span data-ttu-id="03cf9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03cf9-117">Application</span></span>|<span data-ttu-id="03cf9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03cf9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03cf9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03cf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="03cf9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03cf9-120">Request headers</span></span>
|<span data-ttu-id="03cf9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03cf9-121">Header</span></span>|<span data-ttu-id="03cf9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03cf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03cf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03cf9-123">Authorization</span></span>|<span data-ttu-id="03cf9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03cf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03cf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03cf9-125">Accept</span></span>|<span data-ttu-id="03cf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03cf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03cf9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03cf9-127">Request body</span></span>
<span data-ttu-id="03cf9-128">В теле запроса подарим представление JSON для объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="03cf9-128">In the request body, supply a JSON representation for the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

<span data-ttu-id="03cf9-129">В следующей таблице показаны свойства, необходимые при создании [назначенияFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="03cf9-129">The following table shows the properties that are required when you create the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).</span></span>

|<span data-ttu-id="03cf9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03cf9-130">Property</span></span>|<span data-ttu-id="03cf9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03cf9-131">Type</span></span>|<span data-ttu-id="03cf9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03cf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03cf9-133">id</span><span class="sxs-lookup"><span data-stu-id="03cf9-133">id</span></span>|<span data-ttu-id="03cf9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf9-134">String</span></span>|<span data-ttu-id="03cf9-135">Ключ объекта AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="03cf9-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="03cf9-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="03cf9-136">payloadId</span></span>|<span data-ttu-id="03cf9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="03cf9-137">String</span></span>|<span data-ttu-id="03cf9-138">PayloadId, на котором применен фильтр.</span><span class="sxs-lookup"><span data-stu-id="03cf9-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="03cf9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="03cf9-139">Response</span></span>
<span data-ttu-id="03cf9-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03cf9-140">If successful, this method returns a `200 OK` response code and an updated [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03cf9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="03cf9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="03cf9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="03cf9-142">Request</span></span>
<span data-ttu-id="03cf9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03cf9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="03cf9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="03cf9-144">Response</span></span>
<span data-ttu-id="03cf9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03cf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




