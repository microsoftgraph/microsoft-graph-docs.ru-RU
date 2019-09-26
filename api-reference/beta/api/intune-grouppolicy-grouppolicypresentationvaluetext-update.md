---
title: Обновление Граупполиципресентатионвалуетекст
description: Обновление свойств объекта Граупполиципресентатионвалуетекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32264c89594fd10ea9aeea444d65542c4bec25f1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193454"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="2092f-103">Обновление Граупполиципресентатионвалуетекст</span><span class="sxs-lookup"><span data-stu-id="2092f-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="2092f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2092f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2092f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2092f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2092f-106">Обновление свойств объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="2092f-106">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2092f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2092f-107">Prerequisites</span></span>
<span data-ttu-id="2092f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2092f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2092f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2092f-110">Permission type</span></span>|<span data-ttu-id="2092f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2092f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2092f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2092f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2092f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2092f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2092f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2092f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2092f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2092f-115">Not supported.</span></span>|
|<span data-ttu-id="2092f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2092f-116">Application</span></span>|<span data-ttu-id="2092f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2092f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2092f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2092f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="2092f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2092f-119">Request headers</span></span>
|<span data-ttu-id="2092f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2092f-120">Header</span></span>|<span data-ttu-id="2092f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2092f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2092f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2092f-122">Authorization</span></span>|<span data-ttu-id="2092f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2092f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2092f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2092f-124">Accept</span></span>|<span data-ttu-id="2092f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2092f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2092f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2092f-126">Request body</span></span>
<span data-ttu-id="2092f-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2092f-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="2092f-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span><span class="sxs-lookup"><span data-stu-id="2092f-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="2092f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2092f-129">Property</span></span>|<span data-ttu-id="2092f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2092f-130">Type</span></span>|<span data-ttu-id="2092f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2092f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2092f-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2092f-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2092f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2092f-133">DateTimeOffset</span></span>|<span data-ttu-id="2092f-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2092f-134">The date and time the object was last modified.</span></span> <span data-ttu-id="2092f-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2092f-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2092f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2092f-136">createdDateTime</span></span>|<span data-ttu-id="2092f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2092f-137">DateTimeOffset</span></span>|<span data-ttu-id="2092f-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2092f-138">The date and time the object was created.</span></span> <span data-ttu-id="2092f-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2092f-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2092f-140">id</span><span class="sxs-lookup"><span data-stu-id="2092f-140">id</span></span>|<span data-ttu-id="2092f-141">String</span><span class="sxs-lookup"><span data-stu-id="2092f-141">String</span></span>|<span data-ttu-id="2092f-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2092f-142">Key of the entity.</span></span> <span data-ttu-id="2092f-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2092f-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2092f-144">value</span><span class="sxs-lookup"><span data-stu-id="2092f-144">value</span></span>|<span data-ttu-id="2092f-145">String</span><span class="sxs-lookup"><span data-stu-id="2092f-145">String</span></span>|<span data-ttu-id="2092f-146">Строковое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="2092f-146">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2092f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2092f-147">Response</span></span>
<span data-ttu-id="2092f-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2092f-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2092f-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2092f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2092f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2092f-150">Request</span></span>
<span data-ttu-id="2092f-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2092f-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="2092f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2092f-152">Response</span></span>
<span data-ttu-id="2092f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2092f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




