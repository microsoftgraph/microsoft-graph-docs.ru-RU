---
title: Создание Граупполиципресентатионтекстбокс
description: Создание нового объекта Граупполиципресентатионтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f14239e2bdb00f728e2d3df31f803c9f44402dd3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408543"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="e3e06-103">Создание Граупполиципресентатионтекстбокс</span><span class="sxs-lookup"><span data-stu-id="e3e06-103">Create groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="e3e06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3e06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3e06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3e06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3e06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e06-107">Создание нового объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="e3e06-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3e06-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3e06-108">Prerequisites</span></span>
<span data-ttu-id="e3e06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3e06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3e06-111">Permission type</span></span>|<span data-ttu-id="e3e06-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3e06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3e06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e06-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e06-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3e06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e06-116">Not supported.</span></span>|
|<span data-ttu-id="e3e06-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e3e06-117">Application</span></span>|<span data-ttu-id="e3e06-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e06-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3e06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="e3e06-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3e06-120">Request headers</span></span>
|<span data-ttu-id="e3e06-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3e06-121">Header</span></span>|<span data-ttu-id="e3e06-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3e06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e06-123">Authorization</span></span>|<span data-ttu-id="e3e06-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3e06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3e06-125">Accept</span></span>|<span data-ttu-id="e3e06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e06-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3e06-127">Request body</span></span>
<span data-ttu-id="e3e06-128">В тексте запроса добавьте представление объекта Граупполиципресентатионтекстбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3e06-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="e3e06-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионтекстбокс.</span><span class="sxs-lookup"><span data-stu-id="e3e06-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="e3e06-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3e06-130">Property</span></span>|<span data-ttu-id="e3e06-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3e06-131">Type</span></span>|<span data-ttu-id="e3e06-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3e06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e06-133">label</span><span class="sxs-lookup"><span data-stu-id="e3e06-133">label</span></span>|<span data-ttu-id="e3e06-134">String</span><span class="sxs-lookup"><span data-stu-id="e3e06-134">String</span></span>|<span data-ttu-id="e3e06-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="e3e06-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e3e06-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="e3e06-136">The default value is empty.</span></span> <span data-ttu-id="e3e06-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e3e06-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e3e06-138">id</span><span class="sxs-lookup"><span data-stu-id="e3e06-138">id</span></span>|<span data-ttu-id="e3e06-139">String</span><span class="sxs-lookup"><span data-stu-id="e3e06-139">String</span></span>|<span data-ttu-id="e3e06-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3e06-140">Key of the entity.</span></span> <span data-ttu-id="e3e06-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e3e06-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e3e06-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e06-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e3e06-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e06-143">DateTimeOffset</span></span>|<span data-ttu-id="e3e06-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e3e06-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="e3e06-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e3e06-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e3e06-146">Значение</span><span class="sxs-lookup"><span data-stu-id="e3e06-146">defaultValue</span></span>|<span data-ttu-id="e3e06-147">String</span><span class="sxs-lookup"><span data-stu-id="e3e06-147">String</span></span>|<span data-ttu-id="e3e06-148">Локализованная строка по умолчанию, отображаемая в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="e3e06-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="e3e06-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="e3e06-149">The default value is empty.</span></span>|
|<span data-ttu-id="e3e06-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e3e06-150">required</span></span>|<span data-ttu-id="e3e06-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="e3e06-151">Boolean</span></span>|<span data-ttu-id="e3e06-152">Требование ввести значение в текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="e3e06-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="e3e06-153">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="e3e06-153">Default value is false.</span></span>|
|<span data-ttu-id="e3e06-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="e3e06-154">maxLength</span></span>|<span data-ttu-id="e3e06-155">Int64</span><span class="sxs-lookup"><span data-stu-id="e3e06-155">Int64</span></span>|<span data-ttu-id="e3e06-156">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="e3e06-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="e3e06-157">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="e3e06-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="e3e06-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e06-158">Response</span></span>
<span data-ttu-id="e3e06-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3e06-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e06-160">Пример</span><span class="sxs-lookup"><span data-stu-id="e3e06-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3e06-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3e06-161">Request</span></span>
<span data-ttu-id="e3e06-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3e06-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="e3e06-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e06-163">Response</span></span>
<span data-ttu-id="e3e06-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3e06-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



