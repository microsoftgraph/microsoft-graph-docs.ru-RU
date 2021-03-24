---
title: Обновление groupPolicyPresentationValueList
description: Обновление свойств объекта groupPolicyPresentationValueList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46f7658a559098ece77d880d2c43e894b27dc95c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125998"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="50d19-103">Обновление groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="50d19-103">Update groupPolicyPresentationValueList</span></span>

<span data-ttu-id="50d19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50d19-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50d19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50d19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50d19-107">Обновление свойств объекта [groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-107">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50d19-108">Prerequisites</span></span>
<span data-ttu-id="50d19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50d19-111">Permission type</span></span>|<span data-ttu-id="50d19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50d19-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50d19-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50d19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50d19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50d19-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50d19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50d19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d19-116">Not supported.</span></span>|
|<span data-ttu-id="50d19-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="50d19-117">Application</span></span>|<span data-ttu-id="50d19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50d19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="50d19-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50d19-120">Request headers</span></span>
|<span data-ttu-id="50d19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50d19-121">Header</span></span>|<span data-ttu-id="50d19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50d19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50d19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50d19-123">Authorization</span></span>|<span data-ttu-id="50d19-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50d19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50d19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50d19-125">Accept</span></span>|<span data-ttu-id="50d19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50d19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d19-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50d19-127">Request body</span></span>
<span data-ttu-id="50d19-128">В теле запроса поставляем представление JSON для [объекта groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="50d19-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationValueList.](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="50d19-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50d19-130">Property</span></span>|<span data-ttu-id="50d19-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50d19-131">Type</span></span>|<span data-ttu-id="50d19-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50d19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50d19-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50d19-133">lastModifiedDateTime</span></span>|<span data-ttu-id="50d19-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d19-134">DateTimeOffset</span></span>|<span data-ttu-id="50d19-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="50d19-135">The date and time the object was last modified.</span></span> <span data-ttu-id="50d19-136">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="50d19-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50d19-137">createdDateTime</span></span>|<span data-ttu-id="50d19-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d19-138">DateTimeOffset</span></span>|<span data-ttu-id="50d19-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="50d19-139">The date and time the object was created.</span></span> <span data-ttu-id="50d19-140">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="50d19-141">id</span><span class="sxs-lookup"><span data-stu-id="50d19-141">id</span></span>|<span data-ttu-id="50d19-142">Строка</span><span class="sxs-lookup"><span data-stu-id="50d19-142">String</span></span>|<span data-ttu-id="50d19-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50d19-143">Key of the entity.</span></span> <span data-ttu-id="50d19-144">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="50d19-145">values</span><span class="sxs-lookup"><span data-stu-id="50d19-145">values</span></span>|<span data-ttu-id="50d19-146">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="50d19-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="50d19-147">Список пар для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="50d19-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="50d19-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="50d19-148">Response</span></span>
<span data-ttu-id="50d19-149">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="50d19-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d19-150">Пример</span><span class="sxs-lookup"><span data-stu-id="50d19-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d19-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="50d19-151">Request</span></span>
<span data-ttu-id="50d19-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50d19-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50d19-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="50d19-153">Response</span></span>
<span data-ttu-id="50d19-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50d19-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




