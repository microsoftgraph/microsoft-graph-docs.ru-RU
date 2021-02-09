---
title: Обновление mobileAppDependency
description: Обновление свойств объекта mobileAppDependency.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45bb4504fc2d65a7d9284e15e73d6c5da575f881
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155316"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="e776f-103">Обновление mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="e776f-103">Update mobileAppDependency</span></span>

<span data-ttu-id="e776f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e776f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e776f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e776f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e776f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e776f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e776f-107">Обновление свойств объекта [mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e776f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e776f-108">Prerequisites</span></span>
<span data-ttu-id="e776f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e776f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e776f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e776f-111">Permission type</span></span>|<span data-ttu-id="e776f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e776f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e776f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e776f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e776f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e776f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e776f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e776f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e776f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e776f-116">Not supported.</span></span>|
|<span data-ttu-id="e776f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e776f-117">Application</span></span>|<span data-ttu-id="e776f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e776f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e776f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e776f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="e776f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e776f-120">Request headers</span></span>
|<span data-ttu-id="e776f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e776f-121">Header</span></span>|<span data-ttu-id="e776f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e776f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e776f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e776f-123">Authorization</span></span>|<span data-ttu-id="e776f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e776f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e776f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e776f-125">Accept</span></span>|<span data-ttu-id="e776f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e776f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e776f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e776f-127">Request body</span></span>
<span data-ttu-id="e776f-128">В теле запроса указав представление объекта [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="e776f-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="e776f-129">В следующей таблице показаны свойства, необходимые при создании [объекта mobileAppDependency.](../resources/intune-apps-mobileappdependency.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="e776f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e776f-130">Property</span></span>|<span data-ttu-id="e776f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e776f-131">Type</span></span>|<span data-ttu-id="e776f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e776f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e776f-133">id</span><span class="sxs-lookup"><span data-stu-id="e776f-133">id</span></span>|<span data-ttu-id="e776f-134">String</span><span class="sxs-lookup"><span data-stu-id="e776f-134">String</span></span>|<span data-ttu-id="e776f-135">ИД сущности отношения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e776f-136">targetId</span><span class="sxs-lookup"><span data-stu-id="e776f-136">targetId</span></span>|<span data-ttu-id="e776f-137">String</span><span class="sxs-lookup"><span data-stu-id="e776f-137">String</span></span>|<span data-ttu-id="e776f-138">ИД целевого мобильного приложения. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e776f-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="e776f-139">targetDisplayName</span></span>|<span data-ttu-id="e776f-140">String</span><span class="sxs-lookup"><span data-stu-id="e776f-140">String</span></span>|<span data-ttu-id="e776f-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e776f-141">The target mobile app's display name.</span></span> <span data-ttu-id="e776f-142">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e776f-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="e776f-143">targetDisplayVersion</span></span>|<span data-ttu-id="e776f-144">String</span><span class="sxs-lookup"><span data-stu-id="e776f-144">String</span></span>|<span data-ttu-id="e776f-145">Отображаемая версия целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e776f-145">The target mobile app's display version.</span></span> <span data-ttu-id="e776f-146">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e776f-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="e776f-147">targetPublisher</span></span>|<span data-ttu-id="e776f-148">String</span><span class="sxs-lookup"><span data-stu-id="e776f-148">String</span></span>|<span data-ttu-id="e776f-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e776f-149">The target mobile app's publisher.</span></span> <span data-ttu-id="e776f-150">Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="e776f-151">targetType</span><span class="sxs-lookup"><span data-stu-id="e776f-151">targetType</span></span>|[<span data-ttu-id="e776f-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="e776f-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="e776f-153">Тип связи, указывающий, является ли целевой объект родительским или родительским.</span><span class="sxs-lookup"><span data-stu-id="e776f-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="e776f-154">Наследуется [от mobileAppRelationship.](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="e776f-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="e776f-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="e776f-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="e776f-156">dependencyType</span><span class="sxs-lookup"><span data-stu-id="e776f-156">dependencyType</span></span>|[<span data-ttu-id="e776f-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="e776f-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="e776f-158">Тип отношения зависимостей между родительским и родительским приложениями.</span><span class="sxs-lookup"><span data-stu-id="e776f-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="e776f-159">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="e776f-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="e776f-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e776f-160">dependentAppCount</span></span>|<span data-ttu-id="e776f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e776f-161">Int32</span></span>|<span data-ttu-id="e776f-162">Общее количество приложений, которые напрямую или косвенно зависят от родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="e776f-162">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="e776f-163">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="e776f-163">dependsOnAppCount</span></span>|<span data-ttu-id="e776f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e776f-164">Int32</span></span>|<span data-ttu-id="e776f-165">Общее количество приложений, от которых непосредственно или косвенно зависит это приложение.</span><span class="sxs-lookup"><span data-stu-id="e776f-165">The total number of apps the child app directly or indirectly depends on.</span></span>|



## <a name="response"></a><span data-ttu-id="e776f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e776f-166">Response</span></span>
<span data-ttu-id="e776f-167">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e776f-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e776f-168">Пример</span><span class="sxs-lookup"><span data-stu-id="e776f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="e776f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="e776f-169">Request</span></span>
<span data-ttu-id="e776f-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e776f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e776f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="e776f-171">Response</span></span>
<span data-ttu-id="e776f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e776f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




