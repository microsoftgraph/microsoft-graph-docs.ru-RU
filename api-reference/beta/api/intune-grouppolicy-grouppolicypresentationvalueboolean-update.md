---
title: Обновление Граупполиципресентатионвалуебулеан
description: Обновление свойств объекта Граупполиципресентатионвалуебулеан.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1a249347f3c1e7717558e9872ad0524e278cd56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970067"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="c704d-103">Обновление Граупполиципресентатионвалуебулеан</span><span class="sxs-lookup"><span data-stu-id="c704d-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="c704d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c704d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c704d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c704d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c704d-106">Обновление свойств объекта [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="c704d-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c704d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c704d-107">Prerequisites</span></span>
<span data-ttu-id="c704d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c704d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c704d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c704d-110">Permission type</span></span>|<span data-ttu-id="c704d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c704d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c704d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c704d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c704d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c704d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c704d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c704d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c704d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c704d-115">Not supported.</span></span>|
|<span data-ttu-id="c704d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c704d-116">Application</span></span>|<span data-ttu-id="c704d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c704d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c704d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c704d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="c704d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c704d-119">Request headers</span></span>
|<span data-ttu-id="c704d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c704d-120">Header</span></span>|<span data-ttu-id="c704d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c704d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c704d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c704d-122">Authorization</span></span>|<span data-ttu-id="c704d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c704d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c704d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c704d-124">Accept</span></span>|<span data-ttu-id="c704d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c704d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c704d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c704d-126">Request body</span></span>
<span data-ttu-id="c704d-127">В тексте запроса добавьте представление объекта [Граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c704d-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="c704d-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span><span class="sxs-lookup"><span data-stu-id="c704d-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="c704d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c704d-129">Property</span></span>|<span data-ttu-id="c704d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c704d-130">Type</span></span>|<span data-ttu-id="c704d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c704d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c704d-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c704d-132">lastModifiedDateTime</span></span>|<span data-ttu-id="c704d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c704d-133">DateTimeOffset</span></span>|<span data-ttu-id="c704d-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c704d-134">The date and time the object was last modified.</span></span> <span data-ttu-id="c704d-135">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c704d-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c704d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c704d-136">createdDateTime</span></span>|<span data-ttu-id="c704d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c704d-137">DateTimeOffset</span></span>|<span data-ttu-id="c704d-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c704d-138">The date and time the object was created.</span></span> <span data-ttu-id="c704d-139">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c704d-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c704d-140">id</span><span class="sxs-lookup"><span data-stu-id="c704d-140">id</span></span>|<span data-ttu-id="c704d-141">String</span><span class="sxs-lookup"><span data-stu-id="c704d-141">String</span></span>|<span data-ttu-id="c704d-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c704d-142">Key of the entity.</span></span> <span data-ttu-id="c704d-143">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c704d-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c704d-144">value</span><span class="sxs-lookup"><span data-stu-id="c704d-144">value</span></span>|<span data-ttu-id="c704d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c704d-145">Boolean</span></span>|<span data-ttu-id="c704d-146">Логическое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="c704d-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="c704d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c704d-147">Response</span></span>
<span data-ttu-id="c704d-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c704d-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c704d-149">Пример</span><span class="sxs-lookup"><span data-stu-id="c704d-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c704d-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c704d-150">Request</span></span>
<span data-ttu-id="c704d-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c704d-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="c704d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c704d-152">Response</span></span>
<span data-ttu-id="c704d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c704d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




