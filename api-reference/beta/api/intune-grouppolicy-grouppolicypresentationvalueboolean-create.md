---
title: Создание Граупполиципресентатионвалуебулеан
description: Создание нового объекта Граупполиципресентатионвалуебулеан.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd4cf6ba8a7205aadd13e8b4b1d3824d0f812745
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804011"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="df630-103">Создание Граупполиципресентатионвалуебулеан</span><span class="sxs-lookup"><span data-stu-id="df630-103">Create groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="df630-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df630-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df630-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df630-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df630-106">Создание нового объекта [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="df630-106">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df630-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df630-107">Prerequisites</span></span>
<span data-ttu-id="df630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df630-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df630-110">Permission type</span></span>|<span data-ttu-id="df630-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df630-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df630-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df630-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df630-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df630-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df630-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df630-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df630-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df630-115">Not supported.</span></span>|
|<span data-ttu-id="df630-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="df630-116">Application</span></span>|<span data-ttu-id="df630-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df630-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df630-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df630-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="df630-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df630-119">Request headers</span></span>
|<span data-ttu-id="df630-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df630-120">Header</span></span>|<span data-ttu-id="df630-121">Значение</span><span class="sxs-lookup"><span data-stu-id="df630-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df630-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df630-122">Authorization</span></span>|<span data-ttu-id="df630-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df630-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df630-124">Accept</span><span class="sxs-lookup"><span data-stu-id="df630-124">Accept</span></span>|<span data-ttu-id="df630-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df630-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df630-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df630-126">Request body</span></span>
<span data-ttu-id="df630-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуебулеан в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df630-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="df630-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуебулеан.</span><span class="sxs-lookup"><span data-stu-id="df630-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="df630-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="df630-129">Property</span></span>|<span data-ttu-id="df630-130">Тип</span><span class="sxs-lookup"><span data-stu-id="df630-130">Type</span></span>|<span data-ttu-id="df630-131">Описание</span><span class="sxs-lookup"><span data-stu-id="df630-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df630-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df630-132">lastModifiedDateTime</span></span>|<span data-ttu-id="df630-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df630-133">DateTimeOffset</span></span>|<span data-ttu-id="df630-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="df630-134">The date and time the object was last modified.</span></span> <span data-ttu-id="df630-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="df630-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="df630-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df630-136">createdDateTime</span></span>|<span data-ttu-id="df630-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df630-137">DateTimeOffset</span></span>|<span data-ttu-id="df630-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="df630-138">The date and time the object was created.</span></span> <span data-ttu-id="df630-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="df630-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="df630-140">id</span><span class="sxs-lookup"><span data-stu-id="df630-140">id</span></span>|<span data-ttu-id="df630-141">String</span><span class="sxs-lookup"><span data-stu-id="df630-141">String</span></span>|<span data-ttu-id="df630-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="df630-142">Key of the entity.</span></span> <span data-ttu-id="df630-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="df630-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="df630-144">value</span><span class="sxs-lookup"><span data-stu-id="df630-144">value</span></span>|<span data-ttu-id="df630-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="df630-145">Boolean</span></span>|<span data-ttu-id="df630-146">Логическое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="df630-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="df630-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="df630-147">Response</span></span>
<span data-ttu-id="df630-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df630-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df630-149">Пример</span><span class="sxs-lookup"><span data-stu-id="df630-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="df630-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="df630-150">Request</span></span>
<span data-ttu-id="df630-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df630-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="df630-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="df630-152">Response</span></span>
<span data-ttu-id="df630-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df630-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "be61344f-344f-be61-4f34-61be4f3461be",
  "value": true
}
```




