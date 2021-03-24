---
title: Создание mobileAppDependency
description: Создание нового объекта mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04ea3fcfd28ba39e9f8a1b99f3fd8d1ba5de35ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139757"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="22a00-103">Создание mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="22a00-103">Create mobileAppDependency</span></span>

<span data-ttu-id="22a00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a00-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22a00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a00-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22a00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a00-107">Создание нового [объекта mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a00-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22a00-108">Prerequisites</span></span>
<span data-ttu-id="22a00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a00-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22a00-111">Permission type</span></span>|<span data-ttu-id="22a00-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22a00-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a00-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22a00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a00-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a00-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22a00-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22a00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22a00-116">Not supported.</span></span>|
|<span data-ttu-id="22a00-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="22a00-117">Application</span></span>|<span data-ttu-id="22a00-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a00-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a00-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22a00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="22a00-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22a00-120">Request headers</span></span>
|<span data-ttu-id="22a00-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22a00-121">Header</span></span>|<span data-ttu-id="22a00-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22a00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a00-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a00-123">Authorization</span></span>|<span data-ttu-id="22a00-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22a00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a00-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22a00-125">Accept</span></span>|<span data-ttu-id="22a00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a00-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22a00-127">Request body</span></span>
<span data-ttu-id="22a00-128">В теле запроса поставляем представление JSON для объекта mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="22a00-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="22a00-129">В следующей таблице показаны свойства, необходимые при создании mobileAppDependency.</span><span class="sxs-lookup"><span data-stu-id="22a00-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="22a00-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22a00-130">Property</span></span>|<span data-ttu-id="22a00-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22a00-131">Type</span></span>|<span data-ttu-id="22a00-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22a00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a00-133">id</span><span class="sxs-lookup"><span data-stu-id="22a00-133">id</span></span>|<span data-ttu-id="22a00-134">Строка</span><span class="sxs-lookup"><span data-stu-id="22a00-134">String</span></span>|<span data-ttu-id="22a00-135">ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="22a00-136">targetId</span><span class="sxs-lookup"><span data-stu-id="22a00-136">targetId</span></span>|<span data-ttu-id="22a00-137">Строка</span><span class="sxs-lookup"><span data-stu-id="22a00-137">String</span></span>|<span data-ttu-id="22a00-138">ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="22a00-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="22a00-139">targetDisplayName</span></span>|<span data-ttu-id="22a00-140">Строка</span><span class="sxs-lookup"><span data-stu-id="22a00-140">String</span></span>|<span data-ttu-id="22a00-141">Имя отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22a00-141">The target mobile app's display name.</span></span> <span data-ttu-id="22a00-142">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="22a00-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="22a00-143">targetDisplayVersion</span></span>|<span data-ttu-id="22a00-144">Строка</span><span class="sxs-lookup"><span data-stu-id="22a00-144">String</span></span>|<span data-ttu-id="22a00-145">Отображаемая версия целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22a00-145">The target mobile app's display version.</span></span> <span data-ttu-id="22a00-146">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="22a00-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="22a00-147">targetPublisher</span></span>|<span data-ttu-id="22a00-148">Строка</span><span class="sxs-lookup"><span data-stu-id="22a00-148">String</span></span>|<span data-ttu-id="22a00-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22a00-149">The target mobile app's publisher.</span></span> <span data-ttu-id="22a00-150">Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22a00-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="22a00-151">targetType</span><span class="sxs-lookup"><span data-stu-id="22a00-151">targetType</span></span>|[<span data-ttu-id="22a00-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="22a00-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="22a00-153">Тип отношений, указывающий, является ли цель родителем или ребенком.</span><span class="sxs-lookup"><span data-stu-id="22a00-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="22a00-154">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="22a00-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="22a00-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="22a00-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="22a00-156">dependencyType</span><span class="sxs-lookup"><span data-stu-id="22a00-156">dependencyType</span></span>|[<span data-ttu-id="22a00-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="22a00-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="22a00-158">Тип зависимости между родительскими и детскими приложениями.</span><span class="sxs-lookup"><span data-stu-id="22a00-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="22a00-159">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="22a00-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="22a00-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="22a00-160">dependentAppCount</span></span>|<span data-ttu-id="22a00-161">Int32</span><span class="sxs-lookup"><span data-stu-id="22a00-161">Int32</span></span>|<span data-ttu-id="22a00-162">Общее число приложений, которые напрямую или косвенно зависят от родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="22a00-162">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="22a00-163">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="22a00-163">dependsOnAppCount</span></span>|<span data-ttu-id="22a00-164">Int32</span><span class="sxs-lookup"><span data-stu-id="22a00-164">Int32</span></span>|<span data-ttu-id="22a00-165">Общее число приложений, от которых напрямую или косвенно зависит детское приложение.</span><span class="sxs-lookup"><span data-stu-id="22a00-165">The total number of apps the child app directly or indirectly depends on.</span></span>|



## <a name="response"></a><span data-ttu-id="22a00-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a00-166">Response</span></span>
<span data-ttu-id="22a00-167">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект mobileAppDependency](../resources/intune-apps-mobileappdependency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="22a00-167">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a00-168">Пример</span><span class="sxs-lookup"><span data-stu-id="22a00-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a00-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="22a00-169">Request</span></span>
<span data-ttu-id="22a00-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22a00-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
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

### <a name="response"></a><span data-ttu-id="22a00-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a00-171">Response</span></span>
<span data-ttu-id="22a00-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22a00-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




