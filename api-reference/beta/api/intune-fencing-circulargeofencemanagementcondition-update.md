---
title: Обновление Циркуларжеофенцеманажементкондитион
description: Обновление свойств объекта Циркуларжеофенцеманажементкондитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de4ff2a3903e71a3af2a7de090766cc45bcec127
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442261"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="f1d45-103">Обновление Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="f1d45-103">Update circularGeofenceManagementCondition</span></span>

<span data-ttu-id="f1d45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1d45-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1d45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1d45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1d45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d45-107">Обновление свойств объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f1d45-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1d45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1d45-108">Prerequisites</span></span>
<span data-ttu-id="f1d45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d45-111">Permission type</span></span>|<span data-ttu-id="f1d45-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1d45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1d45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1d45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1d45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1d45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1d45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1d45-116">Not supported.</span></span>|
|<span data-ttu-id="f1d45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1d45-117">Application</span></span>|<span data-ttu-id="f1d45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1d45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1d45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="f1d45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1d45-120">Request headers</span></span>
|<span data-ttu-id="f1d45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1d45-121">Header</span></span>|<span data-ttu-id="f1d45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1d45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1d45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1d45-123">Authorization</span></span>|<span data-ttu-id="f1d45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1d45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1d45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1d45-125">Accept</span></span>|<span data-ttu-id="f1d45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1d45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d45-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1d45-127">Request body</span></span>
<span data-ttu-id="f1d45-128">В тексте запроса добавьте представление объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1d45-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="f1d45-129">В следующей таблице приведены свойства, необходимые при создании [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f1d45-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="f1d45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1d45-130">Property</span></span>|<span data-ttu-id="f1d45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1d45-131">Type</span></span>|<span data-ttu-id="f1d45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d45-133">id</span><span class="sxs-lookup"><span data-stu-id="f1d45-133">id</span></span>|<span data-ttu-id="f1d45-134">String</span><span class="sxs-lookup"><span data-stu-id="f1d45-134">String</span></span>|<span data-ttu-id="f1d45-135">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="f1d45-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="f1d45-136">System generated value assigned when created.</span></span> <span data-ttu-id="f1d45-137">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f1d45-138">uniqueName</span></span>|<span data-ttu-id="f1d45-139">String</span><span class="sxs-lookup"><span data-stu-id="f1d45-139">String</span></span>|<span data-ttu-id="f1d45-140">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-140">Unique name for the management condition.</span></span> <span data-ttu-id="f1d45-141">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-141">Used in management condition expressions.</span></span> <span data-ttu-id="f1d45-142">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f1d45-143">displayName</span></span>|<span data-ttu-id="f1d45-144">Строка</span><span class="sxs-lookup"><span data-stu-id="f1d45-144">String</span></span>|<span data-ttu-id="f1d45-145">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="f1d45-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="f1d45-146">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-147">description</span><span class="sxs-lookup"><span data-stu-id="f1d45-147">description</span></span>|<span data-ttu-id="f1d45-148">String</span><span class="sxs-lookup"><span data-stu-id="f1d45-148">String</span></span>|<span data-ttu-id="f1d45-149">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="f1d45-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="f1d45-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d45-151">createdDateTime</span></span>|<span data-ttu-id="f1d45-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d45-152">DateTimeOffset</span></span>|<span data-ttu-id="f1d45-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-153">The time the management condition was created.</span></span> <span data-ttu-id="f1d45-154">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1d45-154">Generated service side.</span></span> <span data-ttu-id="f1d45-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d45-156">modifiedDateTime</span></span>|<span data-ttu-id="f1d45-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d45-157">DateTimeOffset</span></span>|<span data-ttu-id="f1d45-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-158">The time the management condition was last modified.</span></span> <span data-ttu-id="f1d45-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1d45-159">Updated service side.</span></span> <span data-ttu-id="f1d45-160">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-161">eTag</span><span class="sxs-lookup"><span data-stu-id="f1d45-161">eTag</span></span>|<span data-ttu-id="f1d45-162">String</span><span class="sxs-lookup"><span data-stu-id="f1d45-162">String</span></span>|<span data-ttu-id="f1d45-163">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-163">ETag of the management condition.</span></span> <span data-ttu-id="f1d45-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f1d45-164">Updated service side.</span></span> <span data-ttu-id="f1d45-165">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f1d45-166">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="f1d45-166">applicablePlatforms</span></span>|<span data-ttu-id="f1d45-167">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f1d45-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f1d45-168">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="f1d45-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f1d45-169">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f1d45-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f1d45-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f1d45-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="f1d45-171">latitude</span><span class="sxs-lookup"><span data-stu-id="f1d45-171">latitude</span></span>|<span data-ttu-id="f1d45-172">Double</span><span class="sxs-lookup"><span data-stu-id="f1d45-172">Double</span></span>|<span data-ttu-id="f1d45-173">Широта в градусах от – 90 до + 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="f1d45-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="f1d45-174">longitude</span><span class="sxs-lookup"><span data-stu-id="f1d45-174">longitude</span></span>|<span data-ttu-id="f1d45-175">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f1d45-175">Double</span></span>|<span data-ttu-id="f1d45-176">Долгота в градусах от – 180 до + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="f1d45-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="f1d45-177">радиусинметерс</span><span class="sxs-lookup"><span data-stu-id="f1d45-177">radiusInMeters</span></span>|<span data-ttu-id="f1d45-178">Одинарное</span><span class="sxs-lookup"><span data-stu-id="f1d45-178">Single</span></span>|<span data-ttu-id="f1d45-179">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="f1d45-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="f1d45-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1d45-180">Response</span></span>
<span data-ttu-id="f1d45-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1d45-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d45-182">Пример</span><span class="sxs-lookup"><span data-stu-id="f1d45-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1d45-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1d45-183">Request</span></span>
<span data-ttu-id="f1d45-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1d45-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a><span data-ttu-id="f1d45-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1d45-185">Response</span></span>
<span data-ttu-id="f1d45-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1d45-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

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
```



