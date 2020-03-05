---
title: Создание Циркуларжеофенцеманажементкондитион
description: Создание нового объекта Циркуларжеофенцеманажементкондитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcae78759cfd13042d4baef6958f1c3cb835f2ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465942"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="7a149-103">Создание Циркуларжеофенцеманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="7a149-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="7a149-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a149-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a149-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a149-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a149-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a149-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a149-107">Создание нового объекта [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="7a149-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a149-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a149-108">Prerequisites</span></span>
<span data-ttu-id="7a149-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a149-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a149-111">Permission type</span></span>|<span data-ttu-id="7a149-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a149-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a149-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a149-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a149-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a149-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a149-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a149-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a149-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a149-116">Not supported.</span></span>|
|<span data-ttu-id="7a149-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a149-117">Application</span></span>|<span data-ttu-id="7a149-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a149-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a149-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a149-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="7a149-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a149-120">Request headers</span></span>
|<span data-ttu-id="7a149-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a149-121">Header</span></span>|<span data-ttu-id="7a149-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a149-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a149-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a149-123">Authorization</span></span>|<span data-ttu-id="7a149-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a149-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a149-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a149-125">Accept</span></span>|<span data-ttu-id="7a149-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a149-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a149-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a149-127">Request body</span></span>
<span data-ttu-id="7a149-128">В тексте запроса добавьте представление объекта Циркуларжеофенцеманажементкондитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a149-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="7a149-129">В следующей таблице приведены свойства, необходимые при создании Циркуларжеофенцеманажементкондитион.</span><span class="sxs-lookup"><span data-stu-id="7a149-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="7a149-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a149-130">Property</span></span>|<span data-ttu-id="7a149-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a149-131">Type</span></span>|<span data-ttu-id="7a149-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a149-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a149-133">id</span><span class="sxs-lookup"><span data-stu-id="7a149-133">id</span></span>|<span data-ttu-id="7a149-134">String</span><span class="sxs-lookup"><span data-stu-id="7a149-134">String</span></span>|<span data-ttu-id="7a149-135">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="7a149-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="7a149-136">System generated value assigned when created.</span></span> <span data-ttu-id="7a149-137">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="7a149-138">uniqueName</span></span>|<span data-ttu-id="7a149-139">String</span><span class="sxs-lookup"><span data-stu-id="7a149-139">String</span></span>|<span data-ttu-id="7a149-140">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-140">Unique name for the management condition.</span></span> <span data-ttu-id="7a149-141">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-141">Used in management condition expressions.</span></span> <span data-ttu-id="7a149-142">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7a149-143">displayName</span></span>|<span data-ttu-id="7a149-144">Строка</span><span class="sxs-lookup"><span data-stu-id="7a149-144">String</span></span>|<span data-ttu-id="7a149-145">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="7a149-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="7a149-146">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-147">description</span><span class="sxs-lookup"><span data-stu-id="7a149-147">description</span></span>|<span data-ttu-id="7a149-148">String</span><span class="sxs-lookup"><span data-stu-id="7a149-148">String</span></span>|<span data-ttu-id="7a149-149">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="7a149-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="7a149-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a149-151">createdDateTime</span></span>|<span data-ttu-id="7a149-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a149-152">DateTimeOffset</span></span>|<span data-ttu-id="7a149-153">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-153">The time the management condition was created.</span></span> <span data-ttu-id="7a149-154">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="7a149-154">Generated service side.</span></span> <span data-ttu-id="7a149-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a149-156">modifiedDateTime</span></span>|<span data-ttu-id="7a149-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a149-157">DateTimeOffset</span></span>|<span data-ttu-id="7a149-158">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-158">The time the management condition was last modified.</span></span> <span data-ttu-id="7a149-159">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="7a149-159">Updated service side.</span></span> <span data-ttu-id="7a149-160">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-161">eTag</span><span class="sxs-lookup"><span data-stu-id="7a149-161">eTag</span></span>|<span data-ttu-id="7a149-162">String</span><span class="sxs-lookup"><span data-stu-id="7a149-162">String</span></span>|<span data-ttu-id="7a149-163">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-163">ETag of the management condition.</span></span> <span data-ttu-id="7a149-164">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="7a149-164">Updated service side.</span></span> <span data-ttu-id="7a149-165">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7a149-166">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="7a149-166">applicablePlatforms</span></span>|<span data-ttu-id="7a149-167">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="7a149-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7a149-168">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="7a149-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="7a149-169">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="7a149-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="7a149-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7a149-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="7a149-171">latitude</span><span class="sxs-lookup"><span data-stu-id="7a149-171">latitude</span></span>|<span data-ttu-id="7a149-172">Double</span><span class="sxs-lookup"><span data-stu-id="7a149-172">Double</span></span>|<span data-ttu-id="7a149-173">Широта в градусах от – 90 до + 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="7a149-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="7a149-174">longitude</span><span class="sxs-lookup"><span data-stu-id="7a149-174">longitude</span></span>|<span data-ttu-id="7a149-175">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7a149-175">Double</span></span>|<span data-ttu-id="7a149-176">Долгота в градусах от – 180 до + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="7a149-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="7a149-177">радиусинметерс</span><span class="sxs-lookup"><span data-stu-id="7a149-177">radiusInMeters</span></span>|<span data-ttu-id="7a149-178">Одинарное</span><span class="sxs-lookup"><span data-stu-id="7a149-178">Single</span></span>|<span data-ttu-id="7a149-179">Радиус в метрах.</span><span class="sxs-lookup"><span data-stu-id="7a149-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="7a149-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a149-180">Response</span></span>
<span data-ttu-id="7a149-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Циркуларжеофенцеманажементкондитион](../resources/intune-fencing-circulargeofencemanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a149-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a149-182">Пример</span><span class="sxs-lookup"><span data-stu-id="7a149-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a149-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a149-183">Request</span></span>
<span data-ttu-id="7a149-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a149-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7a149-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a149-185">Response</span></span>
<span data-ttu-id="7a149-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a149-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





