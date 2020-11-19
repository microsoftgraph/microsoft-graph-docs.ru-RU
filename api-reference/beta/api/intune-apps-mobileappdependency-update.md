---
title: Обновление Мобилеаппдепенденци
description: Обновление свойств объекта Мобилеаппдепенденци.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9803ce18f0d6dd821573461d88d3bf258fd82a91
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248429"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="62fb8-103">Обновление Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="62fb8-103">Update mobileAppDependency</span></span>

<span data-ttu-id="62fb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62fb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62fb8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62fb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62fb8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62fb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62fb8-107">Обновление свойств объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="62fb8-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62fb8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="62fb8-108">Prerequisites</span></span>
<span data-ttu-id="62fb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62fb8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62fb8-111">Permission type</span></span>|<span data-ttu-id="62fb8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62fb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62fb8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62fb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62fb8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fb8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62fb8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62fb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62fb8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62fb8-116">Not supported.</span></span>|
|<span data-ttu-id="62fb8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="62fb8-117">Application</span></span>|<span data-ttu-id="62fb8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fb8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62fb8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62fb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="62fb8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62fb8-120">Request headers</span></span>
|<span data-ttu-id="62fb8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62fb8-121">Header</span></span>|<span data-ttu-id="62fb8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62fb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62fb8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62fb8-123">Authorization</span></span>|<span data-ttu-id="62fb8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62fb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62fb8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62fb8-125">Accept</span></span>|<span data-ttu-id="62fb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62fb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62fb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62fb8-127">Request body</span></span>
<span data-ttu-id="62fb8-128">В тексте запроса добавьте представление объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62fb8-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="62fb8-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="62fb8-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="62fb8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62fb8-130">Property</span></span>|<span data-ttu-id="62fb8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62fb8-131">Type</span></span>|<span data-ttu-id="62fb8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62fb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62fb8-133">id</span><span class="sxs-lookup"><span data-stu-id="62fb8-133">id</span></span>|<span data-ttu-id="62fb8-134">String</span><span class="sxs-lookup"><span data-stu-id="62fb8-134">String</span></span>|<span data-ttu-id="62fb8-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="62fb8-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="62fb8-136">targetId</span><span class="sxs-lookup"><span data-stu-id="62fb8-136">targetId</span></span>|<span data-ttu-id="62fb8-137">String</span><span class="sxs-lookup"><span data-stu-id="62fb8-137">String</span></span>|<span data-ttu-id="62fb8-138">Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="62fb8-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="62fb8-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="62fb8-139">targetDisplayName</span></span>|<span data-ttu-id="62fb8-140">String</span><span class="sxs-lookup"><span data-stu-id="62fb8-140">String</span></span>|<span data-ttu-id="62fb8-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="62fb8-141">The target mobile app's display name.</span></span> <span data-ttu-id="62fb8-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="62fb8-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="62fb8-143">таржетдисплайверсион</span><span class="sxs-lookup"><span data-stu-id="62fb8-143">targetDisplayVersion</span></span>|<span data-ttu-id="62fb8-144">String</span><span class="sxs-lookup"><span data-stu-id="62fb8-144">String</span></span>|<span data-ttu-id="62fb8-145">Версия отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="62fb8-145">The target mobile app's display version.</span></span> <span data-ttu-id="62fb8-146">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="62fb8-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="62fb8-147">таржетпублишер</span><span class="sxs-lookup"><span data-stu-id="62fb8-147">targetPublisher</span></span>|<span data-ttu-id="62fb8-148">String</span><span class="sxs-lookup"><span data-stu-id="62fb8-148">String</span></span>|<span data-ttu-id="62fb8-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="62fb8-149">The target mobile app's publisher.</span></span> <span data-ttu-id="62fb8-150">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="62fb8-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="62fb8-151">targetType</span><span class="sxs-lookup"><span data-stu-id="62fb8-151">targetType</span></span>|[<span data-ttu-id="62fb8-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="62fb8-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="62fb8-153">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="62fb8-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="62fb8-154">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="62fb8-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="62fb8-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="62fb8-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="62fb8-156">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="62fb8-156">dependencyType</span></span>|[<span data-ttu-id="62fb8-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="62fb8-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="62fb8-158">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="62fb8-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="62fb8-159">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="62fb8-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="62fb8-160">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="62fb8-160">dependentAppCount</span></span>|<span data-ttu-id="62fb8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="62fb8-161">Int32</span></span>|<span data-ttu-id="62fb8-162">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="62fb8-162">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="62fb8-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="62fb8-163">Response</span></span>
<span data-ttu-id="62fb8-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62fb8-164">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62fb8-165">Пример</span><span class="sxs-lookup"><span data-stu-id="62fb8-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="62fb8-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="62fb8-166">Request</span></span>
<span data-ttu-id="62fb8-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62fb8-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="62fb8-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="62fb8-168">Response</span></span>
<span data-ttu-id="62fb8-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62fb8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```




