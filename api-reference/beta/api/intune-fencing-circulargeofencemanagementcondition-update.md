---
title: Обновление Циркуларжеофенцеманажементкондитион
description: Обновление свойств объекта Циркуларжеофенцеманажементкондитион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 651bd899e100d9ece72059f69685a42b0101cfea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967204"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="b2e60-103">Обновление Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="b2e60-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="b2e60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2e60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e60-106">Обновление свойств объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b2e60-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2e60-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2e60-107">Prerequisites</span></span>
<span data-ttu-id="b2e60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2e60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2e60-110">Permission type</span></span>|<span data-ttu-id="b2e60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2e60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2e60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2e60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2e60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2e60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2e60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2e60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2e60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e60-115">Not supported.</span></span>|
|<span data-ttu-id="b2e60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2e60-116">Application</span></span>|<span data-ttu-id="b2e60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2e60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2e60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="b2e60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2e60-119">Request headers</span></span>
|<span data-ttu-id="b2e60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2e60-120">Header</span></span>|<span data-ttu-id="b2e60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2e60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2e60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2e60-122">Authorization</span></span>|<span data-ttu-id="b2e60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2e60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2e60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2e60-124">Accept</span></span>|<span data-ttu-id="b2e60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2e60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2e60-126">Request body</span></span>
<span data-ttu-id="b2e60-127">В тексте запроса добавьте представление объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e60-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="b2e60-128">В следующей таблице приведены свойства, необходимые при создании [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="b2e60-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="b2e60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e60-129">Property</span></span>|<span data-ttu-id="b2e60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e60-130">Type</span></span>|<span data-ttu-id="b2e60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e60-132">id</span><span class="sxs-lookup"><span data-stu-id="b2e60-132">id</span></span>|<span data-ttu-id="b2e60-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b2e60-133">String</span></span>|<span data-ttu-id="b2e60-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="b2e60-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="b2e60-135">System generated value assigned when created.</span></span> <span data-ttu-id="b2e60-136">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b2e60-137">uniqueName</span></span>|<span data-ttu-id="b2e60-138">String</span><span class="sxs-lookup"><span data-stu-id="b2e60-138">String</span></span>|<span data-ttu-id="b2e60-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-139">Unique name for the management condition.</span></span> <span data-ttu-id="b2e60-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-140">Used in management condition expressions.</span></span> <span data-ttu-id="b2e60-141">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b2e60-142">displayName</span></span>|<span data-ttu-id="b2e60-143">String</span><span class="sxs-lookup"><span data-stu-id="b2e60-143">String</span></span>|<span data-ttu-id="b2e60-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="b2e60-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="b2e60-145">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-146">description</span><span class="sxs-lookup"><span data-stu-id="b2e60-146">description</span></span>|<span data-ttu-id="b2e60-147">String</span><span class="sxs-lookup"><span data-stu-id="b2e60-147">String</span></span>|<span data-ttu-id="b2e60-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="b2e60-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="b2e60-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2e60-150">createdDateTime</span></span>|<span data-ttu-id="b2e60-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e60-151">DateTimeOffset</span></span>|<span data-ttu-id="b2e60-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-152">The time the management condition was created.</span></span> <span data-ttu-id="b2e60-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b2e60-153">Generated service side.</span></span> <span data-ttu-id="b2e60-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2e60-155">modifiedDateTime</span></span>|<span data-ttu-id="b2e60-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e60-156">DateTimeOffset</span></span>|<span data-ttu-id="b2e60-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-157">The time the management condition was last modified.</span></span> <span data-ttu-id="b2e60-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b2e60-158">Updated service side.</span></span> <span data-ttu-id="b2e60-159">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-160">eTag</span><span class="sxs-lookup"><span data-stu-id="b2e60-160">eTag</span></span>|<span data-ttu-id="b2e60-161">String</span><span class="sxs-lookup"><span data-stu-id="b2e60-161">String</span></span>|<span data-ttu-id="b2e60-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-162">ETag of the management condition.</span></span> <span data-ttu-id="b2e60-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b2e60-163">Updated service side.</span></span> <span data-ttu-id="b2e60-164">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2e60-165">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="b2e60-165">applicablePlatforms</span></span>|<span data-ttu-id="b2e60-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="b2e60-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b2e60-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="b2e60-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b2e60-168">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="b2e60-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="b2e60-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="b2e60-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="b2e60-170">latitude</span><span class="sxs-lookup"><span data-stu-id="b2e60-170">latitude</span></span>|<span data-ttu-id="b2e60-171">Double</span><span class="sxs-lookup"><span data-stu-id="b2e60-171">Double</span></span>|<span data-ttu-id="b2e60-172">Широта в градусах от – 90 до + 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="b2e60-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="b2e60-173">longitude</span><span class="sxs-lookup"><span data-stu-id="b2e60-173">longitude</span></span>|<span data-ttu-id="b2e60-174">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b2e60-174">Double</span></span>|<span data-ttu-id="b2e60-175">Долгота в градусах от – 180 до + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="b2e60-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="b2e60-176">Радиусинметерс</span><span class="sxs-lookup"><span data-stu-id="b2e60-176">radiusInMeters</span></span>|<span data-ttu-id="b2e60-177">Одинарное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b2e60-177">Single</span></span>|<span data-ttu-id="b2e60-178">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="b2e60-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="b2e60-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e60-179">Response</span></span>
<span data-ttu-id="b2e60-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2e60-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e60-181">Пример</span><span class="sxs-lookup"><span data-stu-id="b2e60-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2e60-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2e60-182">Request</span></span>
<span data-ttu-id="b2e60-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2e60-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2e60-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e60-184">Response</span></span>
<span data-ttu-id="b2e60-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2e60-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




