---
title: Обновление циркуляраGeofenceManagementCondition
description: Обновление свойств объекта circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af17c331bde66baef8f6f5b53fa454928da06cfe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149837"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="17f4a-103">Обновление циркуляраGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="17f4a-103">Update circularGeofenceManagementCondition</span></span>

<span data-ttu-id="17f4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17f4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17f4a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17f4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17f4a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17f4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f4a-107">Обновление свойств объекта [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17f4a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17f4a-108">Prerequisites</span></span>
<span data-ttu-id="17f4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f4a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17f4a-111">Permission type</span></span>|<span data-ttu-id="17f4a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17f4a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17f4a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17f4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17f4a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f4a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17f4a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17f4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17f4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17f4a-116">Not supported.</span></span>|
|<span data-ttu-id="17f4a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17f4a-117">Application</span></span>|<span data-ttu-id="17f4a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f4a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17f4a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17f4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="17f4a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17f4a-120">Request headers</span></span>
|<span data-ttu-id="17f4a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17f4a-121">Header</span></span>|<span data-ttu-id="17f4a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17f4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17f4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17f4a-123">Authorization</span></span>|<span data-ttu-id="17f4a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17f4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17f4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17f4a-125">Accept</span></span>|<span data-ttu-id="17f4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17f4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17f4a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17f4a-127">Request body</span></span>
<span data-ttu-id="17f4a-128">В теле запроса поставляем представление JSON для объекта [circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="17f4a-129">В следующей таблице показаны свойства, необходимые при создании [круговогоGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="17f4a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17f4a-130">Property</span></span>|<span data-ttu-id="17f4a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17f4a-131">Type</span></span>|<span data-ttu-id="17f4a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17f4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f4a-133">id</span><span class="sxs-lookup"><span data-stu-id="17f4a-133">id</span></span>|<span data-ttu-id="17f4a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="17f4a-134">String</span></span>|<span data-ttu-id="17f4a-135">Уникальный идентификатор для состояния управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="17f4a-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="17f4a-136">System generated value assigned when created.</span></span> <span data-ttu-id="17f4a-137">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="17f4a-138">uniqueName</span></span>|<span data-ttu-id="17f4a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="17f4a-139">String</span></span>|<span data-ttu-id="17f4a-140">Уникальное имя для состояния управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-140">Unique name for the management condition.</span></span> <span data-ttu-id="17f4a-141">Используется в выражениях условий управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-141">Used in management condition expressions.</span></span> <span data-ttu-id="17f4a-142">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="17f4a-143">displayName</span></span>|<span data-ttu-id="17f4a-144">Строка</span><span class="sxs-lookup"><span data-stu-id="17f4a-144">String</span></span>|<span data-ttu-id="17f4a-145">Администратор определил имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="17f4a-146">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-147">description</span><span class="sxs-lookup"><span data-stu-id="17f4a-147">description</span></span>|<span data-ttu-id="17f4a-148">Строка</span><span class="sxs-lookup"><span data-stu-id="17f4a-148">String</span></span>|<span data-ttu-id="17f4a-149">Администратор определил описание условия управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="17f4a-150">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17f4a-151">createdDateTime</span></span>|<span data-ttu-id="17f4a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f4a-152">DateTimeOffset</span></span>|<span data-ttu-id="17f4a-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-153">The time the management condition was created.</span></span> <span data-ttu-id="17f4a-154">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="17f4a-154">Generated service side.</span></span> <span data-ttu-id="17f4a-155">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17f4a-156">modifiedDateTime</span></span>|<span data-ttu-id="17f4a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f4a-157">DateTimeOffset</span></span>|<span data-ttu-id="17f4a-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-158">The time the management condition was last modified.</span></span> <span data-ttu-id="17f4a-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="17f4a-159">Updated service side.</span></span> <span data-ttu-id="17f4a-160">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-161">eTag</span><span class="sxs-lookup"><span data-stu-id="17f4a-161">eTag</span></span>|<span data-ttu-id="17f4a-162">String</span><span class="sxs-lookup"><span data-stu-id="17f4a-162">String</span></span>|<span data-ttu-id="17f4a-163">ETag состояния управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-163">ETag of the management condition.</span></span> <span data-ttu-id="17f4a-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="17f4a-164">Updated service side.</span></span> <span data-ttu-id="17f4a-165">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="17f4a-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="17f4a-166">applicablePlatforms</span></span>|<span data-ttu-id="17f4a-167">[коллекция devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="17f4a-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="17f4a-168">Применимые платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="17f4a-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="17f4a-169">Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="17f4a-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="17f4a-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="17f4a-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="17f4a-171">latitude</span><span class="sxs-lookup"><span data-stu-id="17f4a-171">latitude</span></span>|<span data-ttu-id="17f4a-172">Double</span><span class="sxs-lookup"><span data-stu-id="17f4a-172">Double</span></span>|<span data-ttu-id="17f4a-173">Широта в градусах, от -90 до +90 включительно.</span><span class="sxs-lookup"><span data-stu-id="17f4a-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="17f4a-174">longitude</span><span class="sxs-lookup"><span data-stu-id="17f4a-174">longitude</span></span>|<span data-ttu-id="17f4a-175">Double</span><span class="sxs-lookup"><span data-stu-id="17f4a-175">Double</span></span>|<span data-ttu-id="17f4a-176">Долгота в градусах, от -180 до +180 включительно.</span><span class="sxs-lookup"><span data-stu-id="17f4a-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="17f4a-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="17f4a-177">radiusInMeters</span></span>|<span data-ttu-id="17f4a-178">Одинарное</span><span class="sxs-lookup"><span data-stu-id="17f4a-178">Single</span></span>|<span data-ttu-id="17f4a-179">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="17f4a-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="17f4a-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="17f4a-180">Response</span></span>
<span data-ttu-id="17f4a-181">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="17f4a-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f4a-182">Пример</span><span class="sxs-lookup"><span data-stu-id="17f4a-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="17f4a-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="17f4a-183">Request</span></span>
<span data-ttu-id="17f4a-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17f4a-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```

### <a name="response"></a><span data-ttu-id="17f4a-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="17f4a-185">Response</span></span>
<span data-ttu-id="17f4a-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17f4a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

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
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```




