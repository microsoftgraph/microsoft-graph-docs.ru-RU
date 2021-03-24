---
title: Создание deviceManagementCollectionSettingDefinition
description: Создайте новый объект deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: daec478a51c2bd69acacc0eec2444166a387d1c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132186"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="70883-103">Создание deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="70883-103">Create deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="70883-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70883-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70883-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70883-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70883-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70883-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70883-107">Создайте новый [объект deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-107">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70883-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70883-108">Prerequisites</span></span>
<span data-ttu-id="70883-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70883-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70883-111">Permission type</span></span>|<span data-ttu-id="70883-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70883-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70883-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70883-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70883-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70883-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70883-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70883-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70883-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70883-116">Not supported.</span></span>|
|<span data-ttu-id="70883-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="70883-117">Application</span></span>|<span data-ttu-id="70883-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70883-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70883-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70883-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="70883-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="70883-120">Request headers</span></span>
|<span data-ttu-id="70883-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70883-121">Header</span></span>|<span data-ttu-id="70883-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70883-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70883-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70883-123">Authorization</span></span>|<span data-ttu-id="70883-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70883-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70883-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70883-125">Accept</span></span>|<span data-ttu-id="70883-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70883-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70883-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70883-127">Request body</span></span>
<span data-ttu-id="70883-128">В теле запроса поставляем представление JSON для объекта deviceManagementCollectionSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="70883-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="70883-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementCollectionSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="70883-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="70883-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="70883-130">Property</span></span>|<span data-ttu-id="70883-131">Тип</span><span class="sxs-lookup"><span data-stu-id="70883-131">Type</span></span>|<span data-ttu-id="70883-132">Описание</span><span class="sxs-lookup"><span data-stu-id="70883-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70883-133">id</span><span class="sxs-lookup"><span data-stu-id="70883-133">id</span></span>|<span data-ttu-id="70883-134">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-134">String</span></span>|<span data-ttu-id="70883-135">ID определения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-136">valueType</span><span class="sxs-lookup"><span data-stu-id="70883-136">valueType</span></span>|[<span data-ttu-id="70883-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="70883-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="70883-138">Тип данных значения, унаследованный от [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="70883-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="70883-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="70883-140">displayName</span><span class="sxs-lookup"><span data-stu-id="70883-140">displayName</span></span>|<span data-ttu-id="70883-141">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-141">String</span></span>|<span data-ttu-id="70883-142">Имя отображения параметра, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="70883-143">isTopLevel</span></span>|<span data-ttu-id="70883-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="70883-144">Boolean</span></span>|<span data-ttu-id="70883-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр, унаследованный от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-146">description</span><span class="sxs-lookup"><span data-stu-id="70883-146">description</span></span>|<span data-ttu-id="70883-147">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-147">String</span></span>|<span data-ttu-id="70883-148">Описание параметра Унаследовано от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="70883-149">placeholderText</span></span>|<span data-ttu-id="70883-150">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-150">String</span></span>|<span data-ttu-id="70883-151">Текст placeholder в качестве примера допустимого ввода, наследуемого [из deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="70883-152">documentationUrl</span></span>|<span data-ttu-id="70883-153">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-153">String</span></span>|<span data-ttu-id="70883-154">URL-адрес для настройки документации, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="70883-155">headerTitle</span></span>|<span data-ttu-id="70883-156">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-156">String</span></span>|<span data-ttu-id="70883-157">заголовок параметра представляет категорию/раздел параметра/параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="70883-158">headerSubtitle</span></span>|<span data-ttu-id="70883-159">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-159">String</span></span>|<span data-ttu-id="70883-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе, унаследованной от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-161">keywords</span><span class="sxs-lookup"><span data-stu-id="70883-161">keywords</span></span>|<span data-ttu-id="70883-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70883-162">String collection</span></span>|<span data-ttu-id="70883-163">Ключевые слова, связанные с параметром Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="70883-164">constraints</span></span>|<span data-ttu-id="70883-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="70883-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="70883-166">Коллекция ограничений для значения параметра Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="70883-167">dependencies</span></span>|<span data-ttu-id="70883-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="70883-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="70883-169">Коллекция зависимостей от других параметров, унаследованных от [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="70883-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="70883-170">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="70883-170">elementDefinitionId</span></span>|<span data-ttu-id="70883-171">Строка</span><span class="sxs-lookup"><span data-stu-id="70883-171">String</span></span>|<span data-ttu-id="70883-172">The Setting Definition ID that describes what each element of the collection looks like</span><span class="sxs-lookup"><span data-stu-id="70883-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="70883-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="70883-173">Response</span></span>
<span data-ttu-id="70883-174">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="70883-174">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70883-175">Пример</span><span class="sxs-lookup"><span data-stu-id="70883-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="70883-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="70883-176">Request</span></span>
<span data-ttu-id="70883-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70883-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="70883-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="70883-178">Response</span></span>
<span data-ttu-id="70883-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70883-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




