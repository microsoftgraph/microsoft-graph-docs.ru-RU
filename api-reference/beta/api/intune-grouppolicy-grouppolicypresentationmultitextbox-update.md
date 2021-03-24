---
title: Update groupPolicyPresentationMultiTextBox
description: Обновление свойств объекта groupPolicyPresentationMultiTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 719dd7dd2c47b3e47cc3295e9f4ac8d801931cc0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149508"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="b8192-103">Update groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="b8192-103">Update groupPolicyPresentationMultiTextBox</span></span>

<span data-ttu-id="b8192-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8192-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8192-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8192-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8192-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8192-107">Обновление свойств объекта [groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-107">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8192-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8192-108">Prerequisites</span></span>
<span data-ttu-id="b8192-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8192-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8192-111">Permission type</span></span>|<span data-ttu-id="b8192-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8192-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8192-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8192-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8192-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8192-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8192-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8192-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8192-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8192-116">Not supported.</span></span>|
|<span data-ttu-id="b8192-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8192-117">Application</span></span>|<span data-ttu-id="b8192-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8192-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8192-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8192-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b8192-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8192-120">Request headers</span></span>
|<span data-ttu-id="b8192-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8192-121">Header</span></span>|<span data-ttu-id="b8192-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8192-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8192-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8192-123">Authorization</span></span>|<span data-ttu-id="b8192-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8192-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8192-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8192-125">Accept</span></span>|<span data-ttu-id="b8192-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8192-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8192-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8192-127">Request body</span></span>
<span data-ttu-id="b8192-128">В тексте запроса поставляем представление JSON для [объекта groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-128">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="b8192-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-129">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="b8192-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8192-130">Property</span></span>|<span data-ttu-id="b8192-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b8192-131">Type</span></span>|<span data-ttu-id="b8192-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b8192-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8192-133">label</span><span class="sxs-lookup"><span data-stu-id="b8192-133">label</span></span>|<span data-ttu-id="b8192-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b8192-134">String</span></span>|<span data-ttu-id="b8192-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="b8192-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b8192-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="b8192-136">The default value is empty.</span></span> <span data-ttu-id="b8192-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b8192-138">id</span><span class="sxs-lookup"><span data-stu-id="b8192-138">id</span></span>|<span data-ttu-id="b8192-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b8192-139">String</span></span>|<span data-ttu-id="b8192-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b8192-140">Key of the entity.</span></span> <span data-ttu-id="b8192-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b8192-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8192-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b8192-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8192-143">DateTimeOffset</span></span>|<span data-ttu-id="b8192-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b8192-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b8192-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b8192-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b8192-146">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b8192-146">required</span></span>|<span data-ttu-id="b8192-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8192-147">Boolean</span></span>|<span data-ttu-id="b8192-148">Требование ввести значение в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="b8192-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="b8192-149">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="b8192-149">Default value is false.</span></span>|
|<span data-ttu-id="b8192-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="b8192-150">maxLength</span></span>|<span data-ttu-id="b8192-151">Int64</span><span class="sxs-lookup"><span data-stu-id="b8192-151">Int64</span></span>|<span data-ttu-id="b8192-152">Неподписаный целый ряд, который указывает максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="b8192-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="b8192-153">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="b8192-153">Default value is 1023.</span></span>|
|<span data-ttu-id="b8192-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="b8192-154">maxStrings</span></span>|<span data-ttu-id="b8192-155">Int64</span><span class="sxs-lookup"><span data-stu-id="b8192-155">Int64</span></span>|<span data-ttu-id="b8192-156">Неподписаный целый ряд, который указывает максимальное количество строк.</span><span class="sxs-lookup"><span data-stu-id="b8192-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="b8192-157">Значение по умолчанию: 0.</span><span class="sxs-lookup"><span data-stu-id="b8192-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="b8192-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8192-158">Response</span></span>
<span data-ttu-id="b8192-159">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8192-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8192-160">Пример</span><span class="sxs-lookup"><span data-stu-id="b8192-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8192-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8192-161">Request</span></span>
<span data-ttu-id="b8192-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8192-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8192-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8192-163">Response</span></span>
<span data-ttu-id="b8192-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8192-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




