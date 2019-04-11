---
title: Обновление Мобилеаппдепенденци
description: Обновление свойств объекта Мобилеаппдепенденци.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8648fb92953ef8ece7be672e746bffbb63393859
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808989"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="f81af-103">Обновление Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="f81af-103">Update mobileAppDependency</span></span>

> <span data-ttu-id="f81af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f81af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f81af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f81af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f81af-106">Обновление свойств объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .</span><span class="sxs-lookup"><span data-stu-id="f81af-106">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f81af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f81af-107">Prerequisites</span></span>
<span data-ttu-id="f81af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f81af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f81af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f81af-110">Permission type</span></span>|<span data-ttu-id="f81af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f81af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f81af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f81af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f81af-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81af-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f81af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f81af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f81af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f81af-115">Not supported.</span></span>|
|<span data-ttu-id="f81af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f81af-116">Application</span></span>|<span data-ttu-id="f81af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f81af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f81af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f81af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="f81af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f81af-119">Request headers</span></span>
|<span data-ttu-id="f81af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f81af-120">Header</span></span>|<span data-ttu-id="f81af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f81af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f81af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f81af-122">Authorization</span></span>|<span data-ttu-id="f81af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f81af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f81af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f81af-124">Accept</span></span>|<span data-ttu-id="f81af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f81af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f81af-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f81af-126">Request body</span></span>
<span data-ttu-id="f81af-127">В тексте запроса добавьте представление объекта [Мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f81af-127">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="f81af-128">В следующей таблице приведены свойства, необходимые при создании [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="f81af-128">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="f81af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f81af-129">Property</span></span>|<span data-ttu-id="f81af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f81af-130">Type</span></span>|<span data-ttu-id="f81af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f81af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f81af-132">id</span><span class="sxs-lookup"><span data-stu-id="f81af-132">id</span></span>|<span data-ttu-id="f81af-133">String</span><span class="sxs-lookup"><span data-stu-id="f81af-133">String</span></span>|<span data-ttu-id="f81af-134">Идентификатор сущности отношения. НаСледуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="f81af-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="f81af-135">targetId</span><span class="sxs-lookup"><span data-stu-id="f81af-135">targetId</span></span>|<span data-ttu-id="f81af-136">String</span><span class="sxs-lookup"><span data-stu-id="f81af-136">String</span></span>|<span data-ttu-id="f81af-137">Идентификатор приложения целевого дочернего мобильного приложения. НаСледуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="f81af-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="f81af-138">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="f81af-138">targetDisplayName</span></span>|<span data-ttu-id="f81af-139">String</span><span class="sxs-lookup"><span data-stu-id="f81af-139">String</span></span>|<span data-ttu-id="f81af-140">Отображаемое имя целевого дочернего мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f81af-140">The target child mobile app's display name.</span></span> <span data-ttu-id="f81af-141">НаСледуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="f81af-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="f81af-142">Депенденцитипе</span><span class="sxs-lookup"><span data-stu-id="f81af-142">dependencyType</span></span>|[<span data-ttu-id="f81af-143">Мобилеаппдепендецитипе</span><span class="sxs-lookup"><span data-stu-id="f81af-143">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="f81af-144">Тип отношения зависимости между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="f81af-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="f81af-145">Возможные значения: `detect`, `autoInstall`.</span><span class="sxs-lookup"><span data-stu-id="f81af-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="f81af-146">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f81af-146">dependentAppCount</span></span>|<span data-ttu-id="f81af-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f81af-147">Int32</span></span>|<span data-ttu-id="f81af-148">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="f81af-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="f81af-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f81af-149">Response</span></span>
<span data-ttu-id="f81af-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f81af-150">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f81af-151">Пример</span><span class="sxs-lookup"><span data-stu-id="f81af-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="f81af-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="f81af-152">Request</span></span>
<span data-ttu-id="f81af-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f81af-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
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

### <a name="response"></a><span data-ttu-id="f81af-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f81af-154">Response</span></span>
<span data-ttu-id="f81af-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f81af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





