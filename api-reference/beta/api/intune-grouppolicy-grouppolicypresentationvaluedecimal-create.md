---
title: Создание ГраупполиципресентатионвалуедеЦимал
description: Создание нового объекта ГраупполиципресентатионвалуедеЦимал.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a494b9f45a33d8fd8ad8207c6c798ad0bea5fd03
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456569"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="33c54-103">Создание ГраупполиципресентатионвалуедеЦимал</span><span class="sxs-lookup"><span data-stu-id="33c54-103">Create groupPolicyPresentationValueDecimal</span></span>

<span data-ttu-id="33c54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33c54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33c54-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33c54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33c54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33c54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33c54-107">Создание нового объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="33c54-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33c54-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33c54-108">Prerequisites</span></span>
<span data-ttu-id="33c54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33c54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33c54-111">Permission type</span></span>|<span data-ttu-id="33c54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33c54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33c54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33c54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33c54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33c54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33c54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33c54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33c54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33c54-116">Not supported.</span></span>|
|<span data-ttu-id="33c54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33c54-117">Application</span></span>|<span data-ttu-id="33c54-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33c54-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33c54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33c54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="33c54-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33c54-120">Request headers</span></span>
|<span data-ttu-id="33c54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33c54-121">Header</span></span>|<span data-ttu-id="33c54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33c54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33c54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33c54-123">Authorization</span></span>|<span data-ttu-id="33c54-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33c54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33c54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33c54-125">Accept</span></span>|<span data-ttu-id="33c54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33c54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33c54-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33c54-127">Request body</span></span>
<span data-ttu-id="33c54-128">В тексте запроса добавьте представление объекта ГраупполиципресентатионвалуедеЦимал в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33c54-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="33c54-129">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатионвалуедеЦимал.</span><span class="sxs-lookup"><span data-stu-id="33c54-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="33c54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33c54-130">Property</span></span>|<span data-ttu-id="33c54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33c54-131">Type</span></span>|<span data-ttu-id="33c54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33c54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33c54-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33c54-133">lastModifiedDateTime</span></span>|<span data-ttu-id="33c54-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33c54-134">DateTimeOffset</span></span>|<span data-ttu-id="33c54-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33c54-135">The date and time the object was last modified.</span></span> <span data-ttu-id="33c54-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="33c54-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="33c54-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33c54-137">createdDateTime</span></span>|<span data-ttu-id="33c54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33c54-138">DateTimeOffset</span></span>|<span data-ttu-id="33c54-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33c54-139">The date and time the object was created.</span></span> <span data-ttu-id="33c54-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="33c54-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="33c54-141">id</span><span class="sxs-lookup"><span data-stu-id="33c54-141">id</span></span>|<span data-ttu-id="33c54-142">String</span><span class="sxs-lookup"><span data-stu-id="33c54-142">String</span></span>|<span data-ttu-id="33c54-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33c54-143">Key of the entity.</span></span> <span data-ttu-id="33c54-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="33c54-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="33c54-145">значение</span><span class="sxs-lookup"><span data-stu-id="33c54-145">value</span></span>|<span data-ttu-id="33c54-146">Int64</span><span class="sxs-lookup"><span data-stu-id="33c54-146">Int64</span></span>|<span data-ttu-id="33c54-147">Целое значение без знака для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="33c54-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="33c54-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c54-148">Response</span></span>
<span data-ttu-id="33c54-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33c54-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33c54-150">Пример</span><span class="sxs-lookup"><span data-stu-id="33c54-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="33c54-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="33c54-151">Request</span></span>
<span data-ttu-id="33c54-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33c54-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="33c54-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c54-153">Response</span></span>
<span data-ttu-id="33c54-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33c54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```



