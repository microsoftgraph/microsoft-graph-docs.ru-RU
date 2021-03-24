---
title: Создание groupPolicyPresentationTextBox
description: Создайте новый объект groupPolicyPresentationTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e5d23f310744c55522e54a74a77d21dc50d405d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149431"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="a2e10-103">Создание groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="a2e10-103">Create groupPolicyPresentationTextBox</span></span>

<span data-ttu-id="a2e10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2e10-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2e10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2e10-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2e10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e10-107">Создайте новый [объект groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)</span><span class="sxs-lookup"><span data-stu-id="a2e10-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2e10-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2e10-108">Prerequisites</span></span>
<span data-ttu-id="a2e10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2e10-111">Permission type</span></span>|<span data-ttu-id="a2e10-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2e10-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e10-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2e10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e10-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2e10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2e10-116">Not supported.</span></span>|
|<span data-ttu-id="a2e10-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2e10-117">Application</span></span>|<span data-ttu-id="a2e10-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e10-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2e10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a2e10-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2e10-120">Request headers</span></span>
|<span data-ttu-id="a2e10-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2e10-121">Header</span></span>|<span data-ttu-id="a2e10-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2e10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2e10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2e10-123">Authorization</span></span>|<span data-ttu-id="a2e10-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2e10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2e10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2e10-125">Accept</span></span>|<span data-ttu-id="a2e10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2e10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e10-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2e10-127">Request body</span></span>
<span data-ttu-id="a2e10-128">В тексте запроса поставляем представление JSON для объекта groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="a2e10-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="a2e10-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="a2e10-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="a2e10-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2e10-130">Property</span></span>|<span data-ttu-id="a2e10-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2e10-131">Type</span></span>|<span data-ttu-id="a2e10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2e10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e10-133">label</span><span class="sxs-lookup"><span data-stu-id="a2e10-133">label</span></span>|<span data-ttu-id="a2e10-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a2e10-134">String</span></span>|<span data-ttu-id="a2e10-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="a2e10-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a2e10-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="a2e10-136">The default value is empty.</span></span> <span data-ttu-id="a2e10-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a2e10-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a2e10-138">id</span><span class="sxs-lookup"><span data-stu-id="a2e10-138">id</span></span>|<span data-ttu-id="a2e10-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a2e10-139">String</span></span>|<span data-ttu-id="a2e10-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2e10-140">Key of the entity.</span></span> <span data-ttu-id="a2e10-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a2e10-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a2e10-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e10-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a2e10-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e10-143">DateTimeOffset</span></span>|<span data-ttu-id="a2e10-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a2e10-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="a2e10-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a2e10-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a2e10-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a2e10-146">defaultValue</span></span>|<span data-ttu-id="a2e10-147">Строка</span><span class="sxs-lookup"><span data-stu-id="a2e10-147">String</span></span>|<span data-ttu-id="a2e10-148">Локализованная строка по умолчанию, отображаемая в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="a2e10-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="a2e10-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="a2e10-149">The default value is empty.</span></span>|
|<span data-ttu-id="a2e10-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a2e10-150">required</span></span>|<span data-ttu-id="a2e10-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2e10-151">Boolean</span></span>|<span data-ttu-id="a2e10-152">Требование ввести значение в текстовом окне.</span><span class="sxs-lookup"><span data-stu-id="a2e10-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="a2e10-153">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="a2e10-153">Default value is false.</span></span>|
|<span data-ttu-id="a2e10-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="a2e10-154">maxLength</span></span>|<span data-ttu-id="a2e10-155">Int64</span><span class="sxs-lookup"><span data-stu-id="a2e10-155">Int64</span></span>|<span data-ttu-id="a2e10-156">Неподписаный целый ряд, который указывает максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="a2e10-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="a2e10-157">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="a2e10-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="a2e10-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2e10-158">Response</span></span>
<span data-ttu-id="a2e10-159">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a2e10-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e10-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a2e10-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2e10-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2e10-161">Request</span></span>
<span data-ttu-id="a2e10-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2e10-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2e10-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2e10-163">Response</span></span>
<span data-ttu-id="a2e10-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2e10-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




