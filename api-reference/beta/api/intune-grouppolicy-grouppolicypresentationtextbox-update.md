---
title: Обновление groupPolicyPresentationTextBox
description: Обновление свойств объекта groupPolicyPresentationTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ff83558c1d66505e0623d4cd9b48ef83f033f37
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157393"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="141b5-103">Обновление groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="141b5-103">Update groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="141b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="141b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="141b5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="141b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="141b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="141b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="141b5-107">Обновление свойств объекта [groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="141b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="141b5-108">Prerequisites</span></span>
<span data-ttu-id="141b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="141b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="141b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="141b5-111">Permission type</span></span>|<span data-ttu-id="141b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="141b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="141b5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="141b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="141b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="141b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="141b5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="141b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="141b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="141b5-116">Not supported.</span></span>|
|<span data-ttu-id="141b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="141b5-117">Application</span></span>|<span data-ttu-id="141b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="141b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="141b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="141b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="141b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="141b5-120">Request headers</span></span>
|<span data-ttu-id="141b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="141b5-121">Header</span></span>|<span data-ttu-id="141b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="141b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="141b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="141b5-123">Authorization</span></span>|<span data-ttu-id="141b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="141b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="141b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="141b5-125">Accept</span></span>|<span data-ttu-id="141b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="141b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="141b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="141b5-127">Request body</span></span>
<span data-ttu-id="141b5-128">В тексте запроса поставляем представление JSON для [объекта groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="141b5-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="141b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="141b5-130">Property</span></span>|<span data-ttu-id="141b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="141b5-131">Type</span></span>|<span data-ttu-id="141b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="141b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="141b5-133">label</span><span class="sxs-lookup"><span data-stu-id="141b5-133">label</span></span>|<span data-ttu-id="141b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="141b5-134">String</span></span>|<span data-ttu-id="141b5-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="141b5-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="141b5-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="141b5-136">The default value is empty.</span></span> <span data-ttu-id="141b5-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="141b5-138">id</span><span class="sxs-lookup"><span data-stu-id="141b5-138">id</span></span>|<span data-ttu-id="141b5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="141b5-139">String</span></span>|<span data-ttu-id="141b5-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="141b5-140">Key of the entity.</span></span> <span data-ttu-id="141b5-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="141b5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="141b5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="141b5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="141b5-143">DateTimeOffset</span></span>|<span data-ttu-id="141b5-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="141b5-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="141b5-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="141b5-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="141b5-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="141b5-146">defaultValue</span></span>|<span data-ttu-id="141b5-147">Строка</span><span class="sxs-lookup"><span data-stu-id="141b5-147">String</span></span>|<span data-ttu-id="141b5-148">Локализованная строка по умолчанию, отображаемая в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="141b5-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="141b5-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="141b5-149">The default value is empty.</span></span>|
|<span data-ttu-id="141b5-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="141b5-150">required</span></span>|<span data-ttu-id="141b5-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="141b5-151">Boolean</span></span>|<span data-ttu-id="141b5-152">Требование ввести значение в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="141b5-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="141b5-153">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="141b5-153">Default value is false.</span></span>|
|<span data-ttu-id="141b5-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="141b5-154">maxLength</span></span>|<span data-ttu-id="141b5-155">Int64</span><span class="sxs-lookup"><span data-stu-id="141b5-155">Int64</span></span>|<span data-ttu-id="141b5-156">Неподписаный целый ряд, который указывает максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="141b5-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="141b5-157">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="141b5-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="141b5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="141b5-158">Response</span></span>
<span data-ttu-id="141b5-159">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="141b5-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="141b5-160">Пример</span><span class="sxs-lookup"><span data-stu-id="141b5-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="141b5-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="141b5-161">Request</span></span>
<span data-ttu-id="141b5-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="141b5-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="141b5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="141b5-163">Response</span></span>
<span data-ttu-id="141b5-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="141b5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




