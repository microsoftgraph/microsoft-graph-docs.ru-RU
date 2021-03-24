---
title: Обновление mobileAppDependency
description: Обновление свойств объекта mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bf17e10744dd5f2795ac0d5b116bf54419674da
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139736"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="acafd-103">Обновление mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="acafd-103">Update mobileAppDependency</span></span>

<span data-ttu-id="acafd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acafd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acafd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acafd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acafd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acafd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acafd-107">Обновление свойств объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acafd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="acafd-108">Prerequisites</span></span>
<span data-ttu-id="acafd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acafd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acafd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acafd-111">Permission type</span></span>|<span data-ttu-id="acafd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acafd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acafd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acafd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acafd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acafd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="acafd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acafd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acafd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acafd-116">Not supported.</span></span>|
|<span data-ttu-id="acafd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="acafd-117">Application</span></span>|<span data-ttu-id="acafd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acafd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="acafd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acafd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="acafd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="acafd-120">Request headers</span></span>
|<span data-ttu-id="acafd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acafd-121">Header</span></span>|<span data-ttu-id="acafd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="acafd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acafd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acafd-123">Authorization</span></span>|<span data-ttu-id="acafd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acafd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acafd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acafd-125">Accept</span></span>|<span data-ttu-id="acafd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acafd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acafd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acafd-127">Request body</span></span>
<span data-ttu-id="acafd-128">В теле запроса поставляем представление JSON для [объекта mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="acafd-129">В следующей таблице показаны свойства, необходимые при создании [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="acafd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="acafd-130">Property</span></span>|<span data-ttu-id="acafd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="acafd-131">Type</span></span>|<span data-ttu-id="acafd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="acafd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acafd-133">id</span><span class="sxs-lookup"><span data-stu-id="acafd-133">id</span></span>|<span data-ttu-id="acafd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="acafd-134">String</span></span>|<span data-ttu-id="acafd-135">ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="acafd-136">targetId</span><span class="sxs-lookup"><span data-stu-id="acafd-136">targetId</span></span>|<span data-ttu-id="acafd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="acafd-137">String</span></span>|<span data-ttu-id="acafd-138">ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="acafd-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="acafd-139">targetDisplayName</span></span>|<span data-ttu-id="acafd-140">Строка</span><span class="sxs-lookup"><span data-stu-id="acafd-140">String</span></span>|<span data-ttu-id="acafd-141">Имя отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="acafd-141">The target mobile app's display name.</span></span> <span data-ttu-id="acafd-142">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="acafd-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="acafd-143">targetDisplayVersion</span></span>|<span data-ttu-id="acafd-144">Строка</span><span class="sxs-lookup"><span data-stu-id="acafd-144">String</span></span>|<span data-ttu-id="acafd-145">Отображаемая версия целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="acafd-145">The target mobile app's display version.</span></span> <span data-ttu-id="acafd-146">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="acafd-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="acafd-147">targetPublisher</span></span>|<span data-ttu-id="acafd-148">Строка</span><span class="sxs-lookup"><span data-stu-id="acafd-148">String</span></span>|<span data-ttu-id="acafd-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="acafd-149">The target mobile app's publisher.</span></span> <span data-ttu-id="acafd-150">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="acafd-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="acafd-151">targetType</span><span class="sxs-lookup"><span data-stu-id="acafd-151">targetType</span></span>|[<span data-ttu-id="acafd-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="acafd-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="acafd-153">Тип отношений, указывающий, является ли цель родителем или ребенком.</span><span class="sxs-lookup"><span data-stu-id="acafd-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="acafd-154">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="acafd-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="acafd-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="acafd-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="acafd-156">dependencyType</span><span class="sxs-lookup"><span data-stu-id="acafd-156">dependencyType</span></span>|[<span data-ttu-id="acafd-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="acafd-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="acafd-158">Тип зависимости между родительскими и детскими приложениями.</span><span class="sxs-lookup"><span data-stu-id="acafd-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="acafd-159">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="acafd-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="acafd-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="acafd-160">dependentAppCount</span></span>|<span data-ttu-id="acafd-161">Int32</span><span class="sxs-lookup"><span data-stu-id="acafd-161">Int32</span></span>|<span data-ttu-id="acafd-162">Общее число приложений, которые напрямую или косвенно зависят от родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="acafd-162">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="acafd-163">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="acafd-163">dependsOnAppCount</span></span>|<span data-ttu-id="acafd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="acafd-164">Int32</span></span>|<span data-ttu-id="acafd-165">Общее число приложений, от которых напрямую или косвенно зависит детское приложение.</span><span class="sxs-lookup"><span data-stu-id="acafd-165">The total number of apps the child app directly or indirectly depends on.</span></span>|



## <a name="response"></a><span data-ttu-id="acafd-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="acafd-166">Response</span></span>
<span data-ttu-id="acafd-167">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="acafd-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acafd-168">Пример</span><span class="sxs-lookup"><span data-stu-id="acafd-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="acafd-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="acafd-169">Request</span></span>
<span data-ttu-id="acafd-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acafd-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 372

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="acafd-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="acafd-171">Response</span></span>
<span data-ttu-id="acafd-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acafd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```




