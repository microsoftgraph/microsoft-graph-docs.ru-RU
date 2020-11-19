---
title: Создание Девицеманажементкомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементкомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 018c9a5619c61a84c1b76f9467f3af30318ccc0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290086"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="16531-103">Создание Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="16531-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="16531-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16531-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16531-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16531-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16531-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16531-107">Создание нового объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="16531-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16531-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16531-108">Prerequisites</span></span>
<span data-ttu-id="16531-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16531-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16531-111">Permission type</span></span>|<span data-ttu-id="16531-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16531-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16531-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16531-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16531-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16531-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16531-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16531-116">Not supported.</span></span>|
|<span data-ttu-id="16531-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16531-117">Application</span></span>|<span data-ttu-id="16531-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16531-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16531-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/settingDefinitions
POST /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="16531-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16531-120">Request headers</span></span>
|<span data-ttu-id="16531-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16531-121">Header</span></span>|<span data-ttu-id="16531-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16531-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16531-123">Authorization</span></span>|<span data-ttu-id="16531-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16531-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16531-125">Accept</span></span>|<span data-ttu-id="16531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16531-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16531-127">Request body</span></span>
<span data-ttu-id="16531-128">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16531-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="16531-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="16531-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="16531-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16531-130">Property</span></span>|<span data-ttu-id="16531-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16531-131">Type</span></span>|<span data-ttu-id="16531-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16531-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16531-133">id</span><span class="sxs-lookup"><span data-stu-id="16531-133">id</span></span>|<span data-ttu-id="16531-134">String</span><span class="sxs-lookup"><span data-stu-id="16531-134">String</span></span>|<span data-ttu-id="16531-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-136">Типом</span><span class="sxs-lookup"><span data-stu-id="16531-136">valueType</span></span>|[<span data-ttu-id="16531-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="16531-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="16531-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="16531-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="16531-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="16531-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="16531-140">displayName</span><span class="sxs-lookup"><span data-stu-id="16531-140">displayName</span></span>|<span data-ttu-id="16531-141">String</span><span class="sxs-lookup"><span data-stu-id="16531-141">String</span></span>|<span data-ttu-id="16531-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="16531-143">isTopLevel</span></span>|<span data-ttu-id="16531-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="16531-144">Boolean</span></span>|<span data-ttu-id="16531-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-146">description</span><span class="sxs-lookup"><span data-stu-id="16531-146">description</span></span>|<span data-ttu-id="16531-147">String</span><span class="sxs-lookup"><span data-stu-id="16531-147">String</span></span>|<span data-ttu-id="16531-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="16531-149">placeholderText</span></span>|<span data-ttu-id="16531-150">String</span><span class="sxs-lookup"><span data-stu-id="16531-150">String</span></span>|<span data-ttu-id="16531-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="16531-152">documentationUrl</span></span>|<span data-ttu-id="16531-153">String</span><span class="sxs-lookup"><span data-stu-id="16531-153">String</span></span>|<span data-ttu-id="16531-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="16531-155">headerTitle</span></span>|<span data-ttu-id="16531-156">String</span><span class="sxs-lookup"><span data-stu-id="16531-156">String</span></span>|<span data-ttu-id="16531-157">название заголовка параметра представляет категорию или раздел параметров/параметров, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="16531-158">headerSubtitle</span></span>|<span data-ttu-id="16531-159">String</span><span class="sxs-lookup"><span data-stu-id="16531-159">String</span></span>|<span data-ttu-id="16531-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-161">keywords</span><span class="sxs-lookup"><span data-stu-id="16531-161">keywords</span></span>|<span data-ttu-id="16531-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16531-162">String collection</span></span>|<span data-ttu-id="16531-163">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-164">провероч</span><span class="sxs-lookup"><span data-stu-id="16531-164">constraints</span></span>|<span data-ttu-id="16531-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="16531-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="16531-166">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="16531-167">dependencies</span></span>|<span data-ttu-id="16531-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="16531-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="16531-169">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16531-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="16531-170">пропертидефинитионидс</span><span class="sxs-lookup"><span data-stu-id="16531-170">propertyDefinitionIds</span></span>|<span data-ttu-id="16531-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16531-171">String collection</span></span>|<span data-ttu-id="16531-172">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="16531-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="16531-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="16531-173">Response</span></span>
<span data-ttu-id="16531-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16531-174">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16531-175">Пример</span><span class="sxs-lookup"><span data-stu-id="16531-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="16531-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="16531-176">Request</span></span>
<span data-ttu-id="16531-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16531-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="16531-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="16531-178">Response</span></span>
<span data-ttu-id="16531-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16531-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




