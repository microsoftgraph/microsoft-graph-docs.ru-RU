---
title: Создание Граупполиципресентатионвалуелист
description: Создание нового объекта Граупполиципресентатионвалуелист.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a98f68e5a12fae5dc58da301bd730b1616b9fc61
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734338"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="b4226-103">Создание Граупполиципресентатионвалуелист</span><span class="sxs-lookup"><span data-stu-id="b4226-103">Create groupPolicyPresentationValueList</span></span>

<span data-ttu-id="b4226-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4226-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4226-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4226-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4226-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4226-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4226-107">Создание нового объекта [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="b4226-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4226-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4226-108">Prerequisites</span></span>
<span data-ttu-id="b4226-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4226-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4226-111">Permission type</span></span>|<span data-ttu-id="b4226-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4226-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4226-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4226-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4226-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4226-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4226-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4226-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4226-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4226-116">Not supported.</span></span>|
|<span data-ttu-id="b4226-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4226-117">Application</span></span>|<span data-ttu-id="b4226-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4226-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4226-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4226-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="b4226-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4226-120">Request headers</span></span>
|<span data-ttu-id="b4226-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4226-121">Header</span></span>|<span data-ttu-id="b4226-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4226-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4226-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4226-123">Authorization</span></span>|<span data-ttu-id="b4226-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4226-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4226-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4226-125">Accept</span></span>|<span data-ttu-id="b4226-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4226-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4226-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4226-127">Request body</span></span>
<span data-ttu-id="b4226-128">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуелист в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4226-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="b4226-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуелист.</span><span class="sxs-lookup"><span data-stu-id="b4226-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="b4226-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4226-130">Property</span></span>|<span data-ttu-id="b4226-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4226-131">Type</span></span>|<span data-ttu-id="b4226-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4226-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4226-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4226-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b4226-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4226-134">DateTimeOffset</span></span>|<span data-ttu-id="b4226-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b4226-135">The date and time the object was last modified.</span></span> <span data-ttu-id="b4226-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b4226-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b4226-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4226-137">createdDateTime</span></span>|<span data-ttu-id="b4226-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4226-138">DateTimeOffset</span></span>|<span data-ttu-id="b4226-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b4226-139">The date and time the object was created.</span></span> <span data-ttu-id="b4226-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b4226-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b4226-141">id</span><span class="sxs-lookup"><span data-stu-id="b4226-141">id</span></span>|<span data-ttu-id="b4226-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b4226-142">String</span></span>|<span data-ttu-id="b4226-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4226-143">Key of the entity.</span></span> <span data-ttu-id="b4226-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b4226-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b4226-145">values</span><span class="sxs-lookup"><span data-stu-id="b4226-145">values</span></span>|<span data-ttu-id="b4226-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b4226-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b4226-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="b4226-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b4226-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4226-148">Response</span></span>
<span data-ttu-id="b4226-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4226-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4226-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b4226-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4226-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4226-151">Request</span></span>
<span data-ttu-id="b4226-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4226-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4226-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4226-153">Response</span></span>
<span data-ttu-id="b4226-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4226-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





