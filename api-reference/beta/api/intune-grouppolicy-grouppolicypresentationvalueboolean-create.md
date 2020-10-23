---
title: Создание Граупполиципресентатионвалуебулеан
description: Создание нового объекта Граупполиципресентатионвалуебулеан.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4eecddf7a8612c8f97609d0ec41d2a795c4b234
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706557"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="453d2-103">Создание Граупполиципресентатионвалуебулеан</span><span class="sxs-lookup"><span data-stu-id="453d2-103">Create groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="453d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="453d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="453d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="453d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="453d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="453d2-107">Создание нового объекта [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="453d2-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="453d2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="453d2-108">Prerequisites</span></span>
<span data-ttu-id="453d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="453d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="453d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="453d2-111">Permission type</span></span>|<span data-ttu-id="453d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="453d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="453d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="453d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="453d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="453d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="453d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="453d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453d2-116">Not supported.</span></span>|
|<span data-ttu-id="453d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="453d2-117">Application</span></span>|<span data-ttu-id="453d2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453d2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="453d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="453d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="453d2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="453d2-120">Request headers</span></span>
|<span data-ttu-id="453d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="453d2-121">Header</span></span>|<span data-ttu-id="453d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="453d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="453d2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="453d2-123">Authorization</span></span>|<span data-ttu-id="453d2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="453d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="453d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="453d2-125">Accept</span></span>|<span data-ttu-id="453d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="453d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="453d2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="453d2-127">Request body</span></span>
<span data-ttu-id="453d2-128">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуебулеан в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453d2-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="453d2-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуебулеан.</span><span class="sxs-lookup"><span data-stu-id="453d2-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="453d2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="453d2-130">Property</span></span>|<span data-ttu-id="453d2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="453d2-131">Type</span></span>|<span data-ttu-id="453d2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="453d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453d2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="453d2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="453d2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453d2-134">DateTimeOffset</span></span>|<span data-ttu-id="453d2-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="453d2-135">The date and time the object was last modified.</span></span> <span data-ttu-id="453d2-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="453d2-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="453d2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="453d2-137">createdDateTime</span></span>|<span data-ttu-id="453d2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453d2-138">DateTimeOffset</span></span>|<span data-ttu-id="453d2-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="453d2-139">The date and time the object was created.</span></span> <span data-ttu-id="453d2-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="453d2-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="453d2-141">id</span><span class="sxs-lookup"><span data-stu-id="453d2-141">id</span></span>|<span data-ttu-id="453d2-142">Строка</span><span class="sxs-lookup"><span data-stu-id="453d2-142">String</span></span>|<span data-ttu-id="453d2-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="453d2-143">Key of the entity.</span></span> <span data-ttu-id="453d2-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="453d2-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="453d2-145">value</span><span class="sxs-lookup"><span data-stu-id="453d2-145">value</span></span>|<span data-ttu-id="453d2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="453d2-146">Boolean</span></span>|<span data-ttu-id="453d2-147">Логическое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="453d2-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="453d2-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="453d2-148">Response</span></span>
<span data-ttu-id="453d2-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="453d2-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="453d2-150">Пример</span><span class="sxs-lookup"><span data-stu-id="453d2-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="453d2-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="453d2-151">Request</span></span>
<span data-ttu-id="453d2-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="453d2-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="453d2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="453d2-153">Response</span></span>
<span data-ttu-id="453d2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="453d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





