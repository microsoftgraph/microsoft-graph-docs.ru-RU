---
title: Создание Граупполиципресентатионкомбобокс
description: Создание нового объекта Граупполиципресентатионкомбобокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb7bf38ae0b44149bbc85f7850a118af3c601ca3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943041"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="8a98d-103">Создание Граупполиципресентатионкомбобокс</span><span class="sxs-lookup"><span data-stu-id="8a98d-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="8a98d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a98d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a98d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a98d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a98d-106">Создание нового объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="8a98d-106">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a98d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a98d-107">Prerequisites</span></span>
<span data-ttu-id="8a98d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a98d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a98d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a98d-110">Permission type</span></span>|<span data-ttu-id="8a98d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a98d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a98d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a98d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a98d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a98d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a98d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a98d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a98d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a98d-115">Not supported.</span></span>|
|<span data-ttu-id="8a98d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a98d-116">Application</span></span>|<span data-ttu-id="8a98d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a98d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a98d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a98d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8a98d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a98d-119">Request headers</span></span>
|<span data-ttu-id="8a98d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a98d-120">Header</span></span>|<span data-ttu-id="8a98d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8a98d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a98d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a98d-122">Authorization</span></span>|<span data-ttu-id="8a98d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a98d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a98d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a98d-124">Accept</span></span>|<span data-ttu-id="8a98d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a98d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a98d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a98d-126">Request body</span></span>
<span data-ttu-id="8a98d-127">В тексте запроса добавьте представление объекта Граупполиципресентатионкомбобокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a98d-127">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="8a98d-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионкомбобокс.</span><span class="sxs-lookup"><span data-stu-id="8a98d-128">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="8a98d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a98d-129">Property</span></span>|<span data-ttu-id="8a98d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8a98d-130">Type</span></span>|<span data-ttu-id="8a98d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8a98d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a98d-132">label</span><span class="sxs-lookup"><span data-stu-id="8a98d-132">label</span></span>|<span data-ttu-id="8a98d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8a98d-133">String</span></span>|<span data-ttu-id="8a98d-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="8a98d-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8a98d-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="8a98d-135">The default value is empty.</span></span> <span data-ttu-id="8a98d-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8a98d-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8a98d-137">id</span><span class="sxs-lookup"><span data-stu-id="8a98d-137">id</span></span>|<span data-ttu-id="8a98d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8a98d-138">String</span></span>|<span data-ttu-id="8a98d-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a98d-139">Key of the entity.</span></span> <span data-ttu-id="8a98d-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8a98d-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8a98d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a98d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8a98d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a98d-142">DateTimeOffset</span></span>|<span data-ttu-id="8a98d-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8a98d-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="8a98d-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8a98d-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8a98d-145">Значение</span><span class="sxs-lookup"><span data-stu-id="8a98d-145">defaultValue</span></span>|<span data-ttu-id="8a98d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8a98d-146">String</span></span>|<span data-ttu-id="8a98d-147">Локализованная строка по умолчанию, отображаемая в поле со списком.</span><span class="sxs-lookup"><span data-stu-id="8a98d-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="8a98d-148">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="8a98d-148">The default value is empty.</span></span>|
|<span data-ttu-id="8a98d-149">мнение</span><span class="sxs-lookup"><span data-stu-id="8a98d-149">suggestions</span></span>|<span data-ttu-id="8a98d-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a98d-150">String collection</span></span>|<span data-ttu-id="8a98d-151">Локализованные строки, перечисленные в раскрывающемся списке поля со списком.</span><span class="sxs-lookup"><span data-stu-id="8a98d-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="8a98d-152">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="8a98d-152">The default value is empty.</span></span>|
|<span data-ttu-id="8a98d-153">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8a98d-153">required</span></span>|<span data-ttu-id="8a98d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a98d-154">Boolean</span></span>|<span data-ttu-id="8a98d-155">Указывает, следует ли указать значение для параметра.</span><span class="sxs-lookup"><span data-stu-id="8a98d-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="8a98d-156">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="8a98d-156">The default value is false.</span></span>|
|<span data-ttu-id="8a98d-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="8a98d-157">maxLength</span></span>|<span data-ttu-id="8a98d-158">Int64</span><span class="sxs-lookup"><span data-stu-id="8a98d-158">Int64</span></span>|<span data-ttu-id="8a98d-159">Целое число без знака, задающее максимальное количество текстовых символов для параметра.</span><span class="sxs-lookup"><span data-stu-id="8a98d-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="8a98d-160">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="8a98d-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="8a98d-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a98d-161">Response</span></span>
<span data-ttu-id="8a98d-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a98d-162">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a98d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8a98d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a98d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a98d-164">Request</span></span>
<span data-ttu-id="8a98d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a98d-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="8a98d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a98d-166">Response</span></span>
<span data-ttu-id="8a98d-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a98d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





