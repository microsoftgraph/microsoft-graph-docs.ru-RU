---
title: Обновление assignmentFilterEvaluationStatusDetails
description: Обновление свойств объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cd53ae8b487a89cdb47b2635f075a4558acf6b8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160682"
---
# <a name="update-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="4b3b4-103">Обновление assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="4b3b4-103">Update assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="4b3b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b3b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b3b4-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b3b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b3b4-107">Обновление свойств объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="4b3b4-107">Update the properties of a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b3b4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b3b4-108">Prerequisites</span></span>
<span data-ttu-id="4b3b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b3b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b3b4-111">Permission type</span></span>|<span data-ttu-id="4b3b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b3b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b3b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b3b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b3b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-116">Not supported.</span></span>|
|<span data-ttu-id="4b3b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b3b4-117">Application</span></span>|<span data-ttu-id="4b3b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b3b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="4b3b4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b3b4-120">Request headers</span></span>
|<span data-ttu-id="4b3b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b3b4-121">Header</span></span>|<span data-ttu-id="4b3b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b3b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b3b4-123">Authorization</span></span>|<span data-ttu-id="4b3b4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b3b4-125">Accept</span></span>|<span data-ttu-id="4b3b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b3b4-127">Request body</span></span>
<span data-ttu-id="4b3b4-128">В теле запроса предопределение представления объекта [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-128">In the request body, supply a JSON representation for the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

<span data-ttu-id="4b3b4-129">В следующей таблице показаны свойства, необходимые при создании [объекта assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="4b3b4-129">The following table shows the properties that are required when you create the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).</span></span>

|<span data-ttu-id="4b3b4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b3b4-130">Property</span></span>|<span data-ttu-id="4b3b4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b3b4-131">Type</span></span>|<span data-ttu-id="4b3b4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b3b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3b4-133">id</span><span class="sxs-lookup"><span data-stu-id="4b3b4-133">id</span></span>|<span data-ttu-id="4b3b4-134">String</span><span class="sxs-lookup"><span data-stu-id="4b3b4-134">String</span></span>|<span data-ttu-id="4b3b4-135">Ключ объекта AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="4b3b4-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="4b3b4-136">payloadId</span></span>|<span data-ttu-id="4b3b4-137">String</span><span class="sxs-lookup"><span data-stu-id="4b3b4-137">String</span></span>|<span data-ttu-id="4b3b4-138">PayloadId, к которому применен фильтр.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="4b3b4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b3b4-139">Response</span></span>
<span data-ttu-id="4b3b4-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-140">If successful, this method returns a `200 OK` response code and an updated [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3b4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4b3b4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b3b4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b3b4-142">Request</span></span>
<span data-ttu-id="4b3b4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="4b3b4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b3b4-144">Response</span></span>
<span data-ttu-id="4b3b4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b3b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




