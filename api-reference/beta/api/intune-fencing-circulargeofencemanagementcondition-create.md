---
title: Создание circularGeofenceManagementCondition
description: Создание нового объекта circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6ca3d469280b3419700e6948d66e8e3ed1640b22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979595"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="430e6-103">Создание circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="430e6-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="430e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="430e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="430e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="430e6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="430e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="430e6-107">Создание нового объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="430e6-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="430e6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="430e6-108">Prerequisites</span></span>
<span data-ttu-id="430e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="430e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="430e6-111">Permission type</span></span>|<span data-ttu-id="430e6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="430e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="430e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="430e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="430e6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430e6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="430e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="430e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="430e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430e6-116">Not supported.</span></span>|
|<span data-ttu-id="430e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="430e6-117">Application</span></span>|<span data-ttu-id="430e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="430e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="430e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="430e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="430e6-120">Request headers</span></span>
|<span data-ttu-id="430e6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="430e6-121">Header</span></span>|<span data-ttu-id="430e6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="430e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="430e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="430e6-123">Authorization</span></span>|<span data-ttu-id="430e6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="430e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="430e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="430e6-125">Accept</span></span>|<span data-ttu-id="430e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="430e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="430e6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="430e6-127">Request body</span></span>
<span data-ttu-id="430e6-128">В тексте запроса укажите представление JSON для объекта circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="430e6-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="430e6-129">В следующей таблице показаны свойства, которые необходимы для создания circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="430e6-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="430e6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="430e6-130">Property</span></span>|<span data-ttu-id="430e6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="430e6-131">Type</span></span>|<span data-ttu-id="430e6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="430e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="430e6-133">id</span><span class="sxs-lookup"><span data-stu-id="430e6-133">id</span></span>|<span data-ttu-id="430e6-134">String</span><span class="sxs-lookup"><span data-stu-id="430e6-134">String</span></span>|<span data-ttu-id="430e6-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="430e6-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="430e6-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="430e6-136">System generated value assigned when created.</span></span> <span data-ttu-id="430e6-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="430e6-138">uniqueName</span></span>|<span data-ttu-id="430e6-139">String</span><span class="sxs-lookup"><span data-stu-id="430e6-139">String</span></span>|<span data-ttu-id="430e6-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="430e6-140">Unique name for the management condition.</span></span> <span data-ttu-id="430e6-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="430e6-141">Used in management condition expressions.</span></span> <span data-ttu-id="430e6-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="430e6-143">displayName</span></span>|<span data-ttu-id="430e6-144">String</span><span class="sxs-lookup"><span data-stu-id="430e6-144">String</span></span>|<span data-ttu-id="430e6-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="430e6-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="430e6-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-147">описание</span><span class="sxs-lookup"><span data-stu-id="430e6-147">description</span></span>|<span data-ttu-id="430e6-148">String</span><span class="sxs-lookup"><span data-stu-id="430e6-148">String</span></span>|<span data-ttu-id="430e6-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="430e6-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="430e6-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="430e6-151">createdDateTime</span></span>|<span data-ttu-id="430e6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430e6-152">DateTimeOffset</span></span>|<span data-ttu-id="430e6-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="430e6-153">The time the management condition was created.</span></span> <span data-ttu-id="430e6-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="430e6-154">Generated service side.</span></span> <span data-ttu-id="430e6-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="430e6-156">modifiedDateTime</span></span>|<span data-ttu-id="430e6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430e6-157">DateTimeOffset</span></span>|<span data-ttu-id="430e6-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="430e6-158">The time the management condition was last modified.</span></span> <span data-ttu-id="430e6-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="430e6-159">Updated service side.</span></span> <span data-ttu-id="430e6-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-161">eTag</span><span class="sxs-lookup"><span data-stu-id="430e6-161">eTag</span></span>|<span data-ttu-id="430e6-162">String</span><span class="sxs-lookup"><span data-stu-id="430e6-162">String</span></span>|<span data-ttu-id="430e6-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="430e6-163">ETag of the management condition.</span></span> <span data-ttu-id="430e6-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="430e6-164">Updated service side.</span></span> <span data-ttu-id="430e6-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="430e6-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="430e6-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="430e6-166">applicablePlatforms</span></span>|<span data-ttu-id="430e6-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="430e6-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="430e6-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="430e6-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="430e6-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="430e6-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="430e6-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="430e6-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="430e6-171">latitude</span><span class="sxs-lookup"><span data-stu-id="430e6-171">latitude</span></span>|<span data-ttu-id="430e6-172">Double</span><span class="sxs-lookup"><span data-stu-id="430e6-172">Double</span></span>|<span data-ttu-id="430e6-173">Широта в степени, от -90 до 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="430e6-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="430e6-174">longitude</span><span class="sxs-lookup"><span data-stu-id="430e6-174">longitude</span></span>|<span data-ttu-id="430e6-175">Double</span><span class="sxs-lookup"><span data-stu-id="430e6-175">Double</span></span>|<span data-ttu-id="430e6-176">Долгота в градусов между -180 и + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="430e6-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="430e6-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="430e6-177">radiusInMeters</span></span>|<span data-ttu-id="430e6-178">Single</span><span class="sxs-lookup"><span data-stu-id="430e6-178">Single</span></span>|<span data-ttu-id="430e6-179">RADIUS в метры.</span><span class="sxs-lookup"><span data-stu-id="430e6-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="430e6-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="430e6-180">Response</span></span>
<span data-ttu-id="430e6-181">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="430e6-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430e6-182">Пример</span><span class="sxs-lookup"><span data-stu-id="430e6-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="430e6-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="430e6-183">Request</span></span>
<span data-ttu-id="430e6-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="430e6-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="430e6-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="430e6-185">Response</span></span>
<span data-ttu-id="430e6-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="430e6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





