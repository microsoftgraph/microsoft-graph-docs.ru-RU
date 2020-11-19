---
title: Создание Граупполиципресентатионвалуетекст
description: Создание нового объекта Граупполиципресентатионвалуетекст.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9890920cc0912cb51f2856dcb55ac2e2d6543554
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305983"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="8b07e-103">Создание Граупполиципресентатионвалуетекст</span><span class="sxs-lookup"><span data-stu-id="8b07e-103">Create groupPolicyPresentationValueText</span></span>

<span data-ttu-id="8b07e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b07e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b07e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b07e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b07e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b07e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b07e-107">Создание нового объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="8b07e-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b07e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b07e-108">Prerequisites</span></span>
<span data-ttu-id="8b07e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b07e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b07e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b07e-111">Permission type</span></span>|<span data-ttu-id="8b07e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b07e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b07e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b07e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b07e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b07e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b07e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b07e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b07e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b07e-116">Not supported.</span></span>|
|<span data-ttu-id="8b07e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b07e-117">Application</span></span>|<span data-ttu-id="8b07e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b07e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b07e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b07e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="8b07e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b07e-120">Request headers</span></span>
|<span data-ttu-id="8b07e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b07e-121">Header</span></span>|<span data-ttu-id="8b07e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b07e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b07e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b07e-123">Authorization</span></span>|<span data-ttu-id="8b07e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b07e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b07e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b07e-125">Accept</span></span>|<span data-ttu-id="8b07e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b07e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b07e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b07e-127">Request body</span></span>
<span data-ttu-id="8b07e-128">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуетекст в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b07e-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="8b07e-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуетекст.</span><span class="sxs-lookup"><span data-stu-id="8b07e-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="8b07e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b07e-130">Property</span></span>|<span data-ttu-id="8b07e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b07e-131">Type</span></span>|<span data-ttu-id="8b07e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b07e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b07e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b07e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8b07e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b07e-134">DateTimeOffset</span></span>|<span data-ttu-id="8b07e-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8b07e-135">The date and time the object was last modified.</span></span> <span data-ttu-id="8b07e-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8b07e-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8b07e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b07e-137">createdDateTime</span></span>|<span data-ttu-id="8b07e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b07e-138">DateTimeOffset</span></span>|<span data-ttu-id="8b07e-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8b07e-139">The date and time the object was created.</span></span> <span data-ttu-id="8b07e-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8b07e-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8b07e-141">id</span><span class="sxs-lookup"><span data-stu-id="8b07e-141">id</span></span>|<span data-ttu-id="8b07e-142">String</span><span class="sxs-lookup"><span data-stu-id="8b07e-142">String</span></span>|<span data-ttu-id="8b07e-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b07e-143">Key of the entity.</span></span> <span data-ttu-id="8b07e-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8b07e-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="8b07e-145">value</span><span class="sxs-lookup"><span data-stu-id="8b07e-145">value</span></span>|<span data-ttu-id="8b07e-146">String</span><span class="sxs-lookup"><span data-stu-id="8b07e-146">String</span></span>|<span data-ttu-id="8b07e-147">Строковое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="8b07e-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="8b07e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b07e-148">Response</span></span>
<span data-ttu-id="8b07e-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b07e-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b07e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="8b07e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b07e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b07e-151">Request</span></span>
<span data-ttu-id="8b07e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b07e-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="8b07e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b07e-153">Response</span></span>
<span data-ttu-id="8b07e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b07e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




