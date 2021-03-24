---
title: Создание groupPolicyPresentationMultiTextBox
description: Создайте новый объект groupPolicyPresentationMultiTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b633e6b08a06a46be5db297b92a52abe8663422a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149557"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="7e5e1-103">Создание groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="7e5e1-103">Create groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="7e5e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e5e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e5e1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e5e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e5e1-107">Создайте новый [объект groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e5e1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e5e1-108">Prerequisites</span></span>
<span data-ttu-id="7e5e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e5e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e5e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e5e1-111">Permission type</span></span>|<span data-ttu-id="7e5e1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e5e1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e5e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e5e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e5e1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e5e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-116">Not supported.</span></span>|
|<span data-ttu-id="7e5e1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e5e1-117">Application</span></span>|<span data-ttu-id="7e5e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e5e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e5e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e5e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7e5e1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e5e1-120">Request headers</span></span>
|<span data-ttu-id="7e5e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e5e1-121">Header</span></span>|<span data-ttu-id="7e5e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7e5e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e5e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e5e1-123">Authorization</span></span>|<span data-ttu-id="7e5e1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e5e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e5e1-125">Accept</span></span>|<span data-ttu-id="7e5e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e5e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e5e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e5e1-127">Request body</span></span>
<span data-ttu-id="7e5e1-128">В тексте запроса поставляем представление JSON для объекта groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="7e5e1-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="7e5e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e5e1-130">Property</span></span>|<span data-ttu-id="7e5e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7e5e1-131">Type</span></span>|<span data-ttu-id="7e5e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7e5e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5e1-133">label</span><span class="sxs-lookup"><span data-stu-id="7e5e1-133">label</span></span>|<span data-ttu-id="7e5e1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7e5e1-134">String</span></span>|<span data-ttu-id="7e5e1-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7e5e1-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-136">The default value is empty.</span></span> <span data-ttu-id="7e5e1-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e5e1-138">id</span><span class="sxs-lookup"><span data-stu-id="7e5e1-138">id</span></span>|<span data-ttu-id="7e5e1-139">Строка</span><span class="sxs-lookup"><span data-stu-id="7e5e1-139">String</span></span>|<span data-ttu-id="7e5e1-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-140">Key of the entity.</span></span> <span data-ttu-id="7e5e1-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e5e1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e5e1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7e5e1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e5e1-143">DateTimeOffset</span></span>|<span data-ttu-id="7e5e1-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="7e5e1-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e5e1-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e5e1-146">Обязательный</span><span class="sxs-lookup"><span data-stu-id="7e5e1-146">required</span></span>|<span data-ttu-id="7e5e1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e5e1-147">Boolean</span></span>|<span data-ttu-id="7e5e1-148">Требование ввести значение в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="7e5e1-149">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-149">Default value is false.</span></span>|
|<span data-ttu-id="7e5e1-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="7e5e1-150">maxLength</span></span>|<span data-ttu-id="7e5e1-151">Int64</span><span class="sxs-lookup"><span data-stu-id="7e5e1-151">Int64</span></span>|<span data-ttu-id="7e5e1-152">Неподписаный целый ряд, который указывает максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="7e5e1-153">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-153">Default value is 1023.</span></span>|
|<span data-ttu-id="7e5e1-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="7e5e1-154">maxStrings</span></span>|<span data-ttu-id="7e5e1-155">Int64</span><span class="sxs-lookup"><span data-stu-id="7e5e1-155">Int64</span></span>|<span data-ttu-id="7e5e1-156">Неподписаный целый ряд, который указывает максимальное количество строк.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="7e5e1-157">Значение по умолчанию: 0.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="7e5e1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e5e1-158">Response</span></span>
<span data-ttu-id="7e5e1-159">В случае успеха этот метод возвращает код отклика и `201 Created` [объект groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e5e1-160">Пример</span><span class="sxs-lookup"><span data-stu-id="7e5e1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e5e1-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e5e1-161">Request</span></span>
<span data-ttu-id="7e5e1-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e5e1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e5e1-163">Response</span></span>
<span data-ttu-id="7e5e1-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e5e1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




