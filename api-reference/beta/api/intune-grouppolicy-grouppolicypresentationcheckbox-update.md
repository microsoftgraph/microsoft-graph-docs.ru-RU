---
title: Обновление Граупполиципресентатиончеккбокс
description: Обновление свойств объекта Граупполиципресентатиончеккбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ad76e25204bfeefb5ba80087f2c85f2cb40b17f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357931"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="940fc-103">Обновление Граупполиципресентатиончеккбокс</span><span class="sxs-lookup"><span data-stu-id="940fc-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="940fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="940fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="940fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="940fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940fc-106">Обновление свойств объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="940fc-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="940fc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="940fc-107">Prerequisites</span></span>
<span data-ttu-id="940fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="940fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="940fc-110">Permission type</span></span>|<span data-ttu-id="940fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="940fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="940fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="940fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="940fc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940fc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="940fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="940fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="940fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="940fc-115">Not supported.</span></span>|
|<span data-ttu-id="940fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="940fc-116">Application</span></span>|<span data-ttu-id="940fc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940fc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="940fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="940fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="940fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="940fc-119">Request headers</span></span>
|<span data-ttu-id="940fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="940fc-120">Header</span></span>|<span data-ttu-id="940fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="940fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="940fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="940fc-122">Authorization</span></span>|<span data-ttu-id="940fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="940fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="940fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="940fc-124">Accept</span></span>|<span data-ttu-id="940fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="940fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="940fc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="940fc-126">Request body</span></span>
<span data-ttu-id="940fc-127">В тексте запроса добавьте представление объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="940fc-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="940fc-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="940fc-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="940fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="940fc-129">Property</span></span>|<span data-ttu-id="940fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="940fc-130">Type</span></span>|<span data-ttu-id="940fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="940fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940fc-132">label</span><span class="sxs-lookup"><span data-stu-id="940fc-132">label</span></span>|<span data-ttu-id="940fc-133">String</span><span class="sxs-lookup"><span data-stu-id="940fc-133">String</span></span>|<span data-ttu-id="940fc-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="940fc-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="940fc-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="940fc-135">The default value is empty.</span></span> <span data-ttu-id="940fc-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="940fc-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="940fc-137">id</span><span class="sxs-lookup"><span data-stu-id="940fc-137">id</span></span>|<span data-ttu-id="940fc-138">String</span><span class="sxs-lookup"><span data-stu-id="940fc-138">String</span></span>|<span data-ttu-id="940fc-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="940fc-139">Key of the entity.</span></span> <span data-ttu-id="940fc-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="940fc-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="940fc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="940fc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="940fc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="940fc-142">DateTimeOffset</span></span>|<span data-ttu-id="940fc-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="940fc-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="940fc-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="940fc-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="940fc-145">дефаултчеккед</span><span class="sxs-lookup"><span data-stu-id="940fc-145">defaultChecked</span></span>|<span data-ttu-id="940fc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="940fc-146">Boolean</span></span>|<span data-ttu-id="940fc-147">Значение по умолчанию для этого флажка.</span><span class="sxs-lookup"><span data-stu-id="940fc-147">Default value for the check box.</span></span> <span data-ttu-id="940fc-148">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="940fc-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="940fc-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="940fc-149">Response</span></span>
<span data-ttu-id="940fc-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="940fc-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="940fc-151">Пример</span><span class="sxs-lookup"><span data-stu-id="940fc-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="940fc-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="940fc-152">Request</span></span>
<span data-ttu-id="940fc-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="940fc-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="940fc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="940fc-154">Response</span></span>
<span data-ttu-id="940fc-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="940fc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```






