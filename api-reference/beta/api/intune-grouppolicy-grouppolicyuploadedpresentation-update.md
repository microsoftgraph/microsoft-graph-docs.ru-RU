---
title: Обновление groupPolicyUploadedPresentation
description: Обновление свойств объекта groupPolicyUploadedPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd427ea574e8abe971863954c5817321eea14115
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145539"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="3199e-103">Обновление groupPolicyUploadedPresentation</span><span class="sxs-lookup"><span data-stu-id="3199e-103">Update groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="3199e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3199e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3199e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3199e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3199e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3199e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3199e-107">Обновление свойств объекта [groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-107">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3199e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3199e-108">Prerequisites</span></span>
<span data-ttu-id="3199e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3199e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3199e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3199e-111">Permission type</span></span>|<span data-ttu-id="3199e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3199e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3199e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3199e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3199e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3199e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3199e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3199e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3199e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3199e-116">Not supported.</span></span>|
|<span data-ttu-id="3199e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3199e-117">Application</span></span>|<span data-ttu-id="3199e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3199e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3199e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3199e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="3199e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3199e-120">Request headers</span></span>
|<span data-ttu-id="3199e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3199e-121">Header</span></span>|<span data-ttu-id="3199e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3199e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3199e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3199e-123">Authorization</span></span>|<span data-ttu-id="3199e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3199e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3199e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3199e-125">Accept</span></span>|<span data-ttu-id="3199e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3199e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3199e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3199e-127">Request body</span></span>
<span data-ttu-id="3199e-128">В теле запроса поставляем представление JSON для [объекта groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-128">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="3199e-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-129">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="3199e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3199e-130">Property</span></span>|<span data-ttu-id="3199e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3199e-131">Type</span></span>|<span data-ttu-id="3199e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3199e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3199e-133">label</span><span class="sxs-lookup"><span data-stu-id="3199e-133">label</span></span>|<span data-ttu-id="3199e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3199e-134">String</span></span>|<span data-ttu-id="3199e-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="3199e-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3199e-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="3199e-136">The default value is empty.</span></span> <span data-ttu-id="3199e-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3199e-138">id</span><span class="sxs-lookup"><span data-stu-id="3199e-138">id</span></span>|<span data-ttu-id="3199e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3199e-139">String</span></span>|<span data-ttu-id="3199e-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3199e-140">Key of the entity.</span></span> <span data-ttu-id="3199e-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3199e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3199e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3199e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3199e-143">DateTimeOffset</span></span>|<span data-ttu-id="3199e-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3199e-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="3199e-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3199e-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3199e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3199e-146">Response</span></span>
<span data-ttu-id="3199e-147">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3199e-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3199e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3199e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3199e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3199e-149">Request</span></span>
<span data-ttu-id="3199e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3199e-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="3199e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3199e-151">Response</span></span>
<span data-ttu-id="3199e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3199e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value",
  "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




