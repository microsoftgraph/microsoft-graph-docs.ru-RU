---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16931384fb343c21b4d6f8c64c19464411ecde1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43415372"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="cf53b-103">Создание Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="cf53b-103">Create mobileAppDependency</span></span>

<span data-ttu-id="cf53b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf53b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf53b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf53b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf53b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf53b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf53b-107">Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="cf53b-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf53b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf53b-108">Prerequisites</span></span>
<span data-ttu-id="cf53b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf53b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf53b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf53b-111">Permission type</span></span>|<span data-ttu-id="cf53b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf53b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf53b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf53b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf53b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf53b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf53b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf53b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf53b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf53b-116">Not supported.</span></span>|
|<span data-ttu-id="cf53b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf53b-117">Application</span></span>|<span data-ttu-id="cf53b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf53b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf53b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf53b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="cf53b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf53b-120">Request headers</span></span>
|<span data-ttu-id="cf53b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf53b-121">Header</span></span>|<span data-ttu-id="cf53b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf53b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf53b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf53b-123">Authorization</span></span>|<span data-ttu-id="cf53b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf53b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf53b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf53b-125">Accept</span></span>|<span data-ttu-id="cf53b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf53b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf53b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf53b-127">Request body</span></span>
<span data-ttu-id="cf53b-128">В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf53b-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="cf53b-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.</span><span class="sxs-lookup"><span data-stu-id="cf53b-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="cf53b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf53b-130">Property</span></span>|<span data-ttu-id="cf53b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf53b-131">Type</span></span>|<span data-ttu-id="cf53b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf53b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf53b-133">id</span><span class="sxs-lookup"><span data-stu-id="cf53b-133">id</span></span>|<span data-ttu-id="cf53b-134">String</span><span class="sxs-lookup"><span data-stu-id="cf53b-134">String</span></span>|<span data-ttu-id="cf53b-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="cf53b-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="cf53b-136">targetId</span><span class="sxs-lookup"><span data-stu-id="cf53b-136">targetId</span></span>|<span data-ttu-id="cf53b-137">String</span><span class="sxs-lookup"><span data-stu-id="cf53b-137">String</span></span>|<span data-ttu-id="cf53b-138">Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="cf53b-138">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="cf53b-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="cf53b-139">targetDisplayName</span></span>|<span data-ttu-id="cf53b-140">String</span><span class="sxs-lookup"><span data-stu-id="cf53b-140">String</span></span>|<span data-ttu-id="cf53b-141">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cf53b-141">The target child mobile app's display name.</span></span> <span data-ttu-id="cf53b-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="cf53b-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="cf53b-143">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="cf53b-143">dependencyType</span></span>|[<span data-ttu-id="cf53b-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="cf53b-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="cf53b-145">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="cf53b-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="cf53b-146">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="cf53b-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="cf53b-147">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="cf53b-147">dependentAppCount</span></span>|<span data-ttu-id="cf53b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cf53b-148">Int32</span></span>|<span data-ttu-id="cf53b-149">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="cf53b-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="cf53b-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf53b-150">Response</span></span>
<span data-ttu-id="cf53b-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf53b-151">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf53b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="cf53b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf53b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf53b-153">Request</span></span>
<span data-ttu-id="cf53b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf53b-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="cf53b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf53b-155">Response</span></span>
<span data-ttu-id="cf53b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf53b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```



