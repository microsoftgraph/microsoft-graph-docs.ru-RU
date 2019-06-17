---
title: Обновление Граупполиципресентатионкомбобокс
description: Обновление свойств объекта Граупполиципресентатионкомбобокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04bc5333e8f8fc67a4551708823421b6127862a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985075"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="f51c1-103">Обновление Граупполиципресентатионкомбобокс</span><span class="sxs-lookup"><span data-stu-id="f51c1-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="f51c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f51c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f51c1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f51c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f51c1-106">Обновление свойств объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="f51c1-106">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f51c1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f51c1-107">Prerequisites</span></span>
<span data-ttu-id="f51c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f51c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f51c1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f51c1-110">Permission type</span></span>|<span data-ttu-id="f51c1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f51c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f51c1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f51c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f51c1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f51c1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f51c1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f51c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f51c1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f51c1-115">Not supported.</span></span>|
|<span data-ttu-id="f51c1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f51c1-116">Application</span></span>|<span data-ttu-id="f51c1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f51c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f51c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f51c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f51c1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f51c1-119">Request headers</span></span>
|<span data-ttu-id="f51c1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f51c1-120">Header</span></span>|<span data-ttu-id="f51c1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f51c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f51c1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f51c1-122">Authorization</span></span>|<span data-ttu-id="f51c1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f51c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f51c1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f51c1-124">Accept</span></span>|<span data-ttu-id="f51c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f51c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f51c1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f51c1-126">Request body</span></span>
<span data-ttu-id="f51c1-127">В тексте запроса добавьте представление объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f51c1-127">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="f51c1-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span><span class="sxs-lookup"><span data-stu-id="f51c1-128">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="f51c1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f51c1-129">Property</span></span>|<span data-ttu-id="f51c1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f51c1-130">Type</span></span>|<span data-ttu-id="f51c1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f51c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f51c1-132">label</span><span class="sxs-lookup"><span data-stu-id="f51c1-132">label</span></span>|<span data-ttu-id="f51c1-133">String</span><span class="sxs-lookup"><span data-stu-id="f51c1-133">String</span></span>|<span data-ttu-id="f51c1-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="f51c1-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f51c1-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="f51c1-135">The default value is empty.</span></span> <span data-ttu-id="f51c1-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f51c1-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f51c1-137">id</span><span class="sxs-lookup"><span data-stu-id="f51c1-137">id</span></span>|<span data-ttu-id="f51c1-138">String</span><span class="sxs-lookup"><span data-stu-id="f51c1-138">String</span></span>|<span data-ttu-id="f51c1-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f51c1-139">Key of the entity.</span></span> <span data-ttu-id="f51c1-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f51c1-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f51c1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f51c1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f51c1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f51c1-142">DateTimeOffset</span></span>|<span data-ttu-id="f51c1-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f51c1-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="f51c1-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f51c1-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f51c1-145">Значение</span><span class="sxs-lookup"><span data-stu-id="f51c1-145">defaultValue</span></span>|<span data-ttu-id="f51c1-146">String</span><span class="sxs-lookup"><span data-stu-id="f51c1-146">String</span></span>|<span data-ttu-id="f51c1-147">Локализованная строка по умолчанию, отображаемая в поле со списком.</span><span class="sxs-lookup"><span data-stu-id="f51c1-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="f51c1-148">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="f51c1-148">The default value is empty.</span></span>|
|<span data-ttu-id="f51c1-149">мнение</span><span class="sxs-lookup"><span data-stu-id="f51c1-149">suggestions</span></span>|<span data-ttu-id="f51c1-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f51c1-150">String collection</span></span>|<span data-ttu-id="f51c1-151">Локализованные строки, перечисленные в раскрывающемся списке поля со списком.</span><span class="sxs-lookup"><span data-stu-id="f51c1-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="f51c1-152">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="f51c1-152">The default value is empty.</span></span>|
|<span data-ttu-id="f51c1-153">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f51c1-153">required</span></span>|<span data-ttu-id="f51c1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="f51c1-154">Boolean</span></span>|<span data-ttu-id="f51c1-155">Указывает, следует ли указать значение для параметра.</span><span class="sxs-lookup"><span data-stu-id="f51c1-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="f51c1-156">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="f51c1-156">The default value is false.</span></span>|
|<span data-ttu-id="f51c1-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="f51c1-157">maxLength</span></span>|<span data-ttu-id="f51c1-158">Int64</span><span class="sxs-lookup"><span data-stu-id="f51c1-158">Int64</span></span>|<span data-ttu-id="f51c1-159">Целое число без знака, задающее максимальное количество текстовых символов для параметра.</span><span class="sxs-lookup"><span data-stu-id="f51c1-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="f51c1-160">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="f51c1-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="f51c1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f51c1-161">Response</span></span>
<span data-ttu-id="f51c1-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f51c1-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f51c1-163">Пример</span><span class="sxs-lookup"><span data-stu-id="f51c1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f51c1-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f51c1-164">Request</span></span>
<span data-ttu-id="f51c1-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f51c1-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f51c1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f51c1-166">Response</span></span>
<span data-ttu-id="f51c1-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f51c1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





