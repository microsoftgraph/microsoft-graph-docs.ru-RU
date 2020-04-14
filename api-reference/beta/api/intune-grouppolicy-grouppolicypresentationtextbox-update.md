---
title: Обновление Граупполиципресентатионтекстбокс
description: Обновление свойств объекта Граупполиципресентатионтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50d47df3474669f8d086f3b18cf9f2c34f5d6f1f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461112"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="cac0f-103">Обновление Граупполиципресентатионтекстбокс</span><span class="sxs-lookup"><span data-stu-id="cac0f-103">Update groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="cac0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cac0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cac0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cac0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac0f-107">Обновление свойств объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="cac0f-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cac0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cac0f-108">Prerequisites</span></span>
<span data-ttu-id="cac0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cac0f-111">Permission type</span></span>|<span data-ttu-id="cac0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cac0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cac0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cac0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cac0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cac0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cac0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac0f-116">Not supported.</span></span>|
|<span data-ttu-id="cac0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cac0f-117">Application</span></span>|<span data-ttu-id="cac0f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac0f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cac0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cac0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="cac0f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cac0f-120">Request headers</span></span>
|<span data-ttu-id="cac0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cac0f-121">Header</span></span>|<span data-ttu-id="cac0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cac0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cac0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac0f-123">Authorization</span></span>|<span data-ttu-id="cac0f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cac0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cac0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cac0f-125">Accept</span></span>|<span data-ttu-id="cac0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cac0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac0f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cac0f-127">Request body</span></span>
<span data-ttu-id="cac0f-128">В тексте запроса добавьте представление объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cac0f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="cac0f-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span><span class="sxs-lookup"><span data-stu-id="cac0f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="cac0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cac0f-130">Property</span></span>|<span data-ttu-id="cac0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cac0f-131">Type</span></span>|<span data-ttu-id="cac0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cac0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac0f-133">label</span><span class="sxs-lookup"><span data-stu-id="cac0f-133">label</span></span>|<span data-ttu-id="cac0f-134">String</span><span class="sxs-lookup"><span data-stu-id="cac0f-134">String</span></span>|<span data-ttu-id="cac0f-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="cac0f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cac0f-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="cac0f-136">The default value is empty.</span></span> <span data-ttu-id="cac0f-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cac0f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cac0f-138">id</span><span class="sxs-lookup"><span data-stu-id="cac0f-138">id</span></span>|<span data-ttu-id="cac0f-139">String</span><span class="sxs-lookup"><span data-stu-id="cac0f-139">String</span></span>|<span data-ttu-id="cac0f-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cac0f-140">Key of the entity.</span></span> <span data-ttu-id="cac0f-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cac0f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cac0f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cac0f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="cac0f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cac0f-143">DateTimeOffset</span></span>|<span data-ttu-id="cac0f-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cac0f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="cac0f-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cac0f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cac0f-146">Значение</span><span class="sxs-lookup"><span data-stu-id="cac0f-146">defaultValue</span></span>|<span data-ttu-id="cac0f-147">String</span><span class="sxs-lookup"><span data-stu-id="cac0f-147">String</span></span>|<span data-ttu-id="cac0f-148">Локализованная строка по умолчанию, отображаемая в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="cac0f-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="cac0f-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="cac0f-149">The default value is empty.</span></span>|
|<span data-ttu-id="cac0f-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="cac0f-150">required</span></span>|<span data-ttu-id="cac0f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="cac0f-151">Boolean</span></span>|<span data-ttu-id="cac0f-152">Требование ввести значение в текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="cac0f-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="cac0f-153">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="cac0f-153">Default value is false.</span></span>|
|<span data-ttu-id="cac0f-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="cac0f-154">maxLength</span></span>|<span data-ttu-id="cac0f-155">Int64</span><span class="sxs-lookup"><span data-stu-id="cac0f-155">Int64</span></span>|<span data-ttu-id="cac0f-156">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="cac0f-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="cac0f-157">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="cac0f-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="cac0f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac0f-158">Response</span></span>
<span data-ttu-id="cac0f-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cac0f-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac0f-160">Пример</span><span class="sxs-lookup"><span data-stu-id="cac0f-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac0f-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="cac0f-161">Request</span></span>
<span data-ttu-id="cac0f-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cac0f-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="cac0f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac0f-163">Response</span></span>
<span data-ttu-id="cac0f-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cac0f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```



