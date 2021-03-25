---
title: Создание assignmentFilterEvaluationStatusDetails
description: Создание нового объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa4418ea4e00099e807684196d8960231d3b9c28
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158733"
---
# <a name="create-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="dd0e1-103">Создание assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="dd0e1-103">Create assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="dd0e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd0e1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd0e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd0e1-107">Создание нового [объекта assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e1-107">Create a new [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd0e1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd0e1-108">Prerequisites</span></span>
<span data-ttu-id="dd0e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0e1-111">Permission type</span></span>|<span data-ttu-id="dd0e1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd0e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0e1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd0e1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-116">Not supported.</span></span>|
|<span data-ttu-id="dd0e1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd0e1-117">Application</span></span>|<span data-ttu-id="dd0e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="dd0e1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd0e1-120">Request headers</span></span>
|<span data-ttu-id="dd0e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd0e1-121">Header</span></span>|<span data-ttu-id="dd0e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd0e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0e1-123">Authorization</span></span>|<span data-ttu-id="dd0e1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd0e1-125">Accept</span></span>|<span data-ttu-id="dd0e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd0e1-127">Request body</span></span>
<span data-ttu-id="dd0e1-128">В теле запроса подарим представление JSON для объекта assignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-128">In the request body, supply a JSON representation for the assignmentFilterEvaluationStatusDetails object.</span></span>

<span data-ttu-id="dd0e1-129">В следующей таблице показаны свойства, необходимые при создании назначенияFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-129">The following table shows the properties that are required when you create the assignmentFilterEvaluationStatusDetails.</span></span>

|<span data-ttu-id="dd0e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd0e1-130">Property</span></span>|<span data-ttu-id="dd0e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd0e1-131">Type</span></span>|<span data-ttu-id="dd0e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0e1-133">id</span><span class="sxs-lookup"><span data-stu-id="dd0e1-133">id</span></span>|<span data-ttu-id="dd0e1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e1-134">String</span></span>|<span data-ttu-id="dd0e1-135">Ключ объекта AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="dd0e1-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="dd0e1-136">payloadId</span></span>|<span data-ttu-id="dd0e1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e1-137">String</span></span>|<span data-ttu-id="dd0e1-138">PayloadId, на котором применен фильтр.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="dd0e1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e1-139">Response</span></span>
<span data-ttu-id="dd0e1-140">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-140">If successful, this method returns a `201 Created` response code and a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0e1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dd0e1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd0e1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e1-142">Request</span></span>
<span data-ttu-id="dd0e1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="dd0e1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e1-144">Response</span></span>
<span data-ttu-id="dd0e1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd0e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




