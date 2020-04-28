---
title: Создание Девицеманажементкомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементкомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a1e3ef31ebb3d2afa3722bf9fa3cb74dbc8482e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428306"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="4208b-103">Создание Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="4208b-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="4208b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4208b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4208b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4208b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4208b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4208b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4208b-107">Создание нового объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="4208b-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4208b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4208b-108">Prerequisites</span></span>
<span data-ttu-id="4208b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4208b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4208b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4208b-111">Permission type</span></span>|<span data-ttu-id="4208b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4208b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4208b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4208b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4208b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4208b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4208b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4208b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4208b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4208b-116">Not supported.</span></span>|
|<span data-ttu-id="4208b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4208b-117">Application</span></span>|<span data-ttu-id="4208b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4208b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4208b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4208b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4208b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4208b-120">Request headers</span></span>
|<span data-ttu-id="4208b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4208b-121">Header</span></span>|<span data-ttu-id="4208b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4208b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4208b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4208b-123">Authorization</span></span>|<span data-ttu-id="4208b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4208b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4208b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4208b-125">Accept</span></span>|<span data-ttu-id="4208b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4208b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4208b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4208b-127">Request body</span></span>
<span data-ttu-id="4208b-128">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4208b-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="4208b-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="4208b-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="4208b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4208b-130">Property</span></span>|<span data-ttu-id="4208b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4208b-131">Type</span></span>|<span data-ttu-id="4208b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4208b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4208b-133">id</span><span class="sxs-lookup"><span data-stu-id="4208b-133">id</span></span>|<span data-ttu-id="4208b-134">String</span><span class="sxs-lookup"><span data-stu-id="4208b-134">String</span></span>|<span data-ttu-id="4208b-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-136">Типом</span><span class="sxs-lookup"><span data-stu-id="4208b-136">valueType</span></span>|[<span data-ttu-id="4208b-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="4208b-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="4208b-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4208b-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="4208b-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="4208b-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="4208b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4208b-140">displayName</span></span>|<span data-ttu-id="4208b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4208b-141">String</span></span>|<span data-ttu-id="4208b-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="4208b-143">isTopLevel</span></span>|<span data-ttu-id="4208b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="4208b-144">Boolean</span></span>|<span data-ttu-id="4208b-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-146">description</span><span class="sxs-lookup"><span data-stu-id="4208b-146">description</span></span>|<span data-ttu-id="4208b-147">String</span><span class="sxs-lookup"><span data-stu-id="4208b-147">String</span></span>|<span data-ttu-id="4208b-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="4208b-149">placeholderText</span></span>|<span data-ttu-id="4208b-150">String</span><span class="sxs-lookup"><span data-stu-id="4208b-150">String</span></span>|<span data-ttu-id="4208b-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="4208b-152">documentationUrl</span></span>|<span data-ttu-id="4208b-153">String</span><span class="sxs-lookup"><span data-stu-id="4208b-153">String</span></span>|<span data-ttu-id="4208b-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-155">keywords</span><span class="sxs-lookup"><span data-stu-id="4208b-155">keywords</span></span>|<span data-ttu-id="4208b-156">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4208b-156">String collection</span></span>|<span data-ttu-id="4208b-157">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-158">провероч</span><span class="sxs-lookup"><span data-stu-id="4208b-158">constraints</span></span>|<span data-ttu-id="4208b-159">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="4208b-160">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-161">зависящ</span><span class="sxs-lookup"><span data-stu-id="4208b-161">dependencies</span></span>|<span data-ttu-id="4208b-162">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="4208b-163">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4208b-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4208b-164">пропертидефинитионидс</span><span class="sxs-lookup"><span data-stu-id="4208b-164">propertyDefinitionIds</span></span>|<span data-ttu-id="4208b-165">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4208b-165">String collection</span></span>|<span data-ttu-id="4208b-166">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="4208b-166">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="4208b-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="4208b-167">Response</span></span>
<span data-ttu-id="4208b-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4208b-168">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4208b-169">Пример</span><span class="sxs-lookup"><span data-stu-id="4208b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="4208b-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="4208b-170">Request</span></span>
<span data-ttu-id="4208b-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4208b-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1008

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
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

### <a name="response"></a><span data-ttu-id="4208b-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="4208b-172">Response</span></span>
<span data-ttu-id="4208b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4208b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1057

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
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



