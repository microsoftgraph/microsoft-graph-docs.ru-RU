---
title: Обновление Граупполиципресентатионвалуелист
description: Обновление свойств объекта Граупполиципресентатионвалуелист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb51f17998e5a1f0ba0b062a422dd4e6f5ca0940
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942621"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="7f07a-103">Обновление Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="7f07a-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="7f07a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f07a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f07a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f07a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f07a-106">Обновление свойств объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="7f07a-106">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f07a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f07a-107">Prerequisites</span></span>
<span data-ttu-id="7f07a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f07a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f07a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f07a-110">Permission type</span></span>|<span data-ttu-id="7f07a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f07a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f07a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f07a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f07a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f07a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f07a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f07a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f07a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f07a-115">Not supported.</span></span>|
|<span data-ttu-id="7f07a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f07a-116">Application</span></span>|<span data-ttu-id="7f07a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f07a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f07a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f07a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="7f07a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f07a-119">Request headers</span></span>
|<span data-ttu-id="7f07a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f07a-120">Header</span></span>|<span data-ttu-id="7f07a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f07a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f07a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f07a-122">Authorization</span></span>|<span data-ttu-id="7f07a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f07a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f07a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f07a-124">Accept</span></span>|<span data-ttu-id="7f07a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f07a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f07a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f07a-126">Request body</span></span>
<span data-ttu-id="7f07a-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f07a-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="7f07a-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span><span class="sxs-lookup"><span data-stu-id="7f07a-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="7f07a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f07a-129">Property</span></span>|<span data-ttu-id="7f07a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f07a-130">Type</span></span>|<span data-ttu-id="7f07a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f07a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f07a-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f07a-132">lastModifiedDateTime</span></span>|<span data-ttu-id="7f07a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f07a-133">DateTimeOffset</span></span>|<span data-ttu-id="7f07a-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7f07a-134">The date and time the object was last modified.</span></span> <span data-ttu-id="7f07a-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7f07a-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7f07a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f07a-136">createdDateTime</span></span>|<span data-ttu-id="7f07a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f07a-137">DateTimeOffset</span></span>|<span data-ttu-id="7f07a-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7f07a-138">The date and time the object was created.</span></span> <span data-ttu-id="7f07a-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7f07a-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7f07a-140">id</span><span class="sxs-lookup"><span data-stu-id="7f07a-140">id</span></span>|<span data-ttu-id="7f07a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="7f07a-141">String</span></span>|<span data-ttu-id="7f07a-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f07a-142">Key of the entity.</span></span> <span data-ttu-id="7f07a-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7f07a-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7f07a-144">values</span><span class="sxs-lookup"><span data-stu-id="7f07a-144">values</span></span>|<span data-ttu-id="7f07a-145">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7f07a-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7f07a-146">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="7f07a-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="7f07a-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f07a-147">Response</span></span>
<span data-ttu-id="7f07a-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f07a-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f07a-149">Пример</span><span class="sxs-lookup"><span data-stu-id="7f07a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f07a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f07a-150">Request</span></span>
<span data-ttu-id="7f07a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f07a-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f07a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f07a-152">Response</span></span>
<span data-ttu-id="7f07a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f07a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





