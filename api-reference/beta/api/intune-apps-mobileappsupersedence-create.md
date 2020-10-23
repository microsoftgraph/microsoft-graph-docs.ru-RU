---
title: Создание Мобилеаппсуперседенце
description: Создание нового объекта Мобилеаппсуперседенце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 532bdb70977053389aed2be0b0df5c8c9eb4c932
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702203"
---
# <a name="create-mobileappsupersedence"></a><span data-ttu-id="a6cd1-103">Создание Мобилеаппсуперседенце</span><span class="sxs-lookup"><span data-stu-id="a6cd1-103">Create mobileAppSupersedence</span></span>

<span data-ttu-id="a6cd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6cd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6cd1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6cd1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6cd1-107">Создание нового объекта [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) .</span><span class="sxs-lookup"><span data-stu-id="a6cd1-107">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6cd1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6cd1-108">Prerequisites</span></span>
<span data-ttu-id="a6cd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6cd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6cd1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6cd1-111">Permission type</span></span>|<span data-ttu-id="a6cd1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6cd1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6cd1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6cd1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6cd1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6cd1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-116">Not supported.</span></span>|
|<span data-ttu-id="a6cd1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6cd1-117">Application</span></span>|<span data-ttu-id="a6cd1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6cd1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6cd1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6cd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="a6cd1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6cd1-120">Request headers</span></span>
|<span data-ttu-id="a6cd1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6cd1-121">Header</span></span>|<span data-ttu-id="a6cd1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a6cd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6cd1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6cd1-123">Authorization</span></span>|<span data-ttu-id="a6cd1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6cd1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6cd1-125">Accept</span></span>|<span data-ttu-id="a6cd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6cd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6cd1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6cd1-127">Request body</span></span>
<span data-ttu-id="a6cd1-128">В тексте запроса добавьте представление объекта Мобилеаппсуперседенце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-128">In the request body, supply a JSON representation for the mobileAppSupersedence object.</span></span>

<span data-ttu-id="a6cd1-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппсуперседенце.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-129">The following table shows the properties that are required when you create the mobileAppSupersedence.</span></span>

|<span data-ttu-id="a6cd1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6cd1-130">Property</span></span>|<span data-ttu-id="a6cd1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6cd1-131">Type</span></span>|<span data-ttu-id="a6cd1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6cd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6cd1-133">id</span><span class="sxs-lookup"><span data-stu-id="a6cd1-133">id</span></span>|<span data-ttu-id="a6cd1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a6cd1-134">String</span></span>|<span data-ttu-id="a6cd1-135">Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="a6cd1-136">targetId</span><span class="sxs-lookup"><span data-stu-id="a6cd1-136">targetId</span></span>|<span data-ttu-id="a6cd1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a6cd1-137">String</span></span>|<span data-ttu-id="a6cd1-138">Идентификатор приложения целевого приложения для мобильных устройств. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="a6cd1-139">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="a6cd1-139">targetDisplayName</span></span>|<span data-ttu-id="a6cd1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a6cd1-140">String</span></span>|<span data-ttu-id="a6cd1-141">Отображаемое имя целевого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-141">The target mobile app's display name.</span></span> <span data-ttu-id="a6cd1-142">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="a6cd1-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="a6cd1-143">targetType</span><span class="sxs-lookup"><span data-stu-id="a6cd1-143">targetType</span></span>|[<span data-ttu-id="a6cd1-144">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="a6cd1-144">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="a6cd1-145">Тип связи, указывающий, является ли целевой объект родительским или дочерним.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-145">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="a6cd1-146">Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md).</span><span class="sxs-lookup"><span data-stu-id="a6cd1-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="a6cd1-147">Возможные значения: `child`, `parent`.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-147">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="a6cd1-148">суперседенцетипе</span><span class="sxs-lookup"><span data-stu-id="a6cd1-148">supersedenceType</span></span>|[<span data-ttu-id="a6cd1-149">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="a6cd1-149">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="a6cd1-150">Тип отношения замены между родительским и дочерним приложениями.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-150">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="a6cd1-151">Возможные значения: `update`, `replace`.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-151">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="a6cd1-152">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a6cd1-152">supersededAppCount</span></span>|<span data-ttu-id="a6cd1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6cd1-153">Int32</span></span>|<span data-ttu-id="a6cd1-154">Общее число приложений, напрямую или косвенно заменяющих дочерним приложением.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-154">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="a6cd1-155">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a6cd1-155">supersedingAppCount</span></span>|<span data-ttu-id="a6cd1-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a6cd1-156">Int32</span></span>|<span data-ttu-id="a6cd1-157">Общее число приложений, напрямую или косвенно заменяющих родительское приложение.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-157">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="a6cd1-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6cd1-158">Response</span></span>
<span data-ttu-id="a6cd1-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппсуперседенце](../resources/intune-apps-mobileappsupersedence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-159">If successful, this method returns a `201 Created` response code and a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6cd1-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a6cd1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6cd1-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6cd1-161">Request</span></span>
<span data-ttu-id="a6cd1-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="a6cd1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6cd1-163">Response</span></span>
<span data-ttu-id="a6cd1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6cd1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```





