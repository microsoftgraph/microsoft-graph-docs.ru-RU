---
title: Обновление Граупполиципресентатионкомбобокс
description: Обновление свойств объекта Граупполиципресентатионкомбобокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6a19df09a180e28be66ba880ceef964f5a9577e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724758"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="41537-103">Обновление Граупполиципресентатионкомбобокс</span><span class="sxs-lookup"><span data-stu-id="41537-103">Update groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="41537-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41537-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41537-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41537-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41537-107">Обновление свойств объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="41537-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41537-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41537-108">Prerequisites</span></span>
<span data-ttu-id="41537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41537-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41537-111">Permission type</span></span>|<span data-ttu-id="41537-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41537-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41537-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41537-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41537-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41537-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41537-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41537-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41537-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41537-116">Not supported.</span></span>|
|<span data-ttu-id="41537-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41537-117">Application</span></span>|<span data-ttu-id="41537-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41537-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41537-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41537-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="41537-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41537-120">Request headers</span></span>
|<span data-ttu-id="41537-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41537-121">Header</span></span>|<span data-ttu-id="41537-122">Значение</span><span class="sxs-lookup"><span data-stu-id="41537-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41537-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41537-123">Authorization</span></span>|<span data-ttu-id="41537-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41537-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41537-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41537-125">Accept</span></span>|<span data-ttu-id="41537-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41537-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41537-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41537-127">Request body</span></span>
<span data-ttu-id="41537-128">В тексте запроса добавьте представление объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41537-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="41537-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span><span class="sxs-lookup"><span data-stu-id="41537-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="41537-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41537-130">Property</span></span>|<span data-ttu-id="41537-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41537-131">Type</span></span>|<span data-ttu-id="41537-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41537-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41537-133">label</span><span class="sxs-lookup"><span data-stu-id="41537-133">label</span></span>|<span data-ttu-id="41537-134">Строка</span><span class="sxs-lookup"><span data-stu-id="41537-134">String</span></span>|<span data-ttu-id="41537-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="41537-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="41537-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="41537-136">The default value is empty.</span></span> <span data-ttu-id="41537-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="41537-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="41537-138">id</span><span class="sxs-lookup"><span data-stu-id="41537-138">id</span></span>|<span data-ttu-id="41537-139">Строка</span><span class="sxs-lookup"><span data-stu-id="41537-139">String</span></span>|<span data-ttu-id="41537-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41537-140">Key of the entity.</span></span> <span data-ttu-id="41537-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="41537-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="41537-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41537-142">lastModifiedDateTime</span></span>|<span data-ttu-id="41537-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41537-143">DateTimeOffset</span></span>|<span data-ttu-id="41537-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="41537-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="41537-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="41537-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="41537-146">Значение</span><span class="sxs-lookup"><span data-stu-id="41537-146">defaultValue</span></span>|<span data-ttu-id="41537-147">Строка</span><span class="sxs-lookup"><span data-stu-id="41537-147">String</span></span>|<span data-ttu-id="41537-148">Локализованная строка по умолчанию, отображаемая в поле со списком.</span><span class="sxs-lookup"><span data-stu-id="41537-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="41537-149">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="41537-149">The default value is empty.</span></span>|
|<span data-ttu-id="41537-150">мнение</span><span class="sxs-lookup"><span data-stu-id="41537-150">suggestions</span></span>|<span data-ttu-id="41537-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="41537-151">String collection</span></span>|<span data-ttu-id="41537-152">Локализованные строки, перечисленные в раскрывающемся списке поля со списком.</span><span class="sxs-lookup"><span data-stu-id="41537-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="41537-153">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="41537-153">The default value is empty.</span></span>|
|<span data-ttu-id="41537-154">Обязательный</span><span class="sxs-lookup"><span data-stu-id="41537-154">required</span></span>|<span data-ttu-id="41537-155">Логический</span><span class="sxs-lookup"><span data-stu-id="41537-155">Boolean</span></span>|<span data-ttu-id="41537-156">Указывает, следует ли указать значение для параметра.</span><span class="sxs-lookup"><span data-stu-id="41537-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="41537-157">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="41537-157">The default value is false.</span></span>|
|<span data-ttu-id="41537-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="41537-158">maxLength</span></span>|<span data-ttu-id="41537-159">Int64</span><span class="sxs-lookup"><span data-stu-id="41537-159">Int64</span></span>|<span data-ttu-id="41537-160">Целое число без знака, задающее максимальное количество текстовых символов для параметра.</span><span class="sxs-lookup"><span data-stu-id="41537-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="41537-161">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="41537-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="41537-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="41537-162">Response</span></span>
<span data-ttu-id="41537-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41537-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41537-164">Пример</span><span class="sxs-lookup"><span data-stu-id="41537-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="41537-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="41537-165">Request</span></span>
<span data-ttu-id="41537-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41537-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41537-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="41537-167">Response</span></span>
<span data-ttu-id="41537-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41537-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





