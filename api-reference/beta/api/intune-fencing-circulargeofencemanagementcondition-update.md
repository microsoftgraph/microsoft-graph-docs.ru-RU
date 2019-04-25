---
title: Обновление Циркуларжеофенцеманажементкондитион
description: Обновление свойств объекта Циркуларжеофенцеманажементкондитион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa9c306ad3e79967223af5c55a628c84c34978b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532224"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="d4515-103">Обновление Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="d4515-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="d4515-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4515-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4515-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4515-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4515-106">Обновление свойств объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d4515-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4515-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4515-107">Prerequisites</span></span>
<span data-ttu-id="d4515-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4515-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4515-110">Permission type</span></span>|<span data-ttu-id="d4515-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4515-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4515-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4515-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4515-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4515-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4515-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4515-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4515-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4515-115">Not supported.</span></span>|
|<span data-ttu-id="d4515-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4515-116">Application</span></span>|<span data-ttu-id="d4515-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4515-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4515-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4515-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="d4515-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4515-119">Request headers</span></span>
|<span data-ttu-id="d4515-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4515-120">Header</span></span>|<span data-ttu-id="d4515-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d4515-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4515-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4515-122">Authorization</span></span>|<span data-ttu-id="d4515-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4515-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4515-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d4515-124">Accept</span></span>|<span data-ttu-id="d4515-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4515-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4515-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4515-126">Request body</span></span>
<span data-ttu-id="d4515-127">В тексте запроса добавьте представление объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4515-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="d4515-128">В следующей таблице приведены свойства, необходимые при создании [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="d4515-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="d4515-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4515-129">Property</span></span>|<span data-ttu-id="d4515-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d4515-130">Type</span></span>|<span data-ttu-id="d4515-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d4515-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4515-132">id</span><span class="sxs-lookup"><span data-stu-id="d4515-132">id</span></span>|<span data-ttu-id="d4515-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d4515-133">String</span></span>|<span data-ttu-id="d4515-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="d4515-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="d4515-135">System generated value assigned when created.</span></span> <span data-ttu-id="d4515-136">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="d4515-137">uniqueName</span></span>|<span data-ttu-id="d4515-138">String</span><span class="sxs-lookup"><span data-stu-id="d4515-138">String</span></span>|<span data-ttu-id="d4515-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-139">Unique name for the management condition.</span></span> <span data-ttu-id="d4515-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-140">Used in management condition expressions.</span></span> <span data-ttu-id="d4515-141">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d4515-142">displayName</span></span>|<span data-ttu-id="d4515-143">String</span><span class="sxs-lookup"><span data-stu-id="d4515-143">String</span></span>|<span data-ttu-id="d4515-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="d4515-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="d4515-145">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-146">description</span><span class="sxs-lookup"><span data-stu-id="d4515-146">description</span></span>|<span data-ttu-id="d4515-147">String</span><span class="sxs-lookup"><span data-stu-id="d4515-147">String</span></span>|<span data-ttu-id="d4515-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="d4515-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="d4515-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4515-150">createdDateTime</span></span>|<span data-ttu-id="d4515-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4515-151">DateTimeOffset</span></span>|<span data-ttu-id="d4515-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-152">The time the management condition was created.</span></span> <span data-ttu-id="d4515-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="d4515-153">Generated service side.</span></span> <span data-ttu-id="d4515-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4515-155">modifiedDateTime</span></span>|<span data-ttu-id="d4515-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4515-156">DateTimeOffset</span></span>|<span data-ttu-id="d4515-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-157">The time the management condition was last modified.</span></span> <span data-ttu-id="d4515-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="d4515-158">Updated service side.</span></span> <span data-ttu-id="d4515-159">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-160">eTag</span><span class="sxs-lookup"><span data-stu-id="d4515-160">eTag</span></span>|<span data-ttu-id="d4515-161">String</span><span class="sxs-lookup"><span data-stu-id="d4515-161">String</span></span>|<span data-ttu-id="d4515-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-162">ETag of the management condition.</span></span> <span data-ttu-id="d4515-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="d4515-163">Updated service side.</span></span> <span data-ttu-id="d4515-164">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d4515-165">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="d4515-165">applicablePlatforms</span></span>|<span data-ttu-id="d4515-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="d4515-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d4515-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="d4515-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="d4515-168">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="d4515-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="d4515-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="d4515-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="d4515-170">latitude</span><span class="sxs-lookup"><span data-stu-id="d4515-170">latitude</span></span>|<span data-ttu-id="d4515-171">Double</span><span class="sxs-lookup"><span data-stu-id="d4515-171">Double</span></span>|<span data-ttu-id="d4515-172">Широта в градусах от – 90 до + 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="d4515-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="d4515-173">longitude</span><span class="sxs-lookup"><span data-stu-id="d4515-173">longitude</span></span>|<span data-ttu-id="d4515-174">Double</span><span class="sxs-lookup"><span data-stu-id="d4515-174">Double</span></span>|<span data-ttu-id="d4515-175">Долгота в градусах от – 180 до + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="d4515-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="d4515-176">Радиусинметерс</span><span class="sxs-lookup"><span data-stu-id="d4515-176">radiusInMeters</span></span>|<span data-ttu-id="d4515-177">Одинарное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d4515-177">Single</span></span>|<span data-ttu-id="d4515-178">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="d4515-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="d4515-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4515-179">Response</span></span>
<span data-ttu-id="d4515-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4515-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4515-181">Пример</span><span class="sxs-lookup"><span data-stu-id="d4515-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4515-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4515-182">Request</span></span>
<span data-ttu-id="d4515-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4515-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4515-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4515-184">Response</span></span>
<span data-ttu-id="d4515-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4515-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





