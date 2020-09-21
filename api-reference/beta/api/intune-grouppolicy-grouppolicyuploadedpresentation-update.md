---
title: Обновление Граупполициуплоадедпресентатион
description: Обновление свойств объекта Граупполициуплоадедпресентатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 424dbe80fbfcbed2df86963b9c00019ca8df2a58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000380"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="bdfc4-103">Обновление Граупполициуплоадедпресентатион</span><span class="sxs-lookup"><span data-stu-id="bdfc4-103">Update groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="bdfc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdfc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdfc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdfc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdfc4-107">Обновление свойств объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="bdfc4-107">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdfc4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bdfc4-108">Prerequisites</span></span>
<span data-ttu-id="bdfc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdfc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdfc4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdfc4-111">Permission type</span></span>|<span data-ttu-id="bdfc4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdfc4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdfc4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdfc4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdfc4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdfc4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-116">Not supported.</span></span>|
|<span data-ttu-id="bdfc4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdfc4-117">Application</span></span>|<span data-ttu-id="bdfc4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdfc4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdfc4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdfc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="bdfc4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bdfc4-120">Request headers</span></span>
|<span data-ttu-id="bdfc4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdfc4-121">Header</span></span>|<span data-ttu-id="bdfc4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdfc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdfc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdfc4-123">Authorization</span></span>|<span data-ttu-id="bdfc4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdfc4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdfc4-125">Accept</span></span>|<span data-ttu-id="bdfc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdfc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdfc4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdfc4-127">Request body</span></span>
<span data-ttu-id="bdfc4-128">В тексте запроса добавьте представление объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-128">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="bdfc4-129">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="bdfc4-129">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="bdfc4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdfc4-130">Property</span></span>|<span data-ttu-id="bdfc4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bdfc4-131">Type</span></span>|<span data-ttu-id="bdfc4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bdfc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfc4-133">label</span><span class="sxs-lookup"><span data-stu-id="bdfc4-133">label</span></span>|<span data-ttu-id="bdfc4-134">String</span><span class="sxs-lookup"><span data-stu-id="bdfc4-134">String</span></span>|<span data-ttu-id="bdfc4-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bdfc4-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-136">The default value is empty.</span></span> <span data-ttu-id="bdfc4-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bdfc4-138">id</span><span class="sxs-lookup"><span data-stu-id="bdfc4-138">id</span></span>|<span data-ttu-id="bdfc4-139">String</span><span class="sxs-lookup"><span data-stu-id="bdfc4-139">String</span></span>|<span data-ttu-id="bdfc4-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-140">Key of the entity.</span></span> <span data-ttu-id="bdfc4-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bdfc4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdfc4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bdfc4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdfc4-143">DateTimeOffset</span></span>|<span data-ttu-id="bdfc4-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="bdfc4-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bdfc4-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bdfc4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdfc4-146">Response</span></span>
<span data-ttu-id="bdfc4-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdfc4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="bdfc4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdfc4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdfc4-149">Request</span></span>
<span data-ttu-id="bdfc4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="bdfc4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdfc4-151">Response</span></span>
<span data-ttu-id="bdfc4-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdfc4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






