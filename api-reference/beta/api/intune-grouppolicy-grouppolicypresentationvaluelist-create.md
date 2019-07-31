---
title: Создание Граупполиципресентатионвалуелист
description: Создание нового объекта Граупполиципресентатионвалуелист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 148567a611eaa5c3f8a7c857f2b50e947d3a1241
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989128"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="668ce-103">Создание Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="668ce-103">Create groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="668ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="668ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="668ce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="668ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="668ce-106">Создание нового объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="668ce-106">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="668ce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="668ce-107">Prerequisites</span></span>
<span data-ttu-id="668ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="668ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="668ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="668ce-110">Permission type</span></span>|<span data-ttu-id="668ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="668ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="668ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="668ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="668ce-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="668ce-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="668ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="668ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="668ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="668ce-115">Not supported.</span></span>|
|<span data-ttu-id="668ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="668ce-116">Application</span></span>|<span data-ttu-id="668ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="668ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="668ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="668ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="668ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="668ce-119">Request headers</span></span>
|<span data-ttu-id="668ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="668ce-120">Header</span></span>|<span data-ttu-id="668ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="668ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="668ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="668ce-122">Authorization</span></span>|<span data-ttu-id="668ce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="668ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="668ce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="668ce-124">Accept</span></span>|<span data-ttu-id="668ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="668ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="668ce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="668ce-126">Request body</span></span>
<span data-ttu-id="668ce-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуелист в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668ce-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="668ce-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуелист.</span><span class="sxs-lookup"><span data-stu-id="668ce-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="668ce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="668ce-129">Property</span></span>|<span data-ttu-id="668ce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="668ce-130">Type</span></span>|<span data-ttu-id="668ce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="668ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="668ce-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="668ce-132">lastModifiedDateTime</span></span>|<span data-ttu-id="668ce-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="668ce-133">DateTimeOffset</span></span>|<span data-ttu-id="668ce-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="668ce-134">The date and time the object was last modified.</span></span> <span data-ttu-id="668ce-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="668ce-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="668ce-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="668ce-136">createdDateTime</span></span>|<span data-ttu-id="668ce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="668ce-137">DateTimeOffset</span></span>|<span data-ttu-id="668ce-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="668ce-138">The date and time the object was created.</span></span> <span data-ttu-id="668ce-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="668ce-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="668ce-140">id</span><span class="sxs-lookup"><span data-stu-id="668ce-140">id</span></span>|<span data-ttu-id="668ce-141">String</span><span class="sxs-lookup"><span data-stu-id="668ce-141">String</span></span>|<span data-ttu-id="668ce-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="668ce-142">Key of the entity.</span></span> <span data-ttu-id="668ce-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="668ce-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="668ce-144">values</span><span class="sxs-lookup"><span data-stu-id="668ce-144">values</span></span>|<span data-ttu-id="668ce-145">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="668ce-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="668ce-146">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="668ce-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="668ce-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="668ce-147">Response</span></span>
<span data-ttu-id="668ce-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="668ce-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668ce-149">Пример</span><span class="sxs-lookup"><span data-stu-id="668ce-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="668ce-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="668ce-150">Request</span></span>
<span data-ttu-id="668ce-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="668ce-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="668ce-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="668ce-152">Response</span></span>
<span data-ttu-id="668ce-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="668ce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```





