---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69ff12bb7c0d00457d86d62c467778de2a9223fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329182"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="4d72f-103">Создание Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="4d72f-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="4d72f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d72f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d72f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d72f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d72f-106">Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="4d72f-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d72f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d72f-107">Prerequisites</span></span>
<span data-ttu-id="4d72f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d72f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d72f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d72f-110">Permission type</span></span>|<span data-ttu-id="4d72f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d72f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d72f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d72f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d72f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d72f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d72f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d72f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d72f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d72f-115">Not supported.</span></span>|
|<span data-ttu-id="4d72f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d72f-116">Application</span></span>|<span data-ttu-id="4d72f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d72f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d72f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d72f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="4d72f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d72f-119">Request headers</span></span>
|<span data-ttu-id="4d72f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d72f-120">Header</span></span>|<span data-ttu-id="4d72f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4d72f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d72f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d72f-122">Authorization</span></span>|<span data-ttu-id="4d72f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d72f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d72f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4d72f-124">Accept</span></span>|<span data-ttu-id="4d72f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d72f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d72f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d72f-126">Request body</span></span>
<span data-ttu-id="4d72f-127">В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d72f-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="4d72f-128">В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.</span><span class="sxs-lookup"><span data-stu-id="4d72f-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="4d72f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d72f-129">Property</span></span>|<span data-ttu-id="4d72f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4d72f-130">Type</span></span>|<span data-ttu-id="4d72f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4d72f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d72f-132">id</span><span class="sxs-lookup"><span data-stu-id="4d72f-132">id</span></span>|<span data-ttu-id="4d72f-133">String</span><span class="sxs-lookup"><span data-stu-id="4d72f-133">String</span></span>|<span data-ttu-id="4d72f-134">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4d72f-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4d72f-135">targetId</span><span class="sxs-lookup"><span data-stu-id="4d72f-135">targetId</span></span>|<span data-ttu-id="4d72f-136">String</span><span class="sxs-lookup"><span data-stu-id="4d72f-136">String</span></span>|<span data-ttu-id="4d72f-137">Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4d72f-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4d72f-138">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="4d72f-138">targetDisplayName</span></span>|<span data-ttu-id="4d72f-139">String</span><span class="sxs-lookup"><span data-stu-id="4d72f-139">String</span></span>|<span data-ttu-id="4d72f-140">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4d72f-140">The target child mobile app's display name.</span></span> <span data-ttu-id="4d72f-141">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4d72f-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4d72f-142">депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="4d72f-142">dependencyType</span></span>|[<span data-ttu-id="4d72f-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="4d72f-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="4d72f-144">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="4d72f-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="4d72f-145">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="4d72f-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="4d72f-146">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4d72f-146">dependentAppCount</span></span>|<span data-ttu-id="4d72f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4d72f-147">Int32</span></span>|<span data-ttu-id="4d72f-148">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4d72f-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="4d72f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d72f-149">Response</span></span>
<span data-ttu-id="4d72f-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d72f-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d72f-151">Пример</span><span class="sxs-lookup"><span data-stu-id="4d72f-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d72f-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d72f-152">Request</span></span>
<span data-ttu-id="4d72f-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d72f-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d72f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d72f-154">Response</span></span>
<span data-ttu-id="4d72f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d72f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






