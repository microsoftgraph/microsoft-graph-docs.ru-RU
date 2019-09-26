---
title: Обновление Граупполиципресентатионмултитекстбокс
description: Обновление свойств объекта Граупполиципресентатионмултитекстбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4897cb6ea5a127580b99d8ce4ab1f22e4d3e58ae
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194049"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="ef200-103">Обновление Граупполиципресентатионмултитекстбокс</span><span class="sxs-lookup"><span data-stu-id="ef200-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="ef200-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef200-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef200-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef200-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef200-106">Обновление свойств объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="ef200-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef200-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef200-107">Prerequisites</span></span>
<span data-ttu-id="ef200-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef200-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef200-110">Permission type</span></span>|<span data-ttu-id="ef200-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef200-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef200-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef200-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef200-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef200-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef200-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef200-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef200-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef200-115">Not supported.</span></span>|
|<span data-ttu-id="ef200-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef200-116">Application</span></span>|<span data-ttu-id="ef200-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef200-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef200-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef200-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef200-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef200-119">Request headers</span></span>
|<span data-ttu-id="ef200-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef200-120">Header</span></span>|<span data-ttu-id="ef200-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef200-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef200-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef200-122">Authorization</span></span>|<span data-ttu-id="ef200-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef200-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef200-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef200-124">Accept</span></span>|<span data-ttu-id="ef200-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef200-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef200-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef200-126">Request body</span></span>
<span data-ttu-id="ef200-127">В тексте запроса добавьте представление объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef200-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="ef200-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="ef200-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="ef200-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef200-129">Property</span></span>|<span data-ttu-id="ef200-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ef200-130">Type</span></span>|<span data-ttu-id="ef200-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ef200-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef200-132">label</span><span class="sxs-lookup"><span data-stu-id="ef200-132">label</span></span>|<span data-ttu-id="ef200-133">String.</span><span class="sxs-lookup"><span data-stu-id="ef200-133">String</span></span>|<span data-ttu-id="ef200-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ef200-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ef200-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="ef200-135">The default value is empty.</span></span> <span data-ttu-id="ef200-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ef200-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ef200-137">id</span><span class="sxs-lookup"><span data-stu-id="ef200-137">id</span></span>|<span data-ttu-id="ef200-138">String</span><span class="sxs-lookup"><span data-stu-id="ef200-138">String</span></span>|<span data-ttu-id="ef200-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef200-139">Key of the entity.</span></span> <span data-ttu-id="ef200-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ef200-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ef200-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef200-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ef200-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef200-142">DateTimeOffset</span></span>|<span data-ttu-id="ef200-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ef200-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ef200-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ef200-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ef200-145">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ef200-145">required</span></span>|<span data-ttu-id="ef200-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ef200-146">Boolean</span></span>|<span data-ttu-id="ef200-147">Требование ввести значение в текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="ef200-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="ef200-148">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="ef200-148">Default value is false.</span></span>|
|<span data-ttu-id="ef200-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="ef200-149">maxLength</span></span>|<span data-ttu-id="ef200-150">Int64</span><span class="sxs-lookup"><span data-stu-id="ef200-150">Int64</span></span>|<span data-ttu-id="ef200-151">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="ef200-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="ef200-152">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="ef200-152">Default value is 1023.</span></span>|
|<span data-ttu-id="ef200-153">максстрингс</span><span class="sxs-lookup"><span data-stu-id="ef200-153">maxStrings</span></span>|<span data-ttu-id="ef200-154">Int64</span><span class="sxs-lookup"><span data-stu-id="ef200-154">Int64</span></span>|<span data-ttu-id="ef200-155">Целое число без знака, задающее максимальное количество строк.</span><span class="sxs-lookup"><span data-stu-id="ef200-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="ef200-156">Значение по умолчанию: 0.</span><span class="sxs-lookup"><span data-stu-id="ef200-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="ef200-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef200-157">Response</span></span>
<span data-ttu-id="ef200-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef200-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef200-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ef200-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef200-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef200-160">Request</span></span>
<span data-ttu-id="ef200-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef200-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="ef200-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef200-162">Response</span></span>
<span data-ttu-id="ef200-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef200-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




