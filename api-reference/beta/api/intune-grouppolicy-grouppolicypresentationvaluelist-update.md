---
title: Обновление Граупполиципресентатионвалуелист
description: Обновление свойств объекта Граупполиципресентатионвалуелист.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f43f17b95f565fec62d904da566cd33396c6b5d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994612"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="9a61a-103">Обновление Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="9a61a-103">Update groupPolicyPresentationValueList</span></span>

<span data-ttu-id="9a61a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a61a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a61a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a61a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a61a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a61a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a61a-107">Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="9a61a-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a61a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a61a-108">Prerequisites</span></span>
<span data-ttu-id="9a61a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a61a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a61a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a61a-111">Permission type</span></span>|<span data-ttu-id="9a61a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a61a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a61a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a61a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a61a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a61a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a61a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a61a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a61a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a61a-116">Not supported.</span></span>|
|<span data-ttu-id="9a61a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a61a-117">Application</span></span>|<span data-ttu-id="9a61a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a61a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a61a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a61a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="9a61a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a61a-120">Request headers</span></span>
|<span data-ttu-id="9a61a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a61a-121">Header</span></span>|<span data-ttu-id="9a61a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a61a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a61a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a61a-123">Authorization</span></span>|<span data-ttu-id="9a61a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a61a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a61a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a61a-125">Accept</span></span>|<span data-ttu-id="9a61a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a61a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a61a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a61a-127">Request body</span></span>
<span data-ttu-id="9a61a-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a61a-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="9a61a-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="9a61a-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="9a61a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a61a-130">Property</span></span>|<span data-ttu-id="9a61a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a61a-131">Type</span></span>|<span data-ttu-id="9a61a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a61a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a61a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a61a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9a61a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a61a-134">DateTimeOffset</span></span>|<span data-ttu-id="9a61a-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9a61a-135">The date and time the object was last modified.</span></span> <span data-ttu-id="9a61a-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9a61a-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9a61a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a61a-137">createdDateTime</span></span>|<span data-ttu-id="9a61a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a61a-138">DateTimeOffset</span></span>|<span data-ttu-id="9a61a-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9a61a-139">The date and time the object was created.</span></span> <span data-ttu-id="9a61a-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9a61a-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9a61a-141">id</span><span class="sxs-lookup"><span data-stu-id="9a61a-141">id</span></span>|<span data-ttu-id="9a61a-142">String</span><span class="sxs-lookup"><span data-stu-id="9a61a-142">String</span></span>|<span data-ttu-id="9a61a-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9a61a-143">Key of the entity.</span></span> <span data-ttu-id="9a61a-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9a61a-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9a61a-145">values</span><span class="sxs-lookup"><span data-stu-id="9a61a-145">values</span></span>|<span data-ttu-id="9a61a-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9a61a-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9a61a-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="9a61a-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="9a61a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a61a-148">Response</span></span>
<span data-ttu-id="9a61a-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a61a-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a61a-150">Пример</span><span class="sxs-lookup"><span data-stu-id="9a61a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a61a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a61a-151">Request</span></span>
<span data-ttu-id="9a61a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a61a-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a61a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a61a-153">Response</span></span>
<span data-ttu-id="9a61a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a61a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






