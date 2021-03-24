---
title: Создание mobileAppSupersedence
description: Создание нового объекта mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02410619b871c00b92bfacd8df09ff221baff68e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143096"
---
# <a name="create-mobileappsupersedence"></a><span data-ttu-id="d5adc-103">Создание mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="d5adc-103">Create mobileAppSupersedence</span></span>

<span data-ttu-id="d5adc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5adc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5adc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5adc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5adc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5adc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5adc-107">Создание нового [объекта mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-107">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5adc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5adc-108">Prerequisites</span></span>
<span data-ttu-id="d5adc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5adc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5adc-111">Permission type</span></span>|<span data-ttu-id="d5adc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5adc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5adc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5adc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5adc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5adc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5adc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5adc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5adc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5adc-116">Not supported.</span></span>|
|<span data-ttu-id="d5adc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5adc-117">Application</span></span>|<span data-ttu-id="d5adc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5adc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5adc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5adc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="d5adc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5adc-120">Request headers</span></span>
|<span data-ttu-id="d5adc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5adc-121">Header</span></span>|<span data-ttu-id="d5adc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5adc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5adc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5adc-123">Authorization</span></span>|<span data-ttu-id="d5adc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5adc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5adc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5adc-125">Accept</span></span>|<span data-ttu-id="d5adc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5adc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5adc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5adc-127">Request body</span></span>
<span data-ttu-id="d5adc-128">В теле запроса поставляем представление JSON для объекта mobileAppSupersedence.</span><span class="sxs-lookup"><span data-stu-id="d5adc-128">In the request body, supply a JSON representation for the mobileAppSupersedence object.</span></span>

<span data-ttu-id="d5adc-129">В следующей таблице показаны свойства, необходимые при создании mobileAppSupersedence.</span><span class="sxs-lookup"><span data-stu-id="d5adc-129">The following table shows the properties that are required when you create the mobileAppSupersedence.</span></span>

|<span data-ttu-id="d5adc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5adc-130">Property</span></span>|<span data-ttu-id="d5adc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d5adc-131">Type</span></span>|<span data-ttu-id="d5adc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d5adc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5adc-133">id</span><span class="sxs-lookup"><span data-stu-id="d5adc-133">id</span></span>|<span data-ttu-id="d5adc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d5adc-134">String</span></span>|<span data-ttu-id="d5adc-135">ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d5adc-136">targetId</span><span class="sxs-lookup"><span data-stu-id="d5adc-136">targetId</span></span>|<span data-ttu-id="d5adc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d5adc-137">String</span></span>|<span data-ttu-id="d5adc-138">ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d5adc-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d5adc-139">targetDisplayName</span></span>|<span data-ttu-id="d5adc-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d5adc-140">String</span></span>|<span data-ttu-id="d5adc-141">Имя отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d5adc-141">The target mobile app's display name.</span></span> <span data-ttu-id="d5adc-142">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d5adc-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="d5adc-143">targetDisplayVersion</span></span>|<span data-ttu-id="d5adc-144">Строка</span><span class="sxs-lookup"><span data-stu-id="d5adc-144">String</span></span>|<span data-ttu-id="d5adc-145">Отображаемая версия целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d5adc-145">The target mobile app's display version.</span></span> <span data-ttu-id="d5adc-146">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d5adc-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="d5adc-147">targetPublisher</span></span>|<span data-ttu-id="d5adc-148">Строка</span><span class="sxs-lookup"><span data-stu-id="d5adc-148">String</span></span>|<span data-ttu-id="d5adc-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d5adc-149">The target mobile app's publisher.</span></span> <span data-ttu-id="d5adc-150">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d5adc-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d5adc-151">targetType</span><span class="sxs-lookup"><span data-stu-id="d5adc-151">targetType</span></span>|[<span data-ttu-id="d5adc-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="d5adc-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="d5adc-153">Тип отношений, указывающий, является ли цель родителем или ребенком.</span><span class="sxs-lookup"><span data-stu-id="d5adc-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="d5adc-154">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="d5adc-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="d5adc-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="d5adc-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="d5adc-156">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="d5adc-156">supersedenceType</span></span>|[<span data-ttu-id="d5adc-157">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="d5adc-157">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="d5adc-158">Тип отношения supersedence между родительскими и детскими приложениями.</span><span class="sxs-lookup"><span data-stu-id="d5adc-158">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="d5adc-159">Возможные значения: `update`, `replace`.</span><span class="sxs-lookup"><span data-stu-id="d5adc-159">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="d5adc-160">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="d5adc-160">supersededAppCount</span></span>|<span data-ttu-id="d5adc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d5adc-161">Int32</span></span>|<span data-ttu-id="d5adc-162">Общее количество приложений, прямо или косвенно выменимых детским приложением.</span><span class="sxs-lookup"><span data-stu-id="d5adc-162">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="d5adc-163">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="d5adc-163">supersedingAppCount</span></span>|<span data-ttu-id="d5adc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d5adc-164">Int32</span></span>|<span data-ttu-id="d5adc-165">Общее число приложений, прямо или косвенно выменив родительское приложение.</span><span class="sxs-lookup"><span data-stu-id="d5adc-165">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="d5adc-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5adc-166">Response</span></span>
<span data-ttu-id="d5adc-167">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d5adc-167">If successful, this method returns a `201 Created` response code and a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5adc-168">Пример</span><span class="sxs-lookup"><span data-stu-id="d5adc-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5adc-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5adc-169">Request</span></span>
<span data-ttu-id="d5adc-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5adc-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d5adc-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5adc-171">Response</span></span>
<span data-ttu-id="d5adc-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5adc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




