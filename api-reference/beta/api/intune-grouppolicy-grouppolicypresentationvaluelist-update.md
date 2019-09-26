---
title: Обновление Граупполиципресентатионвалуелист
description: Обновление свойств объекта Граупполиципресентатионвалуелист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dee7e6c120dc64a3edb2875358f312a2f4967ea6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193685"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="5bb80-103">Обновление Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="5bb80-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="5bb80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bb80-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bb80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb80-106">Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="5bb80-106">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bb80-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5bb80-107">Prerequisites</span></span>
<span data-ttu-id="5bb80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bb80-110">Permission type</span></span>|<span data-ttu-id="5bb80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bb80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bb80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb80-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb80-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bb80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb80-115">Not supported.</span></span>|
|<span data-ttu-id="5bb80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bb80-116">Application</span></span>|<span data-ttu-id="5bb80-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb80-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bb80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="5bb80-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bb80-119">Request headers</span></span>
|<span data-ttu-id="5bb80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bb80-120">Header</span></span>|<span data-ttu-id="5bb80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5bb80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb80-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bb80-122">Authorization</span></span>|<span data-ttu-id="5bb80-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bb80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5bb80-124">Accept</span></span>|<span data-ttu-id="5bb80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb80-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bb80-126">Request body</span></span>
<span data-ttu-id="5bb80-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bb80-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="5bb80-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="5bb80-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="5bb80-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bb80-129">Property</span></span>|<span data-ttu-id="5bb80-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5bb80-130">Type</span></span>|<span data-ttu-id="5bb80-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5bb80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb80-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb80-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5bb80-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb80-133">DateTimeOffset</span></span>|<span data-ttu-id="5bb80-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5bb80-134">The date and time the object was last modified.</span></span> <span data-ttu-id="5bb80-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5bb80-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5bb80-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb80-136">createdDateTime</span></span>|<span data-ttu-id="5bb80-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb80-137">DateTimeOffset</span></span>|<span data-ttu-id="5bb80-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5bb80-138">The date and time the object was created.</span></span> <span data-ttu-id="5bb80-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5bb80-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5bb80-140">id</span><span class="sxs-lookup"><span data-stu-id="5bb80-140">id</span></span>|<span data-ttu-id="5bb80-141">String</span><span class="sxs-lookup"><span data-stu-id="5bb80-141">String</span></span>|<span data-ttu-id="5bb80-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5bb80-142">Key of the entity.</span></span> <span data-ttu-id="5bb80-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5bb80-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5bb80-144">values</span><span class="sxs-lookup"><span data-stu-id="5bb80-144">values</span></span>|<span data-ttu-id="5bb80-145">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5bb80-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5bb80-146">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="5bb80-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="5bb80-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb80-147">Response</span></span>
<span data-ttu-id="5bb80-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bb80-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb80-149">Пример</span><span class="sxs-lookup"><span data-stu-id="5bb80-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb80-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bb80-150">Request</span></span>
<span data-ttu-id="5bb80-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bb80-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
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

### <a name="response"></a><span data-ttu-id="5bb80-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb80-152">Response</span></span>
<span data-ttu-id="5bb80-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bb80-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




