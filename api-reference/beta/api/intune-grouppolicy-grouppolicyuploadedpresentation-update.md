---
title: Обновление Граупполициуплоадедпресентатион
description: Обновление свойств объекта Граупполициуплоадедпресентатион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 244cc9206679416cdfee4c7aee61d68b3de4de44
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803703"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="2a98c-103">Обновление Граупполициуплоадедпресентатион</span><span class="sxs-lookup"><span data-stu-id="2a98c-103">Update groupPolicyUploadedPresentation</span></span>

> <span data-ttu-id="2a98c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a98c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a98c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a98c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a98c-106">Обновление свойств объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="2a98c-106">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a98c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a98c-107">Prerequisites</span></span>
<span data-ttu-id="2a98c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a98c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a98c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a98c-110">Permission type</span></span>|<span data-ttu-id="2a98c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a98c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a98c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a98c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a98c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a98c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a98c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a98c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a98c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a98c-115">Not supported.</span></span>|
|<span data-ttu-id="2a98c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a98c-116">Application</span></span>|<span data-ttu-id="2a98c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a98c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a98c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a98c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a98c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a98c-119">Request headers</span></span>
|<span data-ttu-id="2a98c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a98c-120">Header</span></span>|<span data-ttu-id="2a98c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a98c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a98c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a98c-122">Authorization</span></span>|<span data-ttu-id="2a98c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a98c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a98c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a98c-124">Accept</span></span>|<span data-ttu-id="2a98c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a98c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a98c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a98c-126">Request body</span></span>
<span data-ttu-id="2a98c-127">В тексте запроса добавьте представление объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a98c-127">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="2a98c-128">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="2a98c-128">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="2a98c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a98c-129">Property</span></span>|<span data-ttu-id="2a98c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a98c-130">Type</span></span>|<span data-ttu-id="2a98c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a98c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a98c-132">label</span><span class="sxs-lookup"><span data-stu-id="2a98c-132">label</span></span>|<span data-ttu-id="2a98c-133">String</span><span class="sxs-lookup"><span data-stu-id="2a98c-133">String</span></span>|<span data-ttu-id="2a98c-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="2a98c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="2a98c-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="2a98c-135">The default value is empty.</span></span> <span data-ttu-id="2a98c-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a98c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2a98c-137">id</span><span class="sxs-lookup"><span data-stu-id="2a98c-137">id</span></span>|<span data-ttu-id="2a98c-138">String</span><span class="sxs-lookup"><span data-stu-id="2a98c-138">String</span></span>|<span data-ttu-id="2a98c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a98c-139">Key of the entity.</span></span> <span data-ttu-id="2a98c-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a98c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2a98c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a98c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2a98c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a98c-142">DateTimeOffset</span></span>|<span data-ttu-id="2a98c-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2a98c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="2a98c-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a98c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2a98c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a98c-145">Response</span></span>
<span data-ttu-id="2a98c-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a98c-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a98c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2a98c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a98c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a98c-148">Request</span></span>
<span data-ttu-id="2a98c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a98c-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="2a98c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a98c-150">Response</span></span>
<span data-ttu-id="2a98c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a98c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




