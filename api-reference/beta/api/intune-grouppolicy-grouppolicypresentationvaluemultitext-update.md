---
title: Обновление Граупполиципресентатионвалуемултитекст
description: Обновление свойств объекта Граупполиципресентатионвалуемултитекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88fb4432b0e634b0babe91e7fb77cc96c9e66b16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463975"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="5ba11-103">Обновление Граупполиципресентатионвалуемултитекст</span><span class="sxs-lookup"><span data-stu-id="5ba11-103">Update groupPolicyPresentationValueMultiText</span></span>

<span data-ttu-id="5ba11-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ba11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ba11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ba11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ba11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ba11-107">Обновление свойств объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="5ba11-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ba11-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ba11-108">Prerequisites</span></span>
<span data-ttu-id="5ba11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ba11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ba11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba11-111">Permission type</span></span>|<span data-ttu-id="5ba11-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ba11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ba11-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ba11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ba11-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba11-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ba11-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ba11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ba11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ba11-116">Not supported.</span></span>|
|<span data-ttu-id="5ba11-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ba11-117">Application</span></span>|<span data-ttu-id="5ba11-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba11-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ba11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ba11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="5ba11-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ba11-120">Request headers</span></span>
|<span data-ttu-id="5ba11-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ba11-121">Header</span></span>|<span data-ttu-id="5ba11-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ba11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ba11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ba11-123">Authorization</span></span>|<span data-ttu-id="5ba11-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ba11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ba11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ba11-125">Accept</span></span>|<span data-ttu-id="5ba11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ba11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ba11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ba11-127">Request body</span></span>
<span data-ttu-id="5ba11-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ba11-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="5ba11-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span><span class="sxs-lookup"><span data-stu-id="5ba11-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="5ba11-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ba11-130">Property</span></span>|<span data-ttu-id="5ba11-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ba11-131">Type</span></span>|<span data-ttu-id="5ba11-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ba11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ba11-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ba11-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5ba11-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ba11-134">DateTimeOffset</span></span>|<span data-ttu-id="5ba11-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5ba11-135">The date and time the object was last modified.</span></span> <span data-ttu-id="5ba11-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5ba11-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5ba11-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ba11-137">createdDateTime</span></span>|<span data-ttu-id="5ba11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ba11-138">DateTimeOffset</span></span>|<span data-ttu-id="5ba11-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5ba11-139">The date and time the object was created.</span></span> <span data-ttu-id="5ba11-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5ba11-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5ba11-141">id</span><span class="sxs-lookup"><span data-stu-id="5ba11-141">id</span></span>|<span data-ttu-id="5ba11-142">String</span><span class="sxs-lookup"><span data-stu-id="5ba11-142">String</span></span>|<span data-ttu-id="5ba11-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ba11-143">Key of the entity.</span></span> <span data-ttu-id="5ba11-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5ba11-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5ba11-145">values</span><span class="sxs-lookup"><span data-stu-id="5ba11-145">values</span></span>|<span data-ttu-id="5ba11-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ba11-146">String collection</span></span>|<span data-ttu-id="5ba11-147">Коллекция непустых строк для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="5ba11-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="5ba11-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ba11-148">Response</span></span>
<span data-ttu-id="5ba11-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ba11-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ba11-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5ba11-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ba11-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ba11-151">Request</span></span>
<span data-ttu-id="5ba11-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ba11-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5ba11-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ba11-153">Response</span></span>
<span data-ttu-id="5ba11-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ba11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```





