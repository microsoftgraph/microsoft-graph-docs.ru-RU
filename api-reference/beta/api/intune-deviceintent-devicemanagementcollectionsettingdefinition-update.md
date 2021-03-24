---
title: Обновление deviceManagementCollectionSettingDefinition
description: Обновление свойств объекта deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bfd9fc6e84ba6c11d6941e87a7acac9237c3562
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132130"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="e10c6-103">Обновление deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e10c6-103">Update deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="e10c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e10c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e10c6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e10c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e10c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10c6-107">Обновление свойств объекта [deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-107">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e10c6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e10c6-108">Prerequisites</span></span>
<span data-ttu-id="e10c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e10c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e10c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e10c6-111">Permission type</span></span>|<span data-ttu-id="e10c6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e10c6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e10c6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e10c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e10c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e10c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e10c6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e10c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e10c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10c6-116">Not supported.</span></span>|
|<span data-ttu-id="e10c6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e10c6-117">Application</span></span>|<span data-ttu-id="e10c6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e10c6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e10c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e10c6-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e10c6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e10c6-120">Request headers</span></span>
|<span data-ttu-id="e10c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e10c6-121">Header</span></span>|<span data-ttu-id="e10c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e10c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e10c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e10c6-123">Authorization</span></span>|<span data-ttu-id="e10c6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e10c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e10c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e10c6-125">Accept</span></span>|<span data-ttu-id="e10c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e10c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e10c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e10c6-127">Request body</span></span>
<span data-ttu-id="e10c6-128">В теле запроса поставляем представление JSON для [объекта deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="e10c6-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="e10c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e10c6-130">Property</span></span>|<span data-ttu-id="e10c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e10c6-131">Type</span></span>|<span data-ttu-id="e10c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e10c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10c6-133">id</span><span class="sxs-lookup"><span data-stu-id="e10c6-133">id</span></span>|<span data-ttu-id="e10c6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-134">String</span></span>|<span data-ttu-id="e10c6-135">ID определения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-136">valueType</span><span class="sxs-lookup"><span data-stu-id="e10c6-136">valueType</span></span>|[<span data-ttu-id="e10c6-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="e10c6-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="e10c6-138">Тип данных значения, унаследованный от [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="e10c6-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="e10c6-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="e10c6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e10c6-140">displayName</span></span>|<span data-ttu-id="e10c6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-141">String</span></span>|<span data-ttu-id="e10c6-142">Имя отображения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="e10c6-143">isTopLevel</span></span>|<span data-ttu-id="e10c6-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e10c6-144">Boolean</span></span>|<span data-ttu-id="e10c6-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-146">description</span><span class="sxs-lookup"><span data-stu-id="e10c6-146">description</span></span>|<span data-ttu-id="e10c6-147">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-147">String</span></span>|<span data-ttu-id="e10c6-148">Описание параметра Унаследовано от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="e10c6-149">placeholderText</span></span>|<span data-ttu-id="e10c6-150">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-150">String</span></span>|<span data-ttu-id="e10c6-151">Текст placeholder в качестве примера допустимого ввода, наследуемого [из deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="e10c6-152">documentationUrl</span></span>|<span data-ttu-id="e10c6-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-153">String</span></span>|<span data-ttu-id="e10c6-154">URL-адрес для настройки документации, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="e10c6-155">headerTitle</span></span>|<span data-ttu-id="e10c6-156">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-156">String</span></span>|<span data-ttu-id="e10c6-157">заголовок параметра представляет категорию/раздел параметра/параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="e10c6-158">headerSubtitle</span></span>|<span data-ttu-id="e10c6-159">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-159">String</span></span>|<span data-ttu-id="e10c6-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-161">keywords</span><span class="sxs-lookup"><span data-stu-id="e10c6-161">keywords</span></span>|<span data-ttu-id="e10c6-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e10c6-162">String collection</span></span>|<span data-ttu-id="e10c6-163">Ключевые слова, связанные с параметром Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="e10c6-164">constraints</span></span>|<span data-ttu-id="e10c6-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e10c6-166">Коллекция ограничений для значения параметра Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="e10c6-167">dependencies</span></span>|<span data-ttu-id="e10c6-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="e10c6-169">Коллекция зависимостей от других параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e10c6-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e10c6-170">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e10c6-170">elementDefinitionId</span></span>|<span data-ttu-id="e10c6-171">Строка</span><span class="sxs-lookup"><span data-stu-id="e10c6-171">String</span></span>|<span data-ttu-id="e10c6-172">The Setting Definition ID that describes what each element of the collection looks like</span><span class="sxs-lookup"><span data-stu-id="e10c6-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="e10c6-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="e10c6-173">Response</span></span>
<span data-ttu-id="e10c6-174">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e10c6-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e10c6-175">Пример</span><span class="sxs-lookup"><span data-stu-id="e10c6-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e10c6-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="e10c6-176">Request</span></span>
<span data-ttu-id="e10c6-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e10c6-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1081

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="e10c6-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e10c6-178">Response</span></span>
<span data-ttu-id="e10c6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e10c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  "elementDefinitionId": "Element Definition Id value"
}
```




