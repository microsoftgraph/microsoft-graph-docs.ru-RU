---
title: Обновление Девицеманажементсеттингдефинитион
description: Обновление свойств объекта Девицеманажементсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0185feea03956ee3037e3eacd70d29316757d4b5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300257"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="295ff-103">Обновление Девицеманажементсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="295ff-103">Update deviceManagementSettingDefinition</span></span>

<span data-ttu-id="295ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="295ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="295ff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="295ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="295ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="295ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="295ff-107">Обновление свойств объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="295ff-107">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="295ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="295ff-108">Prerequisites</span></span>
<span data-ttu-id="295ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="295ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="295ff-111">Permission type</span></span>|<span data-ttu-id="295ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="295ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="295ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="295ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="295ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="295ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="295ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="295ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="295ff-116">Not supported.</span></span>|
|<span data-ttu-id="295ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="295ff-117">Application</span></span>|<span data-ttu-id="295ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="295ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="295ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="295ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="295ff-120">Request headers</span></span>
|<span data-ttu-id="295ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="295ff-121">Header</span></span>|<span data-ttu-id="295ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="295ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="295ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="295ff-123">Authorization</span></span>|<span data-ttu-id="295ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="295ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="295ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="295ff-125">Accept</span></span>|<span data-ttu-id="295ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="295ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="295ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="295ff-127">Request body</span></span>
<span data-ttu-id="295ff-128">В тексте запроса добавьте представление объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="295ff-128">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="295ff-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="295ff-129">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="295ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="295ff-130">Property</span></span>|<span data-ttu-id="295ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="295ff-131">Type</span></span>|<span data-ttu-id="295ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="295ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="295ff-133">id</span><span class="sxs-lookup"><span data-stu-id="295ff-133">id</span></span>|<span data-ttu-id="295ff-134">String</span><span class="sxs-lookup"><span data-stu-id="295ff-134">String</span></span>|<span data-ttu-id="295ff-135">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="295ff-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="295ff-136">Типом</span><span class="sxs-lookup"><span data-stu-id="295ff-136">valueType</span></span>|[<span data-ttu-id="295ff-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="295ff-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="295ff-138">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="295ff-138">The data type of the value.</span></span> <span data-ttu-id="295ff-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="295ff-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="295ff-140">displayName</span><span class="sxs-lookup"><span data-stu-id="295ff-140">displayName</span></span>|<span data-ttu-id="295ff-141">String</span><span class="sxs-lookup"><span data-stu-id="295ff-141">String</span></span>|<span data-ttu-id="295ff-142">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="295ff-142">The setting's display name</span></span>|
|<span data-ttu-id="295ff-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="295ff-143">isTopLevel</span></span>|<span data-ttu-id="295ff-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="295ff-144">Boolean</span></span>|<span data-ttu-id="295ff-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.</span><span class="sxs-lookup"><span data-stu-id="295ff-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="295ff-146">description</span><span class="sxs-lookup"><span data-stu-id="295ff-146">description</span></span>|<span data-ttu-id="295ff-147">String</span><span class="sxs-lookup"><span data-stu-id="295ff-147">String</span></span>|<span data-ttu-id="295ff-148">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="295ff-148">The setting's description</span></span>|
|<span data-ttu-id="295ff-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="295ff-149">placeholderText</span></span>|<span data-ttu-id="295ff-150">String</span><span class="sxs-lookup"><span data-stu-id="295ff-150">String</span></span>|<span data-ttu-id="295ff-151">Замещающий текст в качестве примера допустимых входных данных</span><span class="sxs-lookup"><span data-stu-id="295ff-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="295ff-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="295ff-152">documentationUrl</span></span>|<span data-ttu-id="295ff-153">String</span><span class="sxs-lookup"><span data-stu-id="295ff-153">String</span></span>|<span data-ttu-id="295ff-154">URL-адрес для установки документации</span><span class="sxs-lookup"><span data-stu-id="295ff-154">Url to setting documentation</span></span>|
|<span data-ttu-id="295ff-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="295ff-155">headerTitle</span></span>|<span data-ttu-id="295ff-156">String</span><span class="sxs-lookup"><span data-stu-id="295ff-156">String</span></span>|<span data-ttu-id="295ff-157">Заголовок параметра "заголовок" представляет категорию или раздел параметров или параметров</span><span class="sxs-lookup"><span data-stu-id="295ff-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="295ff-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="295ff-158">headerSubtitle</span></span>|<span data-ttu-id="295ff-159">String</span><span class="sxs-lookup"><span data-stu-id="295ff-159">String</span></span>|<span data-ttu-id="295ff-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе</span><span class="sxs-lookup"><span data-stu-id="295ff-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="295ff-161">keywords</span><span class="sxs-lookup"><span data-stu-id="295ff-161">keywords</span></span>|<span data-ttu-id="295ff-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="295ff-162">String collection</span></span>|<span data-ttu-id="295ff-163">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="295ff-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="295ff-164">провероч</span><span class="sxs-lookup"><span data-stu-id="295ff-164">constraints</span></span>|<span data-ttu-id="295ff-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="295ff-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="295ff-166">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="295ff-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="295ff-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="295ff-167">dependencies</span></span>|<span data-ttu-id="295ff-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="295ff-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="295ff-169">Коллекция зависимостей для других параметров</span><span class="sxs-lookup"><span data-stu-id="295ff-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="295ff-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="295ff-170">Response</span></span>
<span data-ttu-id="295ff-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="295ff-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="295ff-172">Пример</span><span class="sxs-lookup"><span data-stu-id="295ff-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="295ff-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="295ff-173">Request</span></span>
<span data-ttu-id="295ff-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="295ff-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1014

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="295ff-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="295ff-175">Response</span></span>
<span data-ttu-id="295ff-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="295ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1063

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ]
}
```




