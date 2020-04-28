---
title: Обновление Граупполиципресентатионвалуелист
description: Обновление свойств объекта Граупполиципресентатионвалуелист.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c61d31bfd1e1e77806ae5e647fec9e70b794d8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460268"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="6e88d-103">Обновление Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="6e88d-103">Update groupPolicyPresentationValueList</span></span>

<span data-ttu-id="6e88d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e88d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e88d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e88d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e88d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e88d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e88d-107">Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="6e88d-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e88d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e88d-108">Prerequisites</span></span>
<span data-ttu-id="6e88d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e88d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e88d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e88d-111">Permission type</span></span>|<span data-ttu-id="6e88d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e88d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e88d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e88d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e88d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e88d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e88d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e88d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e88d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e88d-116">Not supported.</span></span>|
|<span data-ttu-id="6e88d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e88d-117">Application</span></span>|<span data-ttu-id="6e88d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e88d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e88d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e88d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="6e88d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e88d-120">Request headers</span></span>
|<span data-ttu-id="6e88d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e88d-121">Header</span></span>|<span data-ttu-id="6e88d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e88d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e88d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e88d-123">Authorization</span></span>|<span data-ttu-id="6e88d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e88d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e88d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e88d-125">Accept</span></span>|<span data-ttu-id="6e88d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e88d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e88d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e88d-127">Request body</span></span>
<span data-ttu-id="6e88d-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e88d-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="6e88d-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="6e88d-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="6e88d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e88d-130">Property</span></span>|<span data-ttu-id="6e88d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e88d-131">Type</span></span>|<span data-ttu-id="6e88d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e88d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e88d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e88d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6e88d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e88d-134">DateTimeOffset</span></span>|<span data-ttu-id="6e88d-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e88d-135">The date and time the object was last modified.</span></span> <span data-ttu-id="6e88d-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e88d-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e88d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e88d-137">createdDateTime</span></span>|<span data-ttu-id="6e88d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e88d-138">DateTimeOffset</span></span>|<span data-ttu-id="6e88d-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e88d-139">The date and time the object was created.</span></span> <span data-ttu-id="6e88d-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e88d-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e88d-141">id</span><span class="sxs-lookup"><span data-stu-id="6e88d-141">id</span></span>|<span data-ttu-id="6e88d-142">String</span><span class="sxs-lookup"><span data-stu-id="6e88d-142">String</span></span>|<span data-ttu-id="6e88d-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e88d-143">Key of the entity.</span></span> <span data-ttu-id="6e88d-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e88d-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e88d-145">values</span><span class="sxs-lookup"><span data-stu-id="6e88d-145">values</span></span>|<span data-ttu-id="6e88d-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6e88d-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6e88d-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="6e88d-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="6e88d-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e88d-148">Response</span></span>
<span data-ttu-id="6e88d-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e88d-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e88d-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6e88d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e88d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e88d-151">Request</span></span>
<span data-ttu-id="6e88d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e88d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e88d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e88d-153">Response</span></span>
<span data-ttu-id="6e88d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e88d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



