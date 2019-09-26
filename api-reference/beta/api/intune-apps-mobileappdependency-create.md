---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 321fb11e5e1ee977facd0649c87ef0e46c717b59
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177082"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="04f33-103">Создание Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="04f33-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="04f33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04f33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04f33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04f33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f33-106">Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="04f33-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04f33-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04f33-107">Prerequisites</span></span>
<span data-ttu-id="04f33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04f33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04f33-110">Permission type</span></span>|<span data-ttu-id="04f33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04f33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04f33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04f33-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f33-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04f33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04f33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f33-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04f33-115">Not supported.</span></span>|
|<span data-ttu-id="04f33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04f33-116">Application</span></span>|<span data-ttu-id="04f33-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f33-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04f33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="04f33-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04f33-119">Request headers</span></span>
|<span data-ttu-id="04f33-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04f33-120">Header</span></span>|<span data-ttu-id="04f33-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04f33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f33-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04f33-122">Authorization</span></span>|<span data-ttu-id="04f33-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04f33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f33-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04f33-124">Accept</span></span>|<span data-ttu-id="04f33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04f33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f33-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04f33-126">Request body</span></span>
<span data-ttu-id="04f33-127">В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04f33-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="04f33-128">В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.</span><span class="sxs-lookup"><span data-stu-id="04f33-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="04f33-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="04f33-129">Property</span></span>|<span data-ttu-id="04f33-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04f33-130">Type</span></span>|<span data-ttu-id="04f33-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04f33-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f33-132">id</span><span class="sxs-lookup"><span data-stu-id="04f33-132">id</span></span>|<span data-ttu-id="04f33-133">String</span><span class="sxs-lookup"><span data-stu-id="04f33-133">String</span></span>|<span data-ttu-id="04f33-134">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="04f33-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="04f33-135">targetId</span><span class="sxs-lookup"><span data-stu-id="04f33-135">targetId</span></span>|<span data-ttu-id="04f33-136">String.</span><span class="sxs-lookup"><span data-stu-id="04f33-136">String</span></span>|<span data-ttu-id="04f33-137">Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="04f33-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="04f33-138">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="04f33-138">targetDisplayName</span></span>|<span data-ttu-id="04f33-139">String.</span><span class="sxs-lookup"><span data-stu-id="04f33-139">String</span></span>|<span data-ttu-id="04f33-140">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="04f33-140">The target child mobile app's display name.</span></span> <span data-ttu-id="04f33-141">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="04f33-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="04f33-142">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="04f33-142">dependencyType</span></span>|[<span data-ttu-id="04f33-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="04f33-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="04f33-144">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="04f33-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="04f33-145">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="04f33-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="04f33-146">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="04f33-146">dependentAppCount</span></span>|<span data-ttu-id="04f33-147">Int32</span><span class="sxs-lookup"><span data-stu-id="04f33-147">Int32</span></span>|<span data-ttu-id="04f33-148">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="04f33-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="04f33-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="04f33-149">Response</span></span>
<span data-ttu-id="04f33-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04f33-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f33-151">Пример</span><span class="sxs-lookup"><span data-stu-id="04f33-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="04f33-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="04f33-152">Request</span></span>
<span data-ttu-id="04f33-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04f33-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04f33-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="04f33-154">Response</span></span>
<span data-ttu-id="04f33-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04f33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




