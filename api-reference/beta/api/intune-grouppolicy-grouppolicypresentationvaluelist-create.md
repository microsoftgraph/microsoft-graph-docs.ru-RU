---
title: Создание groupPolicyPresentationValueList
description: Создайте новый объект groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b70dc810050e9c6ebbe46a6d9af2f5ea5a9b3d31
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153239"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="17911-103">Создание groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="17911-103">Create groupPolicyPresentationValueList</span></span>

<span data-ttu-id="17911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17911-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17911-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17911-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17911-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17911-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17911-107">Создайте новый [объект groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="17911-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17911-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17911-108">Prerequisites</span></span>
<span data-ttu-id="17911-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17911-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17911-111">Permission type</span></span>|<span data-ttu-id="17911-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17911-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17911-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17911-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17911-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17911-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17911-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17911-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17911-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17911-116">Not supported.</span></span>|
|<span data-ttu-id="17911-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17911-117">Application</span></span>|<span data-ttu-id="17911-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17911-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17911-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17911-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="17911-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17911-120">Request headers</span></span>
|<span data-ttu-id="17911-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17911-121">Header</span></span>|<span data-ttu-id="17911-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17911-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17911-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17911-123">Authorization</span></span>|<span data-ttu-id="17911-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17911-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17911-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17911-125">Accept</span></span>|<span data-ttu-id="17911-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17911-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17911-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17911-127">Request body</span></span>
<span data-ttu-id="17911-128">В теле запроса поставляем представление JSON для объекта groupPolicyPresentationValueList.</span><span class="sxs-lookup"><span data-stu-id="17911-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="17911-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationValueList.</span><span class="sxs-lookup"><span data-stu-id="17911-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="17911-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17911-130">Property</span></span>|<span data-ttu-id="17911-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17911-131">Type</span></span>|<span data-ttu-id="17911-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17911-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17911-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17911-133">lastModifiedDateTime</span></span>|<span data-ttu-id="17911-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17911-134">DateTimeOffset</span></span>|<span data-ttu-id="17911-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="17911-135">The date and time the object was last modified.</span></span> <span data-ttu-id="17911-136">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="17911-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="17911-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17911-137">createdDateTime</span></span>|<span data-ttu-id="17911-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17911-138">DateTimeOffset</span></span>|<span data-ttu-id="17911-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="17911-139">The date and time the object was created.</span></span> <span data-ttu-id="17911-140">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="17911-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="17911-141">id</span><span class="sxs-lookup"><span data-stu-id="17911-141">id</span></span>|<span data-ttu-id="17911-142">Строка</span><span class="sxs-lookup"><span data-stu-id="17911-142">String</span></span>|<span data-ttu-id="17911-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17911-143">Key of the entity.</span></span> <span data-ttu-id="17911-144">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="17911-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="17911-145">values</span><span class="sxs-lookup"><span data-stu-id="17911-145">values</span></span>|<span data-ttu-id="17911-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="17911-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="17911-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="17911-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="17911-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="17911-148">Response</span></span>
<span data-ttu-id="17911-149">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="17911-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17911-150">Пример</span><span class="sxs-lookup"><span data-stu-id="17911-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="17911-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="17911-151">Request</span></span>
<span data-ttu-id="17911-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17911-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17911-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="17911-153">Response</span></span>
<span data-ttu-id="17911-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17911-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




