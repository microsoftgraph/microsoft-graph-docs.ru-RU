---
title: Обновление circularGeofenceManagementCondition
description: Обновление свойства объекта circularGeofenceManagementCondition.
ms.openlocfilehash: d1bf21db47f25834f62241fb66a96bcf176f5d8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077767"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="020eb-103">Обновление circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="020eb-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="020eb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="020eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="020eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="020eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="020eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="020eb-107">Обновление свойства объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="020eb-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="020eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="020eb-108">Prerequisites</span></span>
<span data-ttu-id="020eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="020eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="020eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="020eb-111">Permission type</span></span>|<span data-ttu-id="020eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="020eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="020eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="020eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="020eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="020eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="020eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="020eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="020eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020eb-116">Not supported.</span></span>|
|<span data-ttu-id="020eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="020eb-117">Application</span></span>|<span data-ttu-id="020eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="020eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="020eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="020eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="020eb-120">Request headers</span></span>
|<span data-ttu-id="020eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="020eb-121">Header</span></span>|<span data-ttu-id="020eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="020eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="020eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="020eb-123">Authorization</span></span>|<span data-ttu-id="020eb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="020eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="020eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="020eb-125">Accept</span></span>|<span data-ttu-id="020eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="020eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="020eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="020eb-127">Request body</span></span>
<span data-ttu-id="020eb-128">В тексте запроса укажите представление JSON для объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="020eb-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="020eb-129">В следующей таблице показаны свойства, которые необходимы для создания [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="020eb-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="020eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="020eb-130">Property</span></span>|<span data-ttu-id="020eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="020eb-131">Type</span></span>|<span data-ttu-id="020eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="020eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="020eb-133">id</span><span class="sxs-lookup"><span data-stu-id="020eb-133">id</span></span>|<span data-ttu-id="020eb-134">String</span><span class="sxs-lookup"><span data-stu-id="020eb-134">String</span></span>|<span data-ttu-id="020eb-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="020eb-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="020eb-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="020eb-136">System generated value assigned when created.</span></span> <span data-ttu-id="020eb-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="020eb-138">uniqueName</span></span>|<span data-ttu-id="020eb-139">String</span><span class="sxs-lookup"><span data-stu-id="020eb-139">String</span></span>|<span data-ttu-id="020eb-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="020eb-140">Unique name for the management condition.</span></span> <span data-ttu-id="020eb-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="020eb-141">Used in management condition expressions.</span></span> <span data-ttu-id="020eb-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-143">displayName</span><span class="sxs-lookup"><span data-stu-id="020eb-143">displayName</span></span>|<span data-ttu-id="020eb-144">String</span><span class="sxs-lookup"><span data-stu-id="020eb-144">String</span></span>|<span data-ttu-id="020eb-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="020eb-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="020eb-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-147">описание</span><span class="sxs-lookup"><span data-stu-id="020eb-147">description</span></span>|<span data-ttu-id="020eb-148">String</span><span class="sxs-lookup"><span data-stu-id="020eb-148">String</span></span>|<span data-ttu-id="020eb-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="020eb-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="020eb-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="020eb-151">createdDateTime</span></span>|<span data-ttu-id="020eb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020eb-152">DateTimeOffset</span></span>|<span data-ttu-id="020eb-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="020eb-153">The time the management condition was created.</span></span> <span data-ttu-id="020eb-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="020eb-154">Generated service side.</span></span> <span data-ttu-id="020eb-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="020eb-156">modifiedDateTime</span></span>|<span data-ttu-id="020eb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020eb-157">DateTimeOffset</span></span>|<span data-ttu-id="020eb-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="020eb-158">The time the management condition was last modified.</span></span> <span data-ttu-id="020eb-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="020eb-159">Updated service side.</span></span> <span data-ttu-id="020eb-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-161">eTag</span><span class="sxs-lookup"><span data-stu-id="020eb-161">eTag</span></span>|<span data-ttu-id="020eb-162">String</span><span class="sxs-lookup"><span data-stu-id="020eb-162">String</span></span>|<span data-ttu-id="020eb-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="020eb-163">ETag of the management condition.</span></span> <span data-ttu-id="020eb-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="020eb-164">Updated service side.</span></span> <span data-ttu-id="020eb-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="020eb-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="020eb-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="020eb-166">applicablePlatforms</span></span>|<span data-ttu-id="020eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="020eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="020eb-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="020eb-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="020eb-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="020eb-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="020eb-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="020eb-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="020eb-171">latitude</span><span class="sxs-lookup"><span data-stu-id="020eb-171">latitude</span></span>|<span data-ttu-id="020eb-172">Double</span><span class="sxs-lookup"><span data-stu-id="020eb-172">Double</span></span>|<span data-ttu-id="020eb-173">Широта в степени, от -90 до 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="020eb-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="020eb-174">longitude</span><span class="sxs-lookup"><span data-stu-id="020eb-174">longitude</span></span>|<span data-ttu-id="020eb-175">Double</span><span class="sxs-lookup"><span data-stu-id="020eb-175">Double</span></span>|<span data-ttu-id="020eb-176">Долгота в градусов между -180 и + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="020eb-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="020eb-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="020eb-177">radiusInMeters</span></span>|<span data-ttu-id="020eb-178">Single</span><span class="sxs-lookup"><span data-stu-id="020eb-178">Single</span></span>|<span data-ttu-id="020eb-179">RADIUS в метры.</span><span class="sxs-lookup"><span data-stu-id="020eb-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="020eb-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="020eb-180">Response</span></span>
<span data-ttu-id="020eb-181">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="020eb-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="020eb-182">Пример</span><span class="sxs-lookup"><span data-stu-id="020eb-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="020eb-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="020eb-183">Request</span></span>
<span data-ttu-id="020eb-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="020eb-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 370

{
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

### <a name="response"></a><span data-ttu-id="020eb-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="020eb-185">Response</span></span>
<span data-ttu-id="020eb-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="020eb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





