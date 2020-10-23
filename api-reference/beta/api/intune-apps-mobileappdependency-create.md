---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b4f0aad0a44385da92696cc5610eb2abc5a1acc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697170"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="0fad9-103">Создание Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="0fad9-103">Create mobileAppDependency</span></span>

<span data-ttu-id="0fad9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fad9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fad9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fad9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fad9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fad9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fad9-107">Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="0fad9-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fad9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0fad9-108">Prerequisites</span></span>
<span data-ttu-id="0fad9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fad9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fad9-111">Permission type</span></span>|<span data-ttu-id="0fad9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fad9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fad9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fad9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fad9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fad9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fad9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fad9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fad9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fad9-116">Not supported.</span></span>|
|<span data-ttu-id="0fad9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fad9-117">Application</span></span>|<span data-ttu-id="0fad9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fad9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fad9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fad9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="0fad9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0fad9-120">Request headers</span></span>
|<span data-ttu-id="0fad9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fad9-121">Header</span></span>|<span data-ttu-id="0fad9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0fad9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fad9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fad9-123">Authorization</span></span>|<span data-ttu-id="0fad9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fad9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fad9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0fad9-125">Accept</span></span>|<span data-ttu-id="0fad9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fad9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fad9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fad9-127">Request body</span></span>
<span data-ttu-id="0fad9-128">В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fad9-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="0fad9-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.</span><span class="sxs-lookup"><span data-stu-id="0fad9-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="0fad9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fad9-130">Property</span></span>|<span data-ttu-id="0fad9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0fad9-131">Type</span></span>|<span data-ttu-id="0fad9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0fad9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fad9-133">id</span><span class="sxs-lookup"><span data-stu-id="0fad9-133">id</span></span>|<span data-ttu-id="0fad9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0fad9-134">String</span></span>|<span data-ttu-id="0fad9-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="0fad9-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="0fad9-136">targetId</span><span class="sxs-lookup"><span data-stu-id="0fad9-136">targetId</span></span>|<span data-ttu-id="0fad9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0fad9-137">String</span></span>|<span data-ttu-id="0fad9-138">Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="0fad9-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="0fad9-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="0fad9-139">targetDisplayName</span></span>|<span data-ttu-id="0fad9-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0fad9-140">String</span></span>|<span data-ttu-id="0fad9-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0fad9-141">The target mobile app's display name.</span></span> <span data-ttu-id="0fad9-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="0fad9-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="0fad9-143">targetType</span><span class="sxs-lookup"><span data-stu-id="0fad9-143">targetType</span></span>|[<span data-ttu-id="0fad9-144">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="0fad9-144">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="0fad9-145">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="0fad9-145">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="0fad9-146">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="0fad9-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="0fad9-147">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="0fad9-147">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="0fad9-148">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="0fad9-148">dependencyType</span></span>|[<span data-ttu-id="0fad9-149">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="0fad9-149">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="0fad9-150">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="0fad9-150">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="0fad9-151">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="0fad9-151">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="0fad9-152">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="0fad9-152">dependentAppCount</span></span>|<span data-ttu-id="0fad9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0fad9-153">Int32</span></span>|<span data-ttu-id="0fad9-154">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="0fad9-154">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="0fad9-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fad9-155">Response</span></span>
<span data-ttu-id="0fad9-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fad9-156">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fad9-157">Пример</span><span class="sxs-lookup"><span data-stu-id="0fad9-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fad9-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fad9-158">Request</span></span>
<span data-ttu-id="0fad9-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fad9-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
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

### <a name="response"></a><span data-ttu-id="0fad9-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fad9-160">Response</span></span>
<span data-ttu-id="0fad9-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fad9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





