---
title: Создание Девицеманажементабстракткомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbf2117c1d170b1548258b6178ca669b50869138
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731595"
---
# <a name="create-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="5f12f-103">Создание Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="5f12f-103">Create deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="5f12f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f12f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f12f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f12f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f12f-106">Создание нового объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="5f12f-106">Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f12f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f12f-107">Prerequisites</span></span>
<span data-ttu-id="5f12f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f12f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f12f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f12f-110">Permission type</span></span>|<span data-ttu-id="5f12f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f12f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f12f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f12f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f12f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f12f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f12f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f12f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f12f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f12f-115">Not supported.</span></span>|
|<span data-ttu-id="5f12f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5f12f-116">Application</span></span>|<span data-ttu-id="5f12f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f12f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f12f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f12f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5f12f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f12f-119">Request headers</span></span>
|<span data-ttu-id="5f12f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f12f-120">Header</span></span>|<span data-ttu-id="5f12f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5f12f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f12f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f12f-122">Authorization</span></span>|<span data-ttu-id="5f12f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f12f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f12f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f12f-124">Accept</span></span>|<span data-ttu-id="5f12f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f12f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f12f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f12f-126">Request body</span></span>
<span data-ttu-id="5f12f-127">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f12f-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingDefinition object.</span></span>

<span data-ttu-id="5f12f-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="5f12f-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingDefinition.</span></span>

|<span data-ttu-id="5f12f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f12f-129">Property</span></span>|<span data-ttu-id="5f12f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5f12f-130">Type</span></span>|<span data-ttu-id="5f12f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5f12f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f12f-132">id</span><span class="sxs-lookup"><span data-stu-id="5f12f-132">id</span></span>|<span data-ttu-id="5f12f-133">String</span><span class="sxs-lookup"><span data-stu-id="5f12f-133">String</span></span>|<span data-ttu-id="5f12f-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-135">Типом</span><span class="sxs-lookup"><span data-stu-id="5f12f-135">valueType</span></span>|[<span data-ttu-id="5f12f-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="5f12f-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="5f12f-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5f12f-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="5f12f-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="5f12f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5f12f-139">displayName</span></span>|<span data-ttu-id="5f12f-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5f12f-140">String</span></span>|<span data-ttu-id="5f12f-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="5f12f-142">isTopLevel</span></span>|<span data-ttu-id="5f12f-143">Логический</span><span class="sxs-lookup"><span data-stu-id="5f12f-143">Boolean</span></span>|<span data-ttu-id="5f12f-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-145">description</span><span class="sxs-lookup"><span data-stu-id="5f12f-145">description</span></span>|<span data-ttu-id="5f12f-146">String</span><span class="sxs-lookup"><span data-stu-id="5f12f-146">String</span></span>|<span data-ttu-id="5f12f-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-148">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="5f12f-148">placeholderText</span></span>|<span data-ttu-id="5f12f-149">String</span><span class="sxs-lookup"><span data-stu-id="5f12f-149">String</span></span>|<span data-ttu-id="5f12f-150">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-151">документатионурл</span><span class="sxs-lookup"><span data-stu-id="5f12f-151">documentationUrl</span></span>|<span data-ttu-id="5f12f-152">String</span><span class="sxs-lookup"><span data-stu-id="5f12f-152">String</span></span>|<span data-ttu-id="5f12f-153">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-154">keywords</span><span class="sxs-lookup"><span data-stu-id="5f12f-154">keywords</span></span>|<span data-ttu-id="5f12f-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5f12f-155">String collection</span></span>|<span data-ttu-id="5f12f-156">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-157">провероч</span><span class="sxs-lookup"><span data-stu-id="5f12f-157">constraints</span></span>|<span data-ttu-id="5f12f-158">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="5f12f-159">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-160">зависящ</span><span class="sxs-lookup"><span data-stu-id="5f12f-160">dependencies</span></span>|<span data-ttu-id="5f12f-161">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="5f12f-162">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5f12f-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5f12f-163">реализации</span><span class="sxs-lookup"><span data-stu-id="5f12f-163">implementations</span></span>|<span data-ttu-id="5f12f-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5f12f-164">String collection</span></span>|<span data-ttu-id="5f12f-165">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="5f12f-165">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="5f12f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f12f-166">Response</span></span>
<span data-ttu-id="5f12f-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f12f-167">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f12f-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5f12f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f12f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f12f-169">Request</span></span>
<span data-ttu-id="5f12f-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f12f-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5f12f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f12f-171">Response</span></span>
<span data-ttu-id="5f12f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f12f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1051

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




