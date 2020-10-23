---
title: Обновление Мобилеаппдепенденци
description: Обновление свойств объекта Мобилеаппдепенденци.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3844d0019a7981509dfbb2a4544f00a61d4575c3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722790"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="95d1d-103">Обновление Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="95d1d-103">Update mobileAppDependency</span></span>

<span data-ttu-id="95d1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95d1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95d1d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95d1d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95d1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95d1d-107">Обновление свойств объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="95d1d-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95d1d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95d1d-108">Prerequisites</span></span>
<span data-ttu-id="95d1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d1d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d1d-111">Permission type</span></span>|<span data-ttu-id="95d1d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d1d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95d1d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d1d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95d1d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d1d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95d1d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d1d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95d1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d1d-116">Not supported.</span></span>|
|<span data-ttu-id="95d1d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95d1d-117">Application</span></span>|<span data-ttu-id="95d1d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d1d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95d1d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d1d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="95d1d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95d1d-120">Request headers</span></span>
|<span data-ttu-id="95d1d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95d1d-121">Header</span></span>|<span data-ttu-id="95d1d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95d1d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95d1d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d1d-123">Authorization</span></span>|<span data-ttu-id="95d1d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d1d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95d1d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95d1d-125">Accept</span></span>|<span data-ttu-id="95d1d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95d1d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95d1d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95d1d-127">Request body</span></span>
<span data-ttu-id="95d1d-128">В тексте запроса добавьте представление объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95d1d-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="95d1d-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="95d1d-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="95d1d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95d1d-130">Property</span></span>|<span data-ttu-id="95d1d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95d1d-131">Type</span></span>|<span data-ttu-id="95d1d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95d1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95d1d-133">id</span><span class="sxs-lookup"><span data-stu-id="95d1d-133">id</span></span>|<span data-ttu-id="95d1d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="95d1d-134">String</span></span>|<span data-ttu-id="95d1d-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="95d1d-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="95d1d-136">targetId</span><span class="sxs-lookup"><span data-stu-id="95d1d-136">targetId</span></span>|<span data-ttu-id="95d1d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="95d1d-137">String</span></span>|<span data-ttu-id="95d1d-138">Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="95d1d-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="95d1d-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="95d1d-139">targetDisplayName</span></span>|<span data-ttu-id="95d1d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="95d1d-140">String</span></span>|<span data-ttu-id="95d1d-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="95d1d-141">The target mobile app's display name.</span></span> <span data-ttu-id="95d1d-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="95d1d-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="95d1d-143">targetType</span><span class="sxs-lookup"><span data-stu-id="95d1d-143">targetType</span></span>|[<span data-ttu-id="95d1d-144">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="95d1d-144">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="95d1d-145">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="95d1d-145">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="95d1d-146">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="95d1d-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="95d1d-147">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="95d1d-147">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="95d1d-148">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="95d1d-148">dependencyType</span></span>|[<span data-ttu-id="95d1d-149">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="95d1d-149">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="95d1d-150">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="95d1d-150">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="95d1d-151">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="95d1d-151">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="95d1d-152">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="95d1d-152">dependentAppCount</span></span>|<span data-ttu-id="95d1d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="95d1d-153">Int32</span></span>|<span data-ttu-id="95d1d-154">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="95d1d-154">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="95d1d-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="95d1d-155">Response</span></span>
<span data-ttu-id="95d1d-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95d1d-156">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95d1d-157">Пример</span><span class="sxs-lookup"><span data-stu-id="95d1d-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="95d1d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d1d-158">Request</span></span>
<span data-ttu-id="95d1d-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95d1d-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="95d1d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d1d-160">Response</span></span>
<span data-ttu-id="95d1d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95d1d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```





