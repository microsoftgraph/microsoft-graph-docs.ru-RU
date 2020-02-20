---
title: Создание Граупполициуплоадедпресентатион
description: Создание нового объекта Граупполициуплоадедпресентатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db3f441395a2cb541b03ae8042f68b4b23e13afc
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161760"
---
# <a name="create-grouppolicyuploadedpresentation"></a><span data-ttu-id="bb54b-103">Создание Граупполициуплоадедпресентатион</span><span class="sxs-lookup"><span data-stu-id="bb54b-103">Create groupPolicyUploadedPresentation</span></span>

> <span data-ttu-id="bb54b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb54b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb54b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb54b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb54b-106">Создание нового объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb54b-106">Create a new [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb54b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb54b-107">Prerequisites</span></span>
<span data-ttu-id="bb54b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb54b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb54b-110">Permission type</span></span>|<span data-ttu-id="bb54b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb54b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb54b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb54b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb54b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb54b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bb54b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb54b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb54b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb54b-115">Not supported.</span></span>|
|<span data-ttu-id="bb54b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb54b-116">Application</span></span>|<span data-ttu-id="bb54b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb54b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb54b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb54b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="bb54b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb54b-119">Request headers</span></span>
|<span data-ttu-id="bb54b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb54b-120">Header</span></span>|<span data-ttu-id="bb54b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bb54b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb54b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb54b-122">Authorization</span></span>|<span data-ttu-id="bb54b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb54b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb54b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb54b-124">Accept</span></span>|<span data-ttu-id="bb54b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb54b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb54b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb54b-126">Request body</span></span>
<span data-ttu-id="bb54b-127">В тексте запроса добавьте представление объекта Граупполициуплоадедпресентатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb54b-127">In the request body, supply a JSON representation for the groupPolicyUploadedPresentation object.</span></span>

<span data-ttu-id="bb54b-128">В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадедпресентатион.</span><span class="sxs-lookup"><span data-stu-id="bb54b-128">The following table shows the properties that are required when you create the groupPolicyUploadedPresentation.</span></span>

|<span data-ttu-id="bb54b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb54b-129">Property</span></span>|<span data-ttu-id="bb54b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb54b-130">Type</span></span>|<span data-ttu-id="bb54b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb54b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb54b-132">label</span><span class="sxs-lookup"><span data-stu-id="bb54b-132">label</span></span>|<span data-ttu-id="bb54b-133">String</span><span class="sxs-lookup"><span data-stu-id="bb54b-133">String</span></span>|<span data-ttu-id="bb54b-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="bb54b-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bb54b-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="bb54b-135">The default value is empty.</span></span> <span data-ttu-id="bb54b-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bb54b-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bb54b-137">id</span><span class="sxs-lookup"><span data-stu-id="bb54b-137">id</span></span>|<span data-ttu-id="bb54b-138">String</span><span class="sxs-lookup"><span data-stu-id="bb54b-138">String</span></span>|<span data-ttu-id="bb54b-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb54b-139">Key of the entity.</span></span> <span data-ttu-id="bb54b-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bb54b-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bb54b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb54b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bb54b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb54b-142">DateTimeOffset</span></span>|<span data-ttu-id="bb54b-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bb54b-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="bb54b-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bb54b-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bb54b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb54b-145">Response</span></span>
<span data-ttu-id="bb54b-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb54b-146">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb54b-147">Пример</span><span class="sxs-lookup"><span data-stu-id="bb54b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb54b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb54b-148">Request</span></span>
<span data-ttu-id="bb54b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb54b-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="bb54b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb54b-150">Response</span></span>
<span data-ttu-id="bb54b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb54b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value",
  "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





