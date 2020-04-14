---
title: Обновление Девицеманажементкомплекссеттингдефинитион
description: Обновление свойств объекта Девицеманажементкомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a8bfc2181bb2e6f7585e48c412a789b118fe95f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428213"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="52bd7-103">Обновление Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="52bd7-103">Update deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="52bd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52bd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52bd7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52bd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52bd7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52bd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52bd7-107">Обновление свойств объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="52bd7-107">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52bd7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52bd7-108">Prerequisites</span></span>
<span data-ttu-id="52bd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52bd7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52bd7-111">Permission type</span></span>|<span data-ttu-id="52bd7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52bd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52bd7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52bd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52bd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52bd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52bd7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52bd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52bd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52bd7-116">Not supported.</span></span>|
|<span data-ttu-id="52bd7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="52bd7-117">Application</span></span>|<span data-ttu-id="52bd7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52bd7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52bd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52bd7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="52bd7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52bd7-120">Request headers</span></span>
|<span data-ttu-id="52bd7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52bd7-121">Header</span></span>|<span data-ttu-id="52bd7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52bd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52bd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52bd7-123">Authorization</span></span>|<span data-ttu-id="52bd7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52bd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52bd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52bd7-125">Accept</span></span>|<span data-ttu-id="52bd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52bd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52bd7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52bd7-127">Request body</span></span>
<span data-ttu-id="52bd7-128">В тексте запроса добавьте представление объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52bd7-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="52bd7-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="52bd7-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="52bd7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52bd7-130">Property</span></span>|<span data-ttu-id="52bd7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52bd7-131">Type</span></span>|<span data-ttu-id="52bd7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52bd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52bd7-133">id</span><span class="sxs-lookup"><span data-stu-id="52bd7-133">id</span></span>|<span data-ttu-id="52bd7-134">String</span><span class="sxs-lookup"><span data-stu-id="52bd7-134">String</span></span>|<span data-ttu-id="52bd7-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-136">Типом</span><span class="sxs-lookup"><span data-stu-id="52bd7-136">valueType</span></span>|[<span data-ttu-id="52bd7-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="52bd7-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="52bd7-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="52bd7-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="52bd7-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="52bd7-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="52bd7-140">displayName</span><span class="sxs-lookup"><span data-stu-id="52bd7-140">displayName</span></span>|<span data-ttu-id="52bd7-141">Строка</span><span class="sxs-lookup"><span data-stu-id="52bd7-141">String</span></span>|<span data-ttu-id="52bd7-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="52bd7-143">isTopLevel</span></span>|<span data-ttu-id="52bd7-144">Логическое</span><span class="sxs-lookup"><span data-stu-id="52bd7-144">Boolean</span></span>|<span data-ttu-id="52bd7-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-146">description</span><span class="sxs-lookup"><span data-stu-id="52bd7-146">description</span></span>|<span data-ttu-id="52bd7-147">String</span><span class="sxs-lookup"><span data-stu-id="52bd7-147">String</span></span>|<span data-ttu-id="52bd7-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="52bd7-149">placeholderText</span></span>|<span data-ttu-id="52bd7-150">String</span><span class="sxs-lookup"><span data-stu-id="52bd7-150">String</span></span>|<span data-ttu-id="52bd7-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="52bd7-152">documentationUrl</span></span>|<span data-ttu-id="52bd7-153">String</span><span class="sxs-lookup"><span data-stu-id="52bd7-153">String</span></span>|<span data-ttu-id="52bd7-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-155">keywords</span><span class="sxs-lookup"><span data-stu-id="52bd7-155">keywords</span></span>|<span data-ttu-id="52bd7-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="52bd7-156">String collection</span></span>|<span data-ttu-id="52bd7-157">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-158">провероч</span><span class="sxs-lookup"><span data-stu-id="52bd7-158">constraints</span></span>|<span data-ttu-id="52bd7-159">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="52bd7-160">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-161">зависящ</span><span class="sxs-lookup"><span data-stu-id="52bd7-161">dependencies</span></span>|<span data-ttu-id="52bd7-162">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="52bd7-163">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52bd7-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="52bd7-164">пропертидефинитионидс</span><span class="sxs-lookup"><span data-stu-id="52bd7-164">propertyDefinitionIds</span></span>|<span data-ttu-id="52bd7-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="52bd7-165">String collection</span></span>|<span data-ttu-id="52bd7-166">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="52bd7-166">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="52bd7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="52bd7-167">Response</span></span>
<span data-ttu-id="52bd7-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52bd7-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52bd7-169">Пример</span><span class="sxs-lookup"><span data-stu-id="52bd7-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="52bd7-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="52bd7-170">Request</span></span>
<span data-ttu-id="52bd7-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52bd7-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="52bd7-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="52bd7-172">Response</span></span>
<span data-ttu-id="52bd7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52bd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



