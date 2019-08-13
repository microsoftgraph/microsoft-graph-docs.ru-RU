---
title: Создание Девицеманажементкомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементкомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fdee09a0fd921aae24a3cca15c0ecd47842609fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313456"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="90f00-103">Создание Девицеманажементкомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="90f00-103">Create deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="90f00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90f00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90f00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90f00-106">Создание нового объекта [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="90f00-106">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90f00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90f00-107">Prerequisites</span></span>
<span data-ttu-id="90f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90f00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90f00-110">Permission type</span></span>|<span data-ttu-id="90f00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90f00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90f00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90f00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90f00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90f00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90f00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90f00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90f00-115">Not supported.</span></span>|
|<span data-ttu-id="90f00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90f00-116">Application</span></span>|<span data-ttu-id="90f00-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f00-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90f00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90f00-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="90f00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90f00-119">Request headers</span></span>
|<span data-ttu-id="90f00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90f00-120">Header</span></span>|<span data-ttu-id="90f00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90f00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90f00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90f00-122">Authorization</span></span>|<span data-ttu-id="90f00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90f00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90f00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90f00-124">Accept</span></span>|<span data-ttu-id="90f00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90f00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90f00-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90f00-126">Request body</span></span>
<span data-ttu-id="90f00-127">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90f00-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="90f00-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="90f00-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="90f00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="90f00-129">Property</span></span>|<span data-ttu-id="90f00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="90f00-130">Type</span></span>|<span data-ttu-id="90f00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="90f00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90f00-132">id</span><span class="sxs-lookup"><span data-stu-id="90f00-132">id</span></span>|<span data-ttu-id="90f00-133">String</span><span class="sxs-lookup"><span data-stu-id="90f00-133">String</span></span>|<span data-ttu-id="90f00-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-135">Типом</span><span class="sxs-lookup"><span data-stu-id="90f00-135">valueType</span></span>|[<span data-ttu-id="90f00-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="90f00-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="90f00-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="90f00-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="90f00-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="90f00-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="90f00-139">displayName</span><span class="sxs-lookup"><span data-stu-id="90f00-139">displayName</span></span>|<span data-ttu-id="90f00-140">Строка</span><span class="sxs-lookup"><span data-stu-id="90f00-140">String</span></span>|<span data-ttu-id="90f00-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="90f00-142">isTopLevel</span></span>|<span data-ttu-id="90f00-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="90f00-143">Boolean</span></span>|<span data-ttu-id="90f00-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-145">description</span><span class="sxs-lookup"><span data-stu-id="90f00-145">description</span></span>|<span data-ttu-id="90f00-146">String</span><span class="sxs-lookup"><span data-stu-id="90f00-146">String</span></span>|<span data-ttu-id="90f00-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-148">документатионурл</span><span class="sxs-lookup"><span data-stu-id="90f00-148">documentationUrl</span></span>|<span data-ttu-id="90f00-149">String</span><span class="sxs-lookup"><span data-stu-id="90f00-149">String</span></span>|<span data-ttu-id="90f00-150">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-151">keywords</span><span class="sxs-lookup"><span data-stu-id="90f00-151">keywords</span></span>|<span data-ttu-id="90f00-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="90f00-152">String collection</span></span>|<span data-ttu-id="90f00-153">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-154">провероч</span><span class="sxs-lookup"><span data-stu-id="90f00-154">constraints</span></span>|<span data-ttu-id="90f00-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="90f00-156">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="90f00-157">dependencies</span></span>|<span data-ttu-id="90f00-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="90f00-159">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="90f00-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="90f00-160">пропертидефинитионидс</span><span class="sxs-lookup"><span data-stu-id="90f00-160">propertyDefinitionIds</span></span>|<span data-ttu-id="90f00-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="90f00-161">String collection</span></span>|<span data-ttu-id="90f00-162">Определения каждого свойства сложного параметра</span><span class="sxs-lookup"><span data-stu-id="90f00-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="90f00-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="90f00-163">Response</span></span>
<span data-ttu-id="90f00-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90f00-164">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f00-165">Пример</span><span class="sxs-lookup"><span data-stu-id="90f00-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="90f00-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="90f00-166">Request</span></span>
<span data-ttu-id="90f00-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90f00-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 808

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="90f00-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="90f00-168">Response</span></span>
<span data-ttu-id="90f00-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90f00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```






