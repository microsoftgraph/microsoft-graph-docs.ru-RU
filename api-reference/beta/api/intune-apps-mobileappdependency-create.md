---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76bc270ef96a3342a5a6094b138068fb03bbc5cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444978"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="13dd1-103">Создание Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="13dd1-103">Create mobileAppDependency</span></span>

<span data-ttu-id="13dd1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13dd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13dd1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13dd1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13dd1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13dd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13dd1-107">Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="13dd1-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13dd1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13dd1-108">Prerequisites</span></span>
<span data-ttu-id="13dd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13dd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13dd1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13dd1-111">Permission type</span></span>|<span data-ttu-id="13dd1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13dd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13dd1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13dd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13dd1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13dd1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13dd1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13dd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13dd1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13dd1-116">Not supported.</span></span>|
|<span data-ttu-id="13dd1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13dd1-117">Application</span></span>|<span data-ttu-id="13dd1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13dd1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13dd1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13dd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="13dd1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13dd1-120">Request headers</span></span>
|<span data-ttu-id="13dd1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13dd1-121">Header</span></span>|<span data-ttu-id="13dd1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13dd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13dd1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13dd1-123">Authorization</span></span>|<span data-ttu-id="13dd1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13dd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13dd1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13dd1-125">Accept</span></span>|<span data-ttu-id="13dd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13dd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13dd1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13dd1-127">Request body</span></span>
<span data-ttu-id="13dd1-128">В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13dd1-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="13dd1-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.</span><span class="sxs-lookup"><span data-stu-id="13dd1-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="13dd1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13dd1-130">Property</span></span>|<span data-ttu-id="13dd1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13dd1-131">Type</span></span>|<span data-ttu-id="13dd1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13dd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13dd1-133">id</span><span class="sxs-lookup"><span data-stu-id="13dd1-133">id</span></span>|<span data-ttu-id="13dd1-134">String</span><span class="sxs-lookup"><span data-stu-id="13dd1-134">String</span></span>|<span data-ttu-id="13dd1-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="13dd1-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="13dd1-136">targetId</span><span class="sxs-lookup"><span data-stu-id="13dd1-136">targetId</span></span>|<span data-ttu-id="13dd1-137">String</span><span class="sxs-lookup"><span data-stu-id="13dd1-137">String</span></span>|<span data-ttu-id="13dd1-138">Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="13dd1-138">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="13dd1-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="13dd1-139">targetDisplayName</span></span>|<span data-ttu-id="13dd1-140">String</span><span class="sxs-lookup"><span data-stu-id="13dd1-140">String</span></span>|<span data-ttu-id="13dd1-141">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="13dd1-141">The target child mobile app's display name.</span></span> <span data-ttu-id="13dd1-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="13dd1-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="13dd1-143">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="13dd1-143">dependencyType</span></span>|[<span data-ttu-id="13dd1-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="13dd1-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="13dd1-145">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="13dd1-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="13dd1-146">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="13dd1-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="13dd1-147">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="13dd1-147">dependentAppCount</span></span>|<span data-ttu-id="13dd1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="13dd1-148">Int32</span></span>|<span data-ttu-id="13dd1-149">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="13dd1-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="13dd1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="13dd1-150">Response</span></span>
<span data-ttu-id="13dd1-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13dd1-151">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13dd1-152">Пример</span><span class="sxs-lookup"><span data-stu-id="13dd1-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="13dd1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="13dd1-153">Request</span></span>
<span data-ttu-id="13dd1-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13dd1-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13dd1-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="13dd1-155">Response</span></span>
<span data-ttu-id="13dd1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13dd1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





