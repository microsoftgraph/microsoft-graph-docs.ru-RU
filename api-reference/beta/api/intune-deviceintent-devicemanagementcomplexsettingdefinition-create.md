---
title: Создание deviceManagementComplexSettingDefinition
description: Создайте новый объект deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa09cd1278162296005feefe44796d3f31d2696d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128986"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="cceda-103">Создание deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="cceda-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="cceda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cceda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cceda-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cceda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cceda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cceda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cceda-107">Создайте новый [объект deviceManagementComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cceda-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cceda-108">Prerequisites</span></span>
<span data-ttu-id="cceda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cceda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cceda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cceda-111">Permission type</span></span>|<span data-ttu-id="cceda-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cceda-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cceda-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cceda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cceda-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cceda-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cceda-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cceda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cceda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cceda-116">Not supported.</span></span>|
|<span data-ttu-id="cceda-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cceda-117">Application</span></span>|<span data-ttu-id="cceda-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cceda-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cceda-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cceda-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cceda-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cceda-120">Request headers</span></span>
|<span data-ttu-id="cceda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cceda-121">Header</span></span>|<span data-ttu-id="cceda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cceda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cceda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cceda-123">Authorization</span></span>|<span data-ttu-id="cceda-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cceda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cceda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cceda-125">Accept</span></span>|<span data-ttu-id="cceda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cceda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cceda-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cceda-127">Request body</span></span>
<span data-ttu-id="cceda-128">В теле запроса поставляем представление JSON для объекта deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="cceda-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="cceda-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="cceda-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="cceda-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cceda-130">Property</span></span>|<span data-ttu-id="cceda-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cceda-131">Type</span></span>|<span data-ttu-id="cceda-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cceda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cceda-133">id</span><span class="sxs-lookup"><span data-stu-id="cceda-133">id</span></span>|<span data-ttu-id="cceda-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-134">String</span></span>|<span data-ttu-id="cceda-135">ID определения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-136">valueType</span><span class="sxs-lookup"><span data-stu-id="cceda-136">valueType</span></span>|[<span data-ttu-id="cceda-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="cceda-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="cceda-138">Тип данных значения, унаследованный от [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="cceda-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="cceda-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="cceda-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cceda-140">displayName</span></span>|<span data-ttu-id="cceda-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-141">String</span></span>|<span data-ttu-id="cceda-142">Имя отображения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="cceda-143">isTopLevel</span></span>|<span data-ttu-id="cceda-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="cceda-144">Boolean</span></span>|<span data-ttu-id="cceda-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-146">description</span><span class="sxs-lookup"><span data-stu-id="cceda-146">description</span></span>|<span data-ttu-id="cceda-147">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-147">String</span></span>|<span data-ttu-id="cceda-148">Описание параметра Унаследовано от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="cceda-149">placeholderText</span></span>|<span data-ttu-id="cceda-150">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-150">String</span></span>|<span data-ttu-id="cceda-151">Текст placeholder в качестве примера допустимого ввода, наследуемого [из deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="cceda-152">documentationUrl</span></span>|<span data-ttu-id="cceda-153">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-153">String</span></span>|<span data-ttu-id="cceda-154">URL-адрес для настройки документации, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="cceda-155">headerTitle</span></span>|<span data-ttu-id="cceda-156">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-156">String</span></span>|<span data-ttu-id="cceda-157">заголовок параметра представляет категорию/раздел параметра/параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="cceda-158">headerSubtitle</span></span>|<span data-ttu-id="cceda-159">Строка</span><span class="sxs-lookup"><span data-stu-id="cceda-159">String</span></span>|<span data-ttu-id="cceda-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-161">keywords</span><span class="sxs-lookup"><span data-stu-id="cceda-161">keywords</span></span>|<span data-ttu-id="cceda-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cceda-162">String collection</span></span>|<span data-ttu-id="cceda-163">Ключевые слова, связанные с параметром Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="cceda-164">constraints</span></span>|<span data-ttu-id="cceda-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="cceda-166">Коллекция ограничений для значения параметра Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="cceda-167">dependencies</span></span>|<span data-ttu-id="cceda-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="cceda-169">Коллекция зависимостей от других параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cceda-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cceda-170">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="cceda-170">propertyDefinitionIds</span></span>|<span data-ttu-id="cceda-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cceda-171">String collection</span></span>|<span data-ttu-id="cceda-172">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="cceda-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="cceda-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="cceda-173">Response</span></span>
<span data-ttu-id="cceda-174">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cceda-174">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cceda-175">Пример</span><span class="sxs-lookup"><span data-stu-id="cceda-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="cceda-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="cceda-176">Request</span></span>
<span data-ttu-id="cceda-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cceda-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cceda-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cceda-178">Response</span></span>
<span data-ttu-id="cceda-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cceda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




