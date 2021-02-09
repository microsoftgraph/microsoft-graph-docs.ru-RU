---
title: Создание assignmentFilterEvaluationStatusDetails
description: Создание объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a234b511821db87d92ee91416f6094379360cc6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160805"
---
# <a name="create-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="17d19-103">Создание assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="17d19-103">Create assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="17d19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17d19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17d19-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17d19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17d19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17d19-107">Создание объекта [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="17d19-107">Create a new [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17d19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17d19-108">Prerequisites</span></span>
<span data-ttu-id="17d19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17d19-111">Permission type</span></span>|<span data-ttu-id="17d19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17d19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17d19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17d19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17d19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17d19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17d19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17d19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d19-116">Not supported.</span></span>|
|<span data-ttu-id="17d19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17d19-117">Application</span></span>|<span data-ttu-id="17d19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17d19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17d19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="17d19-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17d19-120">Request headers</span></span>
|<span data-ttu-id="17d19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17d19-121">Header</span></span>|<span data-ttu-id="17d19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17d19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17d19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17d19-123">Authorization</span></span>|<span data-ttu-id="17d19-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17d19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17d19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17d19-125">Accept</span></span>|<span data-ttu-id="17d19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17d19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17d19-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17d19-127">Request body</span></span>
<span data-ttu-id="17d19-128">В теле запроса предопределение представления объекта assignmentFilterEvaluationStatusDetails в JSON.</span><span class="sxs-lookup"><span data-stu-id="17d19-128">In the request body, supply a JSON representation for the assignmentFilterEvaluationStatusDetails object.</span></span>

<span data-ttu-id="17d19-129">В следующей таблице показаны свойства, необходимые при создании объекта assignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="17d19-129">The following table shows the properties that are required when you create the assignmentFilterEvaluationStatusDetails.</span></span>

|<span data-ttu-id="17d19-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17d19-130">Property</span></span>|<span data-ttu-id="17d19-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17d19-131">Type</span></span>|<span data-ttu-id="17d19-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17d19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17d19-133">id</span><span class="sxs-lookup"><span data-stu-id="17d19-133">id</span></span>|<span data-ttu-id="17d19-134">String</span><span class="sxs-lookup"><span data-stu-id="17d19-134">String</span></span>|<span data-ttu-id="17d19-135">Ключ объекта AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="17d19-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="17d19-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="17d19-136">payloadId</span></span>|<span data-ttu-id="17d19-137">String</span><span class="sxs-lookup"><span data-stu-id="17d19-137">String</span></span>|<span data-ttu-id="17d19-138">PayloadId, к которому применен фильтр.</span><span class="sxs-lookup"><span data-stu-id="17d19-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="17d19-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="17d19-139">Response</span></span>
<span data-ttu-id="17d19-140">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17d19-140">If successful, this method returns a `201 Created` response code and a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17d19-141">Пример</span><span class="sxs-lookup"><span data-stu-id="17d19-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="17d19-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="17d19-142">Request</span></span>
<span data-ttu-id="17d19-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17d19-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="17d19-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="17d19-144">Response</span></span>
<span data-ttu-id="17d19-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17d19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




