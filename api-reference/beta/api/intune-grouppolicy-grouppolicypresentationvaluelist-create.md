---
title: Создание Граупполиципресентатионвалуелист
description: Создание нового объекта Граупполиципресентатионвалуелист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d77f344d90ff691b7bf2a16cab2b75f59370f97d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464234"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="9069f-103">Создание Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="9069f-103">Create groupPolicyPresentationValueList</span></span>

<span data-ttu-id="9069f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9069f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9069f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9069f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9069f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9069f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9069f-107">Создание нового объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="9069f-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9069f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9069f-108">Prerequisites</span></span>
<span data-ttu-id="9069f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9069f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9069f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9069f-111">Permission type</span></span>|<span data-ttu-id="9069f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9069f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9069f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9069f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9069f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9069f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9069f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9069f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9069f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9069f-116">Not supported.</span></span>|
|<span data-ttu-id="9069f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9069f-117">Application</span></span>|<span data-ttu-id="9069f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9069f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9069f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9069f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="9069f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9069f-120">Request headers</span></span>
|<span data-ttu-id="9069f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9069f-121">Header</span></span>|<span data-ttu-id="9069f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9069f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9069f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9069f-123">Authorization</span></span>|<span data-ttu-id="9069f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9069f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9069f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9069f-125">Accept</span></span>|<span data-ttu-id="9069f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9069f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9069f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9069f-127">Request body</span></span>
<span data-ttu-id="9069f-128">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуелист в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9069f-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="9069f-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуелист.</span><span class="sxs-lookup"><span data-stu-id="9069f-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="9069f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9069f-130">Property</span></span>|<span data-ttu-id="9069f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9069f-131">Type</span></span>|<span data-ttu-id="9069f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9069f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9069f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9069f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9069f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9069f-134">DateTimeOffset</span></span>|<span data-ttu-id="9069f-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9069f-135">The date and time the object was last modified.</span></span> <span data-ttu-id="9069f-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9069f-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9069f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9069f-137">createdDateTime</span></span>|<span data-ttu-id="9069f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9069f-138">DateTimeOffset</span></span>|<span data-ttu-id="9069f-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9069f-139">The date and time the object was created.</span></span> <span data-ttu-id="9069f-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9069f-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9069f-141">id</span><span class="sxs-lookup"><span data-stu-id="9069f-141">id</span></span>|<span data-ttu-id="9069f-142">String</span><span class="sxs-lookup"><span data-stu-id="9069f-142">String</span></span>|<span data-ttu-id="9069f-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9069f-143">Key of the entity.</span></span> <span data-ttu-id="9069f-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9069f-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9069f-145">values</span><span class="sxs-lookup"><span data-stu-id="9069f-145">values</span></span>|<span data-ttu-id="9069f-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9069f-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9069f-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="9069f-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="9069f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9069f-148">Response</span></span>
<span data-ttu-id="9069f-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9069f-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9069f-150">Пример</span><span class="sxs-lookup"><span data-stu-id="9069f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="9069f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9069f-151">Request</span></span>
<span data-ttu-id="9069f-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9069f-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9069f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9069f-153">Response</span></span>
<span data-ttu-id="9069f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9069f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





