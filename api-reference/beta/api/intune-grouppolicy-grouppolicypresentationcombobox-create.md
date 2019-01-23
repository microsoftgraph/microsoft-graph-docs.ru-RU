---
title: Создание groupPolicyPresentationComboBox
description: Создание нового объекта groupPolicyPresentationComboBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 328550ed5c07259672ae4debee9a8b28681a4b8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431686"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="b57a2-103">Создание groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="b57a2-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="b57a2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b57a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b57a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b57a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b57a2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b57a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57a2-107">Создание нового объекта [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="b57a2-107">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b57a2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="b57a2-108">Prerequisites</span></span>
<span data-ttu-id="b57a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b57a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b57a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b57a2-111">Permission type</span></span>|<span data-ttu-id="b57a2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b57a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b57a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b57a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b57a2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b57a2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b57a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b57a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b57a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b57a2-116">Not supported.</span></span>|
|<span data-ttu-id="b57a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b57a2-117">Application</span></span>|<span data-ttu-id="b57a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b57a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b57a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b57a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="b57a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b57a2-120">Request headers</span></span>
|<span data-ttu-id="b57a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b57a2-121">Header</span></span>|<span data-ttu-id="b57a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b57a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b57a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b57a2-123">Authorization</span></span>|<span data-ttu-id="b57a2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b57a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b57a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b57a2-125">Accept</span></span>|<span data-ttu-id="b57a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b57a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b57a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b57a2-127">Request body</span></span>
<span data-ttu-id="b57a2-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="b57a2-128">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="b57a2-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationComboBox.</span><span class="sxs-lookup"><span data-stu-id="b57a2-129">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="b57a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b57a2-130">Property</span></span>|<span data-ttu-id="b57a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b57a2-131">Type</span></span>|<span data-ttu-id="b57a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b57a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b57a2-133">label</span><span class="sxs-lookup"><span data-stu-id="b57a2-133">label</span></span>|<span data-ttu-id="b57a2-134">String</span><span class="sxs-lookup"><span data-stu-id="b57a2-134">String</span></span>|<span data-ttu-id="b57a2-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="b57a2-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b57a2-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="b57a2-136">The default value is empty.</span></span> <span data-ttu-id="b57a2-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b57a2-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b57a2-138">id</span><span class="sxs-lookup"><span data-stu-id="b57a2-138">id</span></span>|<span data-ttu-id="b57a2-139">String</span><span class="sxs-lookup"><span data-stu-id="b57a2-139">String</span></span>|<span data-ttu-id="b57a2-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b57a2-140">Key of the entity.</span></span> <span data-ttu-id="b57a2-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b57a2-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b57a2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b57a2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b57a2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b57a2-143">DateTimeOffset</span></span>|<span data-ttu-id="b57a2-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b57a2-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b57a2-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b57a2-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b57a2-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b57a2-146">defaultValue</span></span>|<span data-ttu-id="b57a2-147">String</span><span class="sxs-lookup"><span data-stu-id="b57a2-147">String</span></span>|<span data-ttu-id="b57a2-148">Локализованные строки по умолчанию, отображаемые в поле со списком.</span><span class="sxs-lookup"><span data-stu-id="b57a2-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="b57a2-149">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="b57a2-149">The default value is empty.</span></span>|
|<span data-ttu-id="b57a2-150">предложения</span><span class="sxs-lookup"><span data-stu-id="b57a2-150">suggestions</span></span>|<span data-ttu-id="b57a2-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b57a2-151">String collection</span></span>|<span data-ttu-id="b57a2-152">Локализованные строки, указанные в раскрывающемся списке поле со списком.</span><span class="sxs-lookup"><span data-stu-id="b57a2-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="b57a2-153">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="b57a2-153">The default value is empty.</span></span>|
|<span data-ttu-id="b57a2-154">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b57a2-154">required</span></span>|<span data-ttu-id="b57a2-155">Логический</span><span class="sxs-lookup"><span data-stu-id="b57a2-155">Boolean</span></span>|<span data-ttu-id="b57a2-156">Указывает, должно быть указано значение для параметра.</span><span class="sxs-lookup"><span data-stu-id="b57a2-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="b57a2-157">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="b57a2-157">The default value is false.</span></span>|
|<span data-ttu-id="b57a2-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="b57a2-158">maxLength</span></span>|<span data-ttu-id="b57a2-159">Int64</span><span class="sxs-lookup"><span data-stu-id="b57a2-159">Int64</span></span>|<span data-ttu-id="b57a2-160">Целое число без знака, задающее максимальное число знаков для параметра.</span><span class="sxs-lookup"><span data-stu-id="b57a2-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="b57a2-161">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="b57a2-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="b57a2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="b57a2-162">Response</span></span>
<span data-ttu-id="b57a2-163">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b57a2-163">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b57a2-164">Пример</span><span class="sxs-lookup"><span data-stu-id="b57a2-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b57a2-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b57a2-165">Request</span></span>
<span data-ttu-id="b57a2-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b57a2-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b57a2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b57a2-167">Response</span></span>
<span data-ttu-id="b57a2-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b57a2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




