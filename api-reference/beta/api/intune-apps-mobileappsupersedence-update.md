---
title: Обновление Мобилеаппсуперседенце
description: Обновление свойств объекта Мобилеаппсуперседенце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebc3bee8a610730d2d456bd3194268f5d57263ce
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247911"
---
# <a name="update-mobileappsupersedence"></a><span data-ttu-id="da950-103">Обновление Мобилеаппсуперседенце</span><span class="sxs-lookup"><span data-stu-id="da950-103">Update mobileAppSupersedence</span></span>

<span data-ttu-id="da950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da950-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da950-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da950-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da950-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da950-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da950-107">Обновление свойств объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="da950-107">Update the properties of a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da950-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="da950-108">Prerequisites</span></span>
<span data-ttu-id="da950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da950-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da950-111">Permission type</span></span>|<span data-ttu-id="da950-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da950-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da950-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da950-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da950-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da950-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da950-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da950-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da950-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da950-116">Not supported.</span></span>|
|<span data-ttu-id="da950-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="da950-117">Application</span></span>|<span data-ttu-id="da950-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da950-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da950-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da950-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="da950-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da950-120">Request headers</span></span>
|<span data-ttu-id="da950-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da950-121">Header</span></span>|<span data-ttu-id="da950-122">Значение</span><span class="sxs-lookup"><span data-stu-id="da950-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da950-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da950-123">Authorization</span></span>|<span data-ttu-id="da950-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da950-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da950-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da950-125">Accept</span></span>|<span data-ttu-id="da950-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da950-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da950-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da950-127">Request body</span></span>
<span data-ttu-id="da950-128">В тексте запроса добавьте представление объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da950-128">In the request body, supply a JSON representation for the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

<span data-ttu-id="da950-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md).</span><span class="sxs-lookup"><span data-stu-id="da950-129">The following table shows the properties that are required when you create the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>

|<span data-ttu-id="da950-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="da950-130">Property</span></span>|<span data-ttu-id="da950-131">Тип</span><span class="sxs-lookup"><span data-stu-id="da950-131">Type</span></span>|<span data-ttu-id="da950-132">Описание</span><span class="sxs-lookup"><span data-stu-id="da950-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da950-133">id</span><span class="sxs-lookup"><span data-stu-id="da950-133">id</span></span>|<span data-ttu-id="da950-134">String</span><span class="sxs-lookup"><span data-stu-id="da950-134">String</span></span>|<span data-ttu-id="da950-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="da950-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="da950-136">targetId</span><span class="sxs-lookup"><span data-stu-id="da950-136">targetId</span></span>|<span data-ttu-id="da950-137">String</span><span class="sxs-lookup"><span data-stu-id="da950-137">String</span></span>|<span data-ttu-id="da950-138">Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="da950-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="da950-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="da950-139">targetDisplayName</span></span>|<span data-ttu-id="da950-140">String</span><span class="sxs-lookup"><span data-stu-id="da950-140">String</span></span>|<span data-ttu-id="da950-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="da950-141">The target mobile app's display name.</span></span> <span data-ttu-id="da950-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="da950-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="da950-143">таржетдисплайверсион</span><span class="sxs-lookup"><span data-stu-id="da950-143">targetDisplayVersion</span></span>|<span data-ttu-id="da950-144">String</span><span class="sxs-lookup"><span data-stu-id="da950-144">String</span></span>|<span data-ttu-id="da950-145">Версия отображения целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="da950-145">The target mobile app's display version.</span></span> <span data-ttu-id="da950-146">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="da950-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="da950-147">таржетпублишер</span><span class="sxs-lookup"><span data-stu-id="da950-147">targetPublisher</span></span>|<span data-ttu-id="da950-148">String</span><span class="sxs-lookup"><span data-stu-id="da950-148">String</span></span>|<span data-ttu-id="da950-149">Издатель целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="da950-149">The target mobile app's publisher.</span></span> <span data-ttu-id="da950-150">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="da950-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="da950-151">targetType</span><span class="sxs-lookup"><span data-stu-id="da950-151">targetType</span></span>|[<span data-ttu-id="da950-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="da950-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="da950-153">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="da950-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="da950-154">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="da950-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="da950-155">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="da950-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="da950-156">суперседенцетипе</span><span class="sxs-lookup"><span data-stu-id="da950-156">supersedenceType</span></span>|[<span data-ttu-id="da950-157">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="da950-157">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="da950-158">Тип отношения замены между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="da950-158">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="da950-159">Возможные значения: `update`, `replace`.</span><span class="sxs-lookup"><span data-stu-id="da950-159">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="da950-160">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="da950-160">supersededAppCount</span></span>|<span data-ttu-id="da950-161">Int32</span><span class="sxs-lookup"><span data-stu-id="da950-161">Int32</span></span>|<span data-ttu-id="da950-162">Общее число приложений, напрямую или косвенно заменяющих дочерним приложением.</span><span class="sxs-lookup"><span data-stu-id="da950-162">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="da950-163">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="da950-163">supersedingAppCount</span></span>|<span data-ttu-id="da950-164">Int32</span><span class="sxs-lookup"><span data-stu-id="da950-164">Int32</span></span>|<span data-ttu-id="da950-165">Общее число приложений, напрямую или косвенно заменяющих родительское приложение.</span><span class="sxs-lookup"><span data-stu-id="da950-165">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="da950-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="da950-166">Response</span></span>
<span data-ttu-id="da950-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da950-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da950-168">Пример</span><span class="sxs-lookup"><span data-stu-id="da950-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="da950-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="da950-169">Request</span></span>
<span data-ttu-id="da950-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da950-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="da950-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="da950-171">Response</span></span>
<span data-ttu-id="da950-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da950-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




