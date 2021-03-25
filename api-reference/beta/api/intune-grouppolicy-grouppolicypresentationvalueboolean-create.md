---
title: Создание groupPolicyPresentationValueBoolean
description: Создайте новый объект groupPolicyPresentationValueBoolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 204ab6e117cd6a5b6f1e4084fd3673b403ba4e56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157330"
---
# <a name="create-grouppolicypresentationvalueboolean"></a><span data-ttu-id="aae1c-103">Создание groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="aae1c-103">Create groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="aae1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aae1c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aae1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aae1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aae1c-107">Создайте новый [объект groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)</span><span class="sxs-lookup"><span data-stu-id="aae1c-107">Create a new [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aae1c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aae1c-108">Prerequisites</span></span>
<span data-ttu-id="aae1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aae1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae1c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aae1c-111">Permission type</span></span>|<span data-ttu-id="aae1c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aae1c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aae1c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aae1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aae1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aae1c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aae1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aae1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae1c-116">Not supported.</span></span>|
|<span data-ttu-id="aae1c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aae1c-117">Application</span></span>|<span data-ttu-id="aae1c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae1c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aae1c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aae1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="aae1c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aae1c-120">Request headers</span></span>
|<span data-ttu-id="aae1c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aae1c-121">Header</span></span>|<span data-ttu-id="aae1c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aae1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aae1c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae1c-123">Authorization</span></span>|<span data-ttu-id="aae1c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aae1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aae1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aae1c-125">Accept</span></span>|<span data-ttu-id="aae1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aae1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aae1c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aae1c-127">Request body</span></span>
<span data-ttu-id="aae1c-128">В теле запроса поставляем представление JSON для объекта GroupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="aae1c-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueBoolean object.</span></span>

<span data-ttu-id="aae1c-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationValueBoolean.</span><span class="sxs-lookup"><span data-stu-id="aae1c-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueBoolean.</span></span>

|<span data-ttu-id="aae1c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aae1c-130">Property</span></span>|<span data-ttu-id="aae1c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aae1c-131">Type</span></span>|<span data-ttu-id="aae1c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aae1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae1c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae1c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="aae1c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae1c-134">DateTimeOffset</span></span>|<span data-ttu-id="aae1c-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aae1c-135">The date and time the object was last modified.</span></span> <span data-ttu-id="aae1c-136">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="aae1c-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="aae1c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aae1c-137">createdDateTime</span></span>|<span data-ttu-id="aae1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae1c-138">DateTimeOffset</span></span>|<span data-ttu-id="aae1c-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aae1c-139">The date and time the object was created.</span></span> <span data-ttu-id="aae1c-140">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="aae1c-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="aae1c-141">id</span><span class="sxs-lookup"><span data-stu-id="aae1c-141">id</span></span>|<span data-ttu-id="aae1c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="aae1c-142">String</span></span>|<span data-ttu-id="aae1c-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aae1c-143">Key of the entity.</span></span> <span data-ttu-id="aae1c-144">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="aae1c-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="aae1c-145">value</span><span class="sxs-lookup"><span data-stu-id="aae1c-145">value</span></span>|<span data-ttu-id="aae1c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aae1c-146">Boolean</span></span>|<span data-ttu-id="aae1c-147">Значение boolean для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="aae1c-147">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="aae1c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae1c-148">Response</span></span>
<span data-ttu-id="aae1c-149">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aae1c-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aae1c-150">Пример</span><span class="sxs-lookup"><span data-stu-id="aae1c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="aae1c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="aae1c-151">Request</span></span>
<span data-ttu-id="aae1c-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aae1c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="aae1c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae1c-153">Response</span></span>
<span data-ttu-id="aae1c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aae1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




