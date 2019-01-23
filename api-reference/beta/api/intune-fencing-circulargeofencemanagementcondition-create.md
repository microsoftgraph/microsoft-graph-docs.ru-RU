---
title: Создание circularGeofenceManagementCondition
description: Создание нового объекта circularGeofenceManagementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7009bfe8ef72072aa00c0d430406f550ece83212
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417618"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="3548e-103">Создание circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="3548e-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="3548e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3548e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3548e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3548e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3548e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3548e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3548e-107">Создание нового объекта [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="3548e-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3548e-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3548e-108">Prerequisites</span></span>
<span data-ttu-id="3548e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3548e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3548e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3548e-111">Permission type</span></span>|<span data-ttu-id="3548e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3548e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3548e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3548e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3548e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3548e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3548e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3548e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3548e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3548e-116">Not supported.</span></span>|
|<span data-ttu-id="3548e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3548e-117">Application</span></span>|<span data-ttu-id="3548e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3548e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3548e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3548e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="3548e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3548e-120">Request headers</span></span>
|<span data-ttu-id="3548e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3548e-121">Header</span></span>|<span data-ttu-id="3548e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3548e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3548e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3548e-123">Authorization</span></span>|<span data-ttu-id="3548e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3548e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3548e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3548e-125">Accept</span></span>|<span data-ttu-id="3548e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3548e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3548e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3548e-127">Request body</span></span>
<span data-ttu-id="3548e-128">В тексте запроса укажите представление JSON для объекта circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="3548e-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="3548e-129">В следующей таблице показаны свойства, которые необходимы для создания circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="3548e-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="3548e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3548e-130">Property</span></span>|<span data-ttu-id="3548e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3548e-131">Type</span></span>|<span data-ttu-id="3548e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3548e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3548e-133">id</span><span class="sxs-lookup"><span data-stu-id="3548e-133">id</span></span>|<span data-ttu-id="3548e-134">String</span><span class="sxs-lookup"><span data-stu-id="3548e-134">String</span></span>|<span data-ttu-id="3548e-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="3548e-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="3548e-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="3548e-136">System generated value assigned when created.</span></span> <span data-ttu-id="3548e-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="3548e-138">uniqueName</span></span>|<span data-ttu-id="3548e-139">String</span><span class="sxs-lookup"><span data-stu-id="3548e-139">String</span></span>|<span data-ttu-id="3548e-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="3548e-140">Unique name for the management condition.</span></span> <span data-ttu-id="3548e-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="3548e-141">Used in management condition expressions.</span></span> <span data-ttu-id="3548e-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3548e-143">displayName</span></span>|<span data-ttu-id="3548e-144">String</span><span class="sxs-lookup"><span data-stu-id="3548e-144">String</span></span>|<span data-ttu-id="3548e-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="3548e-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="3548e-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-147">description</span><span class="sxs-lookup"><span data-stu-id="3548e-147">description</span></span>|<span data-ttu-id="3548e-148">String</span><span class="sxs-lookup"><span data-stu-id="3548e-148">String</span></span>|<span data-ttu-id="3548e-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="3548e-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="3548e-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3548e-151">createdDateTime</span></span>|<span data-ttu-id="3548e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3548e-152">DateTimeOffset</span></span>|<span data-ttu-id="3548e-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="3548e-153">The time the management condition was created.</span></span> <span data-ttu-id="3548e-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="3548e-154">Generated service side.</span></span> <span data-ttu-id="3548e-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3548e-156">modifiedDateTime</span></span>|<span data-ttu-id="3548e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3548e-157">DateTimeOffset</span></span>|<span data-ttu-id="3548e-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="3548e-158">The time the management condition was last modified.</span></span> <span data-ttu-id="3548e-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="3548e-159">Updated service side.</span></span> <span data-ttu-id="3548e-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-161">eTag</span><span class="sxs-lookup"><span data-stu-id="3548e-161">eTag</span></span>|<span data-ttu-id="3548e-162">String</span><span class="sxs-lookup"><span data-stu-id="3548e-162">String</span></span>|<span data-ttu-id="3548e-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="3548e-163">ETag of the management condition.</span></span> <span data-ttu-id="3548e-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="3548e-164">Updated service side.</span></span> <span data-ttu-id="3548e-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3548e-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3548e-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="3548e-166">applicablePlatforms</span></span>|<span data-ttu-id="3548e-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3548e-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="3548e-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="3548e-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="3548e-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="3548e-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="3548e-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="3548e-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="3548e-171">latitude</span><span class="sxs-lookup"><span data-stu-id="3548e-171">latitude</span></span>|<span data-ttu-id="3548e-172">Double</span><span class="sxs-lookup"><span data-stu-id="3548e-172">Double</span></span>|<span data-ttu-id="3548e-173">Широта в степени, от -90 до 90 включительно.</span><span class="sxs-lookup"><span data-stu-id="3548e-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="3548e-174">longitude</span><span class="sxs-lookup"><span data-stu-id="3548e-174">longitude</span></span>|<span data-ttu-id="3548e-175">Double</span><span class="sxs-lookup"><span data-stu-id="3548e-175">Double</span></span>|<span data-ttu-id="3548e-176">Долгота в градусов между -180 и + 180 включительно.</span><span class="sxs-lookup"><span data-stu-id="3548e-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="3548e-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="3548e-177">radiusInMeters</span></span>|<span data-ttu-id="3548e-178">Single</span><span class="sxs-lookup"><span data-stu-id="3548e-178">Single</span></span>|<span data-ttu-id="3548e-179">RADIUS в метры.</span><span class="sxs-lookup"><span data-stu-id="3548e-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="3548e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="3548e-180">Response</span></span>
<span data-ttu-id="3548e-181">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3548e-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3548e-182">Пример</span><span class="sxs-lookup"><span data-stu-id="3548e-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="3548e-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="3548e-183">Request</span></span>
<span data-ttu-id="3548e-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3548e-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3548e-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="3548e-185">Response</span></span>
<span data-ttu-id="3548e-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3548e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




