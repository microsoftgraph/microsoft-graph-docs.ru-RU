---
title: Обновление Граупполиципресентатиончеккбокс
description: Обновление свойств объекта Граупполиципресентатиончеккбокс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26de37d645174d60dbfaf0717f236ec15ce0f31e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804333"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="f0248-103">Обновление Граупполиципресентатиончеккбокс</span><span class="sxs-lookup"><span data-stu-id="f0248-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="f0248-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0248-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0248-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0248-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0248-106">Обновление свойств объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="f0248-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0248-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0248-107">Prerequisites</span></span>
<span data-ttu-id="f0248-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0248-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0248-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0248-110">Permission type</span></span>|<span data-ttu-id="f0248-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0248-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0248-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0248-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0248-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0248-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0248-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0248-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0248-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0248-115">Not supported.</span></span>|
|<span data-ttu-id="f0248-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0248-116">Application</span></span>|<span data-ttu-id="f0248-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0248-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0248-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0248-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f0248-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0248-119">Request headers</span></span>
|<span data-ttu-id="f0248-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0248-120">Header</span></span>|<span data-ttu-id="f0248-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0248-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0248-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0248-122">Authorization</span></span>|<span data-ttu-id="f0248-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0248-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0248-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f0248-124">Accept</span></span>|<span data-ttu-id="f0248-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0248-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0248-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0248-126">Request body</span></span>
<span data-ttu-id="f0248-127">В тексте запроса добавьте представление объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0248-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="f0248-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="f0248-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="f0248-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0248-129">Property</span></span>|<span data-ttu-id="f0248-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f0248-130">Type</span></span>|<span data-ttu-id="f0248-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f0248-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0248-132">label</span><span class="sxs-lookup"><span data-stu-id="f0248-132">label</span></span>|<span data-ttu-id="f0248-133">String</span><span class="sxs-lookup"><span data-stu-id="f0248-133">String</span></span>|<span data-ttu-id="f0248-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="f0248-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f0248-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="f0248-135">The default value is empty.</span></span> <span data-ttu-id="f0248-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f0248-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f0248-137">id</span><span class="sxs-lookup"><span data-stu-id="f0248-137">id</span></span>|<span data-ttu-id="f0248-138">String</span><span class="sxs-lookup"><span data-stu-id="f0248-138">String</span></span>|<span data-ttu-id="f0248-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0248-139">Key of the entity.</span></span> <span data-ttu-id="f0248-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f0248-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f0248-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0248-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f0248-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0248-142">DateTimeOffset</span></span>|<span data-ttu-id="f0248-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f0248-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="f0248-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f0248-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f0248-145">дефаултчеккед</span><span class="sxs-lookup"><span data-stu-id="f0248-145">defaultChecked</span></span>|<span data-ttu-id="f0248-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f0248-146">Boolean</span></span>|<span data-ttu-id="f0248-147">Значение по умолчанию для этого флажка.</span><span class="sxs-lookup"><span data-stu-id="f0248-147">Default value for the check box.</span></span> <span data-ttu-id="f0248-148">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="f0248-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="f0248-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0248-149">Response</span></span>
<span data-ttu-id="f0248-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0248-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0248-151">Пример</span><span class="sxs-lookup"><span data-stu-id="f0248-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0248-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0248-152">Request</span></span>
<span data-ttu-id="f0248-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0248-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0248-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0248-154">Response</span></span>
<span data-ttu-id="f0248-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0248-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




