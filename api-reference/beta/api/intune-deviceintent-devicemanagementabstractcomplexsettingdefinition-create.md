---
title: Создание Девицеманажементабстракткомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be28dc686388fafe6eb139051a88a3f58feac2b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49282638"
---
# <a name="create-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="d62d3-103">Создание Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="d62d3-103">Create deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="d62d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d62d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d62d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d62d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d62d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d62d3-107">Создание нового объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d62d3-107">Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d62d3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d62d3-108">Prerequisites</span></span>
<span data-ttu-id="d62d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d62d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d62d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d62d3-111">Permission type</span></span>|<span data-ttu-id="d62d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d62d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d62d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d62d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d62d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d62d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d62d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d62d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d62d3-116">Not supported.</span></span>|
|<span data-ttu-id="d62d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d62d3-117">Application</span></span>|<span data-ttu-id="d62d3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62d3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d62d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d62d3-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d62d3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d62d3-120">Request headers</span></span>
|<span data-ttu-id="d62d3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d62d3-121">Header</span></span>|<span data-ttu-id="d62d3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d62d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d62d3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d62d3-123">Authorization</span></span>|<span data-ttu-id="d62d3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d62d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d62d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d62d3-125">Accept</span></span>|<span data-ttu-id="d62d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d62d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d62d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d62d3-127">Request body</span></span>
<span data-ttu-id="d62d3-128">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d62d3-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingDefinition object.</span></span>

<span data-ttu-id="d62d3-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="d62d3-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingDefinition.</span></span>

|<span data-ttu-id="d62d3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d62d3-130">Property</span></span>|<span data-ttu-id="d62d3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d62d3-131">Type</span></span>|<span data-ttu-id="d62d3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d62d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d62d3-133">id</span><span class="sxs-lookup"><span data-stu-id="d62d3-133">id</span></span>|<span data-ttu-id="d62d3-134">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-134">String</span></span>|<span data-ttu-id="d62d3-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-136">Типом</span><span class="sxs-lookup"><span data-stu-id="d62d3-136">valueType</span></span>|[<span data-ttu-id="d62d3-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="d62d3-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="d62d3-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d62d3-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="d62d3-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="d62d3-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="d62d3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d62d3-140">displayName</span></span>|<span data-ttu-id="d62d3-141">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-141">String</span></span>|<span data-ttu-id="d62d3-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="d62d3-143">isTopLevel</span></span>|<span data-ttu-id="d62d3-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62d3-144">Boolean</span></span>|<span data-ttu-id="d62d3-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-146">description</span><span class="sxs-lookup"><span data-stu-id="d62d3-146">description</span></span>|<span data-ttu-id="d62d3-147">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-147">String</span></span>|<span data-ttu-id="d62d3-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="d62d3-149">placeholderText</span></span>|<span data-ttu-id="d62d3-150">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-150">String</span></span>|<span data-ttu-id="d62d3-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="d62d3-152">documentationUrl</span></span>|<span data-ttu-id="d62d3-153">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-153">String</span></span>|<span data-ttu-id="d62d3-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="d62d3-155">headerTitle</span></span>|<span data-ttu-id="d62d3-156">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-156">String</span></span>|<span data-ttu-id="d62d3-157">название заголовка параметра представляет категорию или раздел параметров/параметров, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="d62d3-158">headerSubtitle</span></span>|<span data-ttu-id="d62d3-159">String</span><span class="sxs-lookup"><span data-stu-id="d62d3-159">String</span></span>|<span data-ttu-id="d62d3-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-161">keywords</span><span class="sxs-lookup"><span data-stu-id="d62d3-161">keywords</span></span>|<span data-ttu-id="d62d3-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d62d3-162">String collection</span></span>|<span data-ttu-id="d62d3-163">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-164">провероч</span><span class="sxs-lookup"><span data-stu-id="d62d3-164">constraints</span></span>|<span data-ttu-id="d62d3-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="d62d3-166">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="d62d3-167">dependencies</span></span>|<span data-ttu-id="d62d3-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="d62d3-169">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d62d3-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d62d3-170">реализации</span><span class="sxs-lookup"><span data-stu-id="d62d3-170">implementations</span></span>|<span data-ttu-id="d62d3-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d62d3-171">String collection</span></span>|<span data-ttu-id="d62d3-172">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="d62d3-172">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="d62d3-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="d62d3-173">Response</span></span>
<span data-ttu-id="d62d3-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d62d3-174">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d62d3-175">Пример</span><span class="sxs-lookup"><span data-stu-id="d62d3-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d62d3-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="d62d3-176">Request</span></span>
<span data-ttu-id="d62d3-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d62d3-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1088

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d62d3-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="d62d3-178">Response</span></span>
<span data-ttu-id="d62d3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d62d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




