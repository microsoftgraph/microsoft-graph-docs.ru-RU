---
title: Создание Граупполиципресентатионмултитекстбокс
description: Создание нового объекта Граупполиципресентатионмултитекстбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdde2677c4852c70f1693e7a16e2b9e3fb048388
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152103"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="ce726-103">Создание Граупполиципресентатионмултитекстбокс</span><span class="sxs-lookup"><span data-stu-id="ce726-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="ce726-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce726-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce726-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce726-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce726-106">Создание нового объекта [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="ce726-106">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce726-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce726-107">Prerequisites</span></span>
<span data-ttu-id="ce726-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce726-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce726-110">Permission type</span></span>|<span data-ttu-id="ce726-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce726-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce726-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce726-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce726-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce726-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ce726-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce726-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce726-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce726-115">Not supported.</span></span>|
|<span data-ttu-id="ce726-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce726-116">Application</span></span>|<span data-ttu-id="ce726-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce726-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce726-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce726-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="ce726-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce726-119">Request headers</span></span>
|<span data-ttu-id="ce726-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce726-120">Header</span></span>|<span data-ttu-id="ce726-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ce726-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce726-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce726-122">Authorization</span></span>|<span data-ttu-id="ce726-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ce726-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce726-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ce726-124">Accept</span></span>|<span data-ttu-id="ce726-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce726-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce726-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce726-126">Request body</span></span>
<span data-ttu-id="ce726-127">В тексте запроса добавьте представление объекта Граупполиципресентатионмултитекстбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce726-127">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="ce726-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионмултитекстбокс.</span><span class="sxs-lookup"><span data-stu-id="ce726-128">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="ce726-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce726-129">Property</span></span>|<span data-ttu-id="ce726-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ce726-130">Type</span></span>|<span data-ttu-id="ce726-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ce726-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce726-132">label</span><span class="sxs-lookup"><span data-stu-id="ce726-132">label</span></span>|<span data-ttu-id="ce726-133">String</span><span class="sxs-lookup"><span data-stu-id="ce726-133">String</span></span>|<span data-ttu-id="ce726-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ce726-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ce726-135">Значение по умолчанию — пустое значение.</span><span class="sxs-lookup"><span data-stu-id="ce726-135">The default value is empty.</span></span> <span data-ttu-id="ce726-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce726-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ce726-137">id</span><span class="sxs-lookup"><span data-stu-id="ce726-137">id</span></span>|<span data-ttu-id="ce726-138">String</span><span class="sxs-lookup"><span data-stu-id="ce726-138">String</span></span>|<span data-ttu-id="ce726-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce726-139">Key of the entity.</span></span> <span data-ttu-id="ce726-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce726-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ce726-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce726-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ce726-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce726-142">DateTimeOffset</span></span>|<span data-ttu-id="ce726-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce726-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ce726-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce726-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ce726-145">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ce726-145">required</span></span>|<span data-ttu-id="ce726-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ce726-146">Boolean</span></span>|<span data-ttu-id="ce726-147">Требование ввести значение в текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="ce726-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="ce726-148">Значение по умолчанию — False.</span><span class="sxs-lookup"><span data-stu-id="ce726-148">Default value is false.</span></span>|
|<span data-ttu-id="ce726-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="ce726-149">maxLength</span></span>|<span data-ttu-id="ce726-150">Int64</span><span class="sxs-lookup"><span data-stu-id="ce726-150">Int64</span></span>|<span data-ttu-id="ce726-151">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="ce726-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="ce726-152">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="ce726-152">Default value is 1023.</span></span>|
|<span data-ttu-id="ce726-153">Максстрингс</span><span class="sxs-lookup"><span data-stu-id="ce726-153">maxStrings</span></span>|<span data-ttu-id="ce726-154">Int64</span><span class="sxs-lookup"><span data-stu-id="ce726-154">Int64</span></span>|<span data-ttu-id="ce726-155">Целое число без знака, задающее максимальное количество строк.</span><span class="sxs-lookup"><span data-stu-id="ce726-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="ce726-156">Значение по умолчанию — 0.</span><span class="sxs-lookup"><span data-stu-id="ce726-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="ce726-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce726-157">Response</span></span>
<span data-ttu-id="ce726-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионмултитекстбокс](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce726-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce726-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ce726-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce726-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce726-160">Request</span></span>
<span data-ttu-id="ce726-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce726-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="ce726-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce726-162">Response</span></span>
<span data-ttu-id="ce726-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce726-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




