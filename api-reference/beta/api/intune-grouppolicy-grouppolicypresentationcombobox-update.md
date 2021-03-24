---
title: Update groupPolicyPresentationComboBox
description: Обновление свойств объекта groupPolicyPresentationComboBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a3fa1ef56577fe13a21367e4844be41870538df
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149704"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="58970-103">Update groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="58970-103">Update groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="58970-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58970-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58970-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58970-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58970-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58970-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58970-107">Обновление свойств объекта [groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)</span><span class="sxs-lookup"><span data-stu-id="58970-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58970-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58970-108">Prerequisites</span></span>
<span data-ttu-id="58970-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58970-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58970-111">Permission type</span></span>|<span data-ttu-id="58970-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58970-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58970-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58970-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58970-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58970-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58970-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58970-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58970-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58970-116">Not supported.</span></span>|
|<span data-ttu-id="58970-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58970-117">Application</span></span>|<span data-ttu-id="58970-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58970-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58970-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58970-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="58970-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58970-120">Request headers</span></span>
|<span data-ttu-id="58970-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58970-121">Header</span></span>|<span data-ttu-id="58970-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58970-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58970-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58970-123">Authorization</span></span>|<span data-ttu-id="58970-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58970-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58970-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58970-125">Accept</span></span>|<span data-ttu-id="58970-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58970-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58970-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58970-127">Request body</span></span>
<span data-ttu-id="58970-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)</span><span class="sxs-lookup"><span data-stu-id="58970-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="58970-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)</span><span class="sxs-lookup"><span data-stu-id="58970-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="58970-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58970-130">Property</span></span>|<span data-ttu-id="58970-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58970-131">Type</span></span>|<span data-ttu-id="58970-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58970-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58970-133">label</span><span class="sxs-lookup"><span data-stu-id="58970-133">label</span></span>|<span data-ttu-id="58970-134">Строка</span><span class="sxs-lookup"><span data-stu-id="58970-134">String</span></span>|<span data-ttu-id="58970-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="58970-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="58970-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="58970-136">The default value is empty.</span></span> <span data-ttu-id="58970-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58970-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58970-138">id</span><span class="sxs-lookup"><span data-stu-id="58970-138">id</span></span>|<span data-ttu-id="58970-139">Строка</span><span class="sxs-lookup"><span data-stu-id="58970-139">String</span></span>|<span data-ttu-id="58970-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58970-140">Key of the entity.</span></span> <span data-ttu-id="58970-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58970-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58970-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58970-142">lastModifiedDateTime</span></span>|<span data-ttu-id="58970-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58970-143">DateTimeOffset</span></span>|<span data-ttu-id="58970-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="58970-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="58970-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58970-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58970-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="58970-146">defaultValue</span></span>|<span data-ttu-id="58970-147">Строка</span><span class="sxs-lookup"><span data-stu-id="58970-147">String</span></span>|<span data-ttu-id="58970-148">Локализованная строка по умолчанию, отображаемая в поле комбо.</span><span class="sxs-lookup"><span data-stu-id="58970-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="58970-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="58970-149">The default value is empty.</span></span>|
|<span data-ttu-id="58970-150">предложения</span><span class="sxs-lookup"><span data-stu-id="58970-150">suggestions</span></span>|<span data-ttu-id="58970-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="58970-151">String collection</span></span>|<span data-ttu-id="58970-152">Локализованные строки, перечисленные в выпадаемом списке комбо-окна.</span><span class="sxs-lookup"><span data-stu-id="58970-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="58970-153">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="58970-153">The default value is empty.</span></span>|
|<span data-ttu-id="58970-154">Обязательный</span><span class="sxs-lookup"><span data-stu-id="58970-154">required</span></span>|<span data-ttu-id="58970-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="58970-155">Boolean</span></span>|<span data-ttu-id="58970-156">Указывает, должно ли значение быть задано для параметра.</span><span class="sxs-lookup"><span data-stu-id="58970-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="58970-157">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="58970-157">The default value is false.</span></span>|
|<span data-ttu-id="58970-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="58970-158">maxLength</span></span>|<span data-ttu-id="58970-159">Int64</span><span class="sxs-lookup"><span data-stu-id="58970-159">Int64</span></span>|<span data-ttu-id="58970-160">Неподписаный целый ряд, который указывает максимальное количество текстовых символов для параметра.</span><span class="sxs-lookup"><span data-stu-id="58970-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="58970-161">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="58970-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="58970-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="58970-162">Response</span></span>
<span data-ttu-id="58970-163">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="58970-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58970-164">Пример</span><span class="sxs-lookup"><span data-stu-id="58970-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="58970-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="58970-165">Request</span></span>
<span data-ttu-id="58970-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58970-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="58970-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="58970-167">Response</span></span>
<span data-ttu-id="58970-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58970-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




