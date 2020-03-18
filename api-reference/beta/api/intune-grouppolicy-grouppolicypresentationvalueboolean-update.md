---
title: Обновление Граупполиципресентатионвалуебулеан
description: Обновление свойств объекта Граупполиципресентатионвалуебулеан.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6edb102c3875333656a8936fb4f32f89f22d7366
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803983"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="6cdcf-103">Обновление Граупполиципресентатионвалуебулеан</span><span class="sxs-lookup"><span data-stu-id="6cdcf-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="6cdcf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cdcf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cdcf-106">Обновление свойств объекта [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="6cdcf-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cdcf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cdcf-107">Prerequisites</span></span>
<span data-ttu-id="6cdcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cdcf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cdcf-110">Permission type</span></span>|<span data-ttu-id="6cdcf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cdcf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cdcf-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdcf-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6cdcf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cdcf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-115">Not supported.</span></span>|
|<span data-ttu-id="6cdcf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6cdcf-116">Application</span></span>|<span data-ttu-id="6cdcf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdcf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cdcf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cdcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="6cdcf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6cdcf-119">Request headers</span></span>
|<span data-ttu-id="6cdcf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cdcf-120">Header</span></span>|<span data-ttu-id="6cdcf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6cdcf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cdcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cdcf-122">Authorization</span></span>|<span data-ttu-id="6cdcf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cdcf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6cdcf-124">Accept</span></span>|<span data-ttu-id="6cdcf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cdcf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cdcf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cdcf-126">Request body</span></span>
<span data-ttu-id="6cdcf-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="6cdcf-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span><span class="sxs-lookup"><span data-stu-id="6cdcf-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="6cdcf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cdcf-129">Property</span></span>|<span data-ttu-id="6cdcf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6cdcf-130">Type</span></span>|<span data-ttu-id="6cdcf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6cdcf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cdcf-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdcf-132">lastModifiedDateTime</span></span>|<span data-ttu-id="6cdcf-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cdcf-133">DateTimeOffset</span></span>|<span data-ttu-id="6cdcf-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-134">The date and time the object was last modified.</span></span> <span data-ttu-id="6cdcf-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6cdcf-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdcf-136">createdDateTime</span></span>|<span data-ttu-id="6cdcf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cdcf-137">DateTimeOffset</span></span>|<span data-ttu-id="6cdcf-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-138">The date and time the object was created.</span></span> <span data-ttu-id="6cdcf-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6cdcf-140">id</span><span class="sxs-lookup"><span data-stu-id="6cdcf-140">id</span></span>|<span data-ttu-id="6cdcf-141">String</span><span class="sxs-lookup"><span data-stu-id="6cdcf-141">String</span></span>|<span data-ttu-id="6cdcf-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-142">Key of the entity.</span></span> <span data-ttu-id="6cdcf-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcf-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6cdcf-144">value</span><span class="sxs-lookup"><span data-stu-id="6cdcf-144">value</span></span>|<span data-ttu-id="6cdcf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cdcf-145">Boolean</span></span>|<span data-ttu-id="6cdcf-146">Логическое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="6cdcf-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cdcf-147">Response</span></span>
<span data-ttu-id="6cdcf-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cdcf-149">Пример</span><span class="sxs-lookup"><span data-stu-id="6cdcf-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cdcf-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cdcf-150">Request</span></span>
<span data-ttu-id="6cdcf-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="6cdcf-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cdcf-152">Response</span></span>
<span data-ttu-id="6cdcf-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cdcf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




