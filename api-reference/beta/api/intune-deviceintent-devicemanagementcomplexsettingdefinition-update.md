---
title: Обновление deviceManagementComplexSettingDefinition
description: Обновление свойств объекта deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e09bbe4c8372840b35cd27229750f781282f115
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132123"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="78491-103">Обновление deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="78491-103">Update deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="78491-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78491-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78491-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78491-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78491-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78491-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78491-107">Обновление свойств объекта [deviceManagementComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-107">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78491-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78491-108">Prerequisites</span></span>
<span data-ttu-id="78491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78491-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78491-111">Permission type</span></span>|<span data-ttu-id="78491-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78491-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78491-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78491-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78491-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78491-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78491-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78491-116">Not supported.</span></span>|
|<span data-ttu-id="78491-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="78491-117">Application</span></span>|<span data-ttu-id="78491-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78491-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78491-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78491-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="78491-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78491-120">Request headers</span></span>
|<span data-ttu-id="78491-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78491-121">Header</span></span>|<span data-ttu-id="78491-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78491-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78491-123">Authorization</span></span>|<span data-ttu-id="78491-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78491-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78491-125">Accept</span></span>|<span data-ttu-id="78491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78491-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78491-127">Request body</span></span>
<span data-ttu-id="78491-128">В теле запроса поставляем представление JSON для [объекта deviceManagementComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="78491-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="78491-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="78491-130">Property</span></span>|<span data-ttu-id="78491-131">Тип</span><span class="sxs-lookup"><span data-stu-id="78491-131">Type</span></span>|<span data-ttu-id="78491-132">Описание</span><span class="sxs-lookup"><span data-stu-id="78491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78491-133">id</span><span class="sxs-lookup"><span data-stu-id="78491-133">id</span></span>|<span data-ttu-id="78491-134">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-134">String</span></span>|<span data-ttu-id="78491-135">ID определения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-136">valueType</span><span class="sxs-lookup"><span data-stu-id="78491-136">valueType</span></span>|[<span data-ttu-id="78491-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="78491-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="78491-138">Тип данных значения, унаследованный от [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="78491-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="78491-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="78491-140">displayName</span><span class="sxs-lookup"><span data-stu-id="78491-140">displayName</span></span>|<span data-ttu-id="78491-141">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-141">String</span></span>|<span data-ttu-id="78491-142">Имя отображения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="78491-143">isTopLevel</span></span>|<span data-ttu-id="78491-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="78491-144">Boolean</span></span>|<span data-ttu-id="78491-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-146">description</span><span class="sxs-lookup"><span data-stu-id="78491-146">description</span></span>|<span data-ttu-id="78491-147">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-147">String</span></span>|<span data-ttu-id="78491-148">Описание параметра Унаследовано от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="78491-149">placeholderText</span></span>|<span data-ttu-id="78491-150">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-150">String</span></span>|<span data-ttu-id="78491-151">Текст placeholder в качестве примера допустимого ввода, наследуемого [из deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="78491-152">documentationUrl</span></span>|<span data-ttu-id="78491-153">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-153">String</span></span>|<span data-ttu-id="78491-154">URL-адрес для настройки документации, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="78491-155">headerTitle</span></span>|<span data-ttu-id="78491-156">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-156">String</span></span>|<span data-ttu-id="78491-157">заголовок параметра представляет категорию/раздел параметра/параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="78491-158">headerSubtitle</span></span>|<span data-ttu-id="78491-159">Строка</span><span class="sxs-lookup"><span data-stu-id="78491-159">String</span></span>|<span data-ttu-id="78491-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-161">keywords</span><span class="sxs-lookup"><span data-stu-id="78491-161">keywords</span></span>|<span data-ttu-id="78491-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="78491-162">String collection</span></span>|<span data-ttu-id="78491-163">Ключевые слова, связанные с параметром Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="78491-164">constraints</span></span>|<span data-ttu-id="78491-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="78491-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="78491-166">Коллекция ограничений для значения параметра Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="78491-167">dependencies</span></span>|<span data-ttu-id="78491-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="78491-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="78491-169">Коллекция зависимостей от других параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="78491-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="78491-170">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="78491-170">propertyDefinitionIds</span></span>|<span data-ttu-id="78491-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="78491-171">String collection</span></span>|<span data-ttu-id="78491-172">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="78491-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="78491-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="78491-173">Response</span></span>
<span data-ttu-id="78491-174">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="78491-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78491-175">Пример</span><span class="sxs-lookup"><span data-stu-id="78491-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="78491-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="78491-176">Request</span></span>
<span data-ttu-id="78491-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78491-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78491-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="78491-178">Response</span></span>
<span data-ttu-id="78491-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78491-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




