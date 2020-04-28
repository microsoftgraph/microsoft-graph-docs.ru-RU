---
title: Обновление Граупполиципресентатиончеккбокс
description: Обновление свойств объекта Граупполиципресентатиончеккбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 013bd2aefe44da044f382ebfec3754b111dfebef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377934"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="5299c-103">Обновление Граупполиципресентатиончеккбокс</span><span class="sxs-lookup"><span data-stu-id="5299c-103">Update groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="5299c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5299c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5299c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5299c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5299c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5299c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5299c-107">Обновление свойств объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="5299c-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5299c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5299c-108">Prerequisites</span></span>
<span data-ttu-id="5299c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5299c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5299c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5299c-111">Permission type</span></span>|<span data-ttu-id="5299c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5299c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5299c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5299c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5299c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5299c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5299c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5299c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5299c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5299c-116">Not supported.</span></span>|
|<span data-ttu-id="5299c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5299c-117">Application</span></span>|<span data-ttu-id="5299c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5299c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5299c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5299c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="5299c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5299c-120">Request headers</span></span>
|<span data-ttu-id="5299c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5299c-121">Header</span></span>|<span data-ttu-id="5299c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5299c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5299c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5299c-123">Authorization</span></span>|<span data-ttu-id="5299c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5299c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5299c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5299c-125">Accept</span></span>|<span data-ttu-id="5299c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5299c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5299c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5299c-127">Request body</span></span>
<span data-ttu-id="5299c-128">В тексте запроса добавьте представление объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5299c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="5299c-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="5299c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="5299c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5299c-130">Property</span></span>|<span data-ttu-id="5299c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5299c-131">Type</span></span>|<span data-ttu-id="5299c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5299c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5299c-133">label</span><span class="sxs-lookup"><span data-stu-id="5299c-133">label</span></span>|<span data-ttu-id="5299c-134">String</span><span class="sxs-lookup"><span data-stu-id="5299c-134">String</span></span>|<span data-ttu-id="5299c-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="5299c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="5299c-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="5299c-136">The default value is empty.</span></span> <span data-ttu-id="5299c-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5299c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5299c-138">id</span><span class="sxs-lookup"><span data-stu-id="5299c-138">id</span></span>|<span data-ttu-id="5299c-139">String</span><span class="sxs-lookup"><span data-stu-id="5299c-139">String</span></span>|<span data-ttu-id="5299c-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5299c-140">Key of the entity.</span></span> <span data-ttu-id="5299c-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5299c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5299c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5299c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="5299c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5299c-143">DateTimeOffset</span></span>|<span data-ttu-id="5299c-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5299c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="5299c-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5299c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5299c-146">дефаултчеккед</span><span class="sxs-lookup"><span data-stu-id="5299c-146">defaultChecked</span></span>|<span data-ttu-id="5299c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5299c-147">Boolean</span></span>|<span data-ttu-id="5299c-148">Значение по умолчанию для этого флажка.</span><span class="sxs-lookup"><span data-stu-id="5299c-148">Default value for the check box.</span></span> <span data-ttu-id="5299c-149">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="5299c-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="5299c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5299c-150">Response</span></span>
<span data-ttu-id="5299c-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5299c-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5299c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="5299c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="5299c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5299c-153">Request</span></span>
<span data-ttu-id="5299c-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5299c-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5299c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5299c-155">Response</span></span>
<span data-ttu-id="5299c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5299c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



