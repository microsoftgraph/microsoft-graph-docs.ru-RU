---
title: Обновление Девицеманажементкомплекссеттингдефинитион
description: Обновление свойств объекта Девицеманажементкомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74214ce9da11f9c9846f35ce687a94f1a5c44284
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695602"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="feb08-103">Обновление Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="feb08-103">Update deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="feb08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="feb08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feb08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feb08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="feb08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb08-107">Обновление свойств объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="feb08-107">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feb08-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="feb08-108">Prerequisites</span></span>
<span data-ttu-id="feb08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feb08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feb08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="feb08-111">Permission type</span></span>|<span data-ttu-id="feb08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="feb08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feb08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="feb08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="feb08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="feb08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feb08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feb08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feb08-116">Not supported.</span></span>|
|<span data-ttu-id="feb08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="feb08-117">Application</span></span>|<span data-ttu-id="feb08-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb08-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="feb08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="feb08-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="feb08-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="feb08-120">Request headers</span></span>
|<span data-ttu-id="feb08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="feb08-121">Header</span></span>|<span data-ttu-id="feb08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="feb08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feb08-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="feb08-123">Authorization</span></span>|<span data-ttu-id="feb08-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="feb08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feb08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="feb08-125">Accept</span></span>|<span data-ttu-id="feb08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="feb08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feb08-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="feb08-127">Request body</span></span>
<span data-ttu-id="feb08-128">В тексте запроса добавьте представление объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feb08-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="feb08-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="feb08-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="feb08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="feb08-130">Property</span></span>|<span data-ttu-id="feb08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="feb08-131">Type</span></span>|<span data-ttu-id="feb08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="feb08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb08-133">id</span><span class="sxs-lookup"><span data-stu-id="feb08-133">id</span></span>|<span data-ttu-id="feb08-134">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-134">String</span></span>|<span data-ttu-id="feb08-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-136">Типом</span><span class="sxs-lookup"><span data-stu-id="feb08-136">valueType</span></span>|[<span data-ttu-id="feb08-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="feb08-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="feb08-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="feb08-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="feb08-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="feb08-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="feb08-140">displayName</span><span class="sxs-lookup"><span data-stu-id="feb08-140">displayName</span></span>|<span data-ttu-id="feb08-141">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-141">String</span></span>|<span data-ttu-id="feb08-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="feb08-143">isTopLevel</span></span>|<span data-ttu-id="feb08-144">Логический</span><span class="sxs-lookup"><span data-stu-id="feb08-144">Boolean</span></span>|<span data-ttu-id="feb08-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-146">description</span><span class="sxs-lookup"><span data-stu-id="feb08-146">description</span></span>|<span data-ttu-id="feb08-147">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-147">String</span></span>|<span data-ttu-id="feb08-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="feb08-149">placeholderText</span></span>|<span data-ttu-id="feb08-150">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-150">String</span></span>|<span data-ttu-id="feb08-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="feb08-152">documentationUrl</span></span>|<span data-ttu-id="feb08-153">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-153">String</span></span>|<span data-ttu-id="feb08-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="feb08-155">headerTitle</span></span>|<span data-ttu-id="feb08-156">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-156">String</span></span>|<span data-ttu-id="feb08-157">название заголовка параметра представляет категорию или раздел параметров/параметров, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="feb08-158">headerSubtitle</span></span>|<span data-ttu-id="feb08-159">Строка</span><span class="sxs-lookup"><span data-stu-id="feb08-159">String</span></span>|<span data-ttu-id="feb08-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-161">keywords</span><span class="sxs-lookup"><span data-stu-id="feb08-161">keywords</span></span>|<span data-ttu-id="feb08-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="feb08-162">String collection</span></span>|<span data-ttu-id="feb08-163">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-164">провероч</span><span class="sxs-lookup"><span data-stu-id="feb08-164">constraints</span></span>|<span data-ttu-id="feb08-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="feb08-166">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="feb08-167">dependencies</span></span>|<span data-ttu-id="feb08-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="feb08-169">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="feb08-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="feb08-170">пропертидефинитионидс</span><span class="sxs-lookup"><span data-stu-id="feb08-170">propertyDefinitionIds</span></span>|<span data-ttu-id="feb08-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="feb08-171">String collection</span></span>|<span data-ttu-id="feb08-172">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="feb08-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="feb08-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="feb08-173">Response</span></span>
<span data-ttu-id="feb08-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="feb08-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feb08-175">Пример</span><span class="sxs-lookup"><span data-stu-id="feb08-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="feb08-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="feb08-176">Request</span></span>
<span data-ttu-id="feb08-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="feb08-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1094

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
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
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="feb08-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="feb08-178">Response</span></span>
<span data-ttu-id="feb08-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="feb08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1143

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
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
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```





