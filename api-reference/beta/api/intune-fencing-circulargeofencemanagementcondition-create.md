---
title: Создание Циркуларжеофенцеманажементкондитион
description: Создание нового объекта Циркуларжеофенцеманажементкондитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05c9d99d0b9b27e462a1b0e9a0579b40ccb2aab4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355691"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="4baa0-103">Создание Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="4baa0-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="4baa0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4baa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4baa0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4baa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4baa0-106">Создание нового объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="4baa0-106">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4baa0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4baa0-107">Prerequisites</span></span>
<span data-ttu-id="4baa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4baa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4baa0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4baa0-110">Permission type</span></span>|<span data-ttu-id="4baa0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4baa0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4baa0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4baa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4baa0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4baa0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4baa0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4baa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4baa0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4baa0-115">Not supported.</span></span>|
|<span data-ttu-id="4baa0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4baa0-116">Application</span></span>|<span data-ttu-id="4baa0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4baa0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4baa0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4baa0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4baa0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4baa0-119">Request headers</span></span>
|<span data-ttu-id="4baa0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4baa0-120">Header</span></span>|<span data-ttu-id="4baa0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4baa0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4baa0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4baa0-122">Authorization</span></span>|<span data-ttu-id="4baa0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4baa0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4baa0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4baa0-124">Accept</span></span>|<span data-ttu-id="4baa0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4baa0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4baa0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4baa0-126">Request body</span></span>
<span data-ttu-id="4baa0-127">В тексте запроса добавьте представление объекта Циркуларжеофенцеманажементкондитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4baa0-127">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="4baa0-128">В следующей таблице приведены свойства, необходимые при создании Циркуларжеофенцеманажементкондитион.</span><span class="sxs-lookup"><span data-stu-id="4baa0-128">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="4baa0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4baa0-129">Property</span></span>|<span data-ttu-id="4baa0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4baa0-130">Type</span></span>|<span data-ttu-id="4baa0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4baa0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4baa0-132">id</span><span class="sxs-lookup"><span data-stu-id="4baa0-132">id</span></span>|<span data-ttu-id="4baa0-133">String</span><span class="sxs-lookup"><span data-stu-id="4baa0-133">String</span></span>|<span data-ttu-id="4baa0-134">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="4baa0-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="4baa0-135">System generated value assigned when created.</span></span> <span data-ttu-id="4baa0-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="4baa0-137">uniqueName</span></span>|<span data-ttu-id="4baa0-138">String</span><span class="sxs-lookup"><span data-stu-id="4baa0-138">String</span></span>|<span data-ttu-id="4baa0-139">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-139">Unique name for the management condition.</span></span> <span data-ttu-id="4baa0-140">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-140">Used in management condition expressions.</span></span> <span data-ttu-id="4baa0-141">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4baa0-142">displayName</span></span>|<span data-ttu-id="4baa0-143">Строка</span><span class="sxs-lookup"><span data-stu-id="4baa0-143">String</span></span>|<span data-ttu-id="4baa0-144">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="4baa0-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="4baa0-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-146">description</span><span class="sxs-lookup"><span data-stu-id="4baa0-146">description</span></span>|<span data-ttu-id="4baa0-147">String</span><span class="sxs-lookup"><span data-stu-id="4baa0-147">String</span></span>|<span data-ttu-id="4baa0-148">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="4baa0-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="4baa0-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4baa0-150">createdDateTime</span></span>|<span data-ttu-id="4baa0-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4baa0-151">DateTimeOffset</span></span>|<span data-ttu-id="4baa0-152">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-152">The time the management condition was created.</span></span> <span data-ttu-id="4baa0-153">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4baa0-153">Generated service side.</span></span> <span data-ttu-id="4baa0-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4baa0-155">modifiedDateTime</span></span>|<span data-ttu-id="4baa0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4baa0-156">DateTimeOffset</span></span>|<span data-ttu-id="4baa0-157">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-157">The time the management condition was last modified.</span></span> <span data-ttu-id="4baa0-158">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4baa0-158">Updated service side.</span></span> <span data-ttu-id="4baa0-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-160">eTag</span><span class="sxs-lookup"><span data-stu-id="4baa0-160">eTag</span></span>|<span data-ttu-id="4baa0-161">String</span><span class="sxs-lookup"><span data-stu-id="4baa0-161">String</span></span>|<span data-ttu-id="4baa0-162">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-162">ETag of the management condition.</span></span> <span data-ttu-id="4baa0-163">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="4baa0-163">Updated service side.</span></span> <span data-ttu-id="4baa0-164">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4baa0-165">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="4baa0-165">applicablePlatforms</span></span>|<span data-ttu-id="4baa0-166">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="4baa0-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="4baa0-167">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="4baa0-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="4baa0-168">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="4baa0-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="4baa0-169">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4baa0-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="4baa0-170">latitude</span><span class="sxs-lookup"><span data-stu-id="4baa0-170">latitude</span></span>|<span data-ttu-id="4baa0-171">Double</span><span class="sxs-lookup"><span data-stu-id="4baa0-171">Double</span></span>|<span data-ttu-id="4baa0-172">Широта в градусах от – 90 до + 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="4baa0-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="4baa0-173">longitude</span><span class="sxs-lookup"><span data-stu-id="4baa0-173">longitude</span></span>|<span data-ttu-id="4baa0-174">Двойное</span><span class="sxs-lookup"><span data-stu-id="4baa0-174">Double</span></span>|<span data-ttu-id="4baa0-175">Долгота в градусах от – 180 до + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="4baa0-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="4baa0-176">радиусинметерс</span><span class="sxs-lookup"><span data-stu-id="4baa0-176">radiusInMeters</span></span>|<span data-ttu-id="4baa0-177">Одинарное</span><span class="sxs-lookup"><span data-stu-id="4baa0-177">Single</span></span>|<span data-ttu-id="4baa0-178">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="4baa0-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="4baa0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="4baa0-179">Response</span></span>
<span data-ttu-id="4baa0-180">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4baa0-180">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4baa0-181">Пример</span><span class="sxs-lookup"><span data-stu-id="4baa0-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="4baa0-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="4baa0-182">Request</span></span>
<span data-ttu-id="4baa0-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4baa0-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="4baa0-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4baa0-184">Response</span></span>
<span data-ttu-id="4baa0-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4baa0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






