---
title: Обновление Девицеманажементабстракткомплекссеттингдефинитион
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b828e4eec983fcbd533ccf187285094905f0793a
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635749"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="0cb54-103">Обновление Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="0cb54-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="0cb54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cb54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cb54-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cb54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb54-106">Обновление свойств объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0cb54-106">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cb54-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0cb54-107">Prerequisites</span></span>
<span data-ttu-id="0cb54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cb54-110">Permission type</span></span>|<span data-ttu-id="0cb54-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cb54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cb54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cb54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cb54-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb54-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cb54-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cb54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cb54-115">Not supported.</span></span>|
|<span data-ttu-id="0cb54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cb54-116">Application</span></span>|<span data-ttu-id="0cb54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb54-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cb54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cb54-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0cb54-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0cb54-119">Request headers</span></span>
|<span data-ttu-id="0cb54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cb54-120">Header</span></span>|<span data-ttu-id="0cb54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0cb54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cb54-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cb54-122">Authorization</span></span>|<span data-ttu-id="0cb54-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cb54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cb54-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0cb54-124">Accept</span></span>|<span data-ttu-id="0cb54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cb54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb54-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cb54-126">Request body</span></span>
<span data-ttu-id="0cb54-127">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cb54-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="0cb54-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0cb54-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="0cb54-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cb54-129">Property</span></span>|<span data-ttu-id="0cb54-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0cb54-130">Type</span></span>|<span data-ttu-id="0cb54-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0cb54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cb54-132">id</span><span class="sxs-lookup"><span data-stu-id="0cb54-132">id</span></span>|<span data-ttu-id="0cb54-133">String</span><span class="sxs-lookup"><span data-stu-id="0cb54-133">String</span></span>|<span data-ttu-id="0cb54-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-135">Типом</span><span class="sxs-lookup"><span data-stu-id="0cb54-135">valueType</span></span>|[<span data-ttu-id="0cb54-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="0cb54-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="0cb54-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0cb54-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="0cb54-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="0cb54-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="0cb54-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0cb54-139">displayName</span></span>|<span data-ttu-id="0cb54-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0cb54-140">String</span></span>|<span data-ttu-id="0cb54-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="0cb54-142">isTopLevel</span></span>|<span data-ttu-id="0cb54-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb54-143">Boolean</span></span>|<span data-ttu-id="0cb54-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-145">description</span><span class="sxs-lookup"><span data-stu-id="0cb54-145">description</span></span>|<span data-ttu-id="0cb54-146">String</span><span class="sxs-lookup"><span data-stu-id="0cb54-146">String</span></span>|<span data-ttu-id="0cb54-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-148">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="0cb54-148">placeholderText</span></span>|<span data-ttu-id="0cb54-149">Строка</span><span class="sxs-lookup"><span data-stu-id="0cb54-149">String</span></span>|<span data-ttu-id="0cb54-150">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-151">документатионурл</span><span class="sxs-lookup"><span data-stu-id="0cb54-151">documentationUrl</span></span>|<span data-ttu-id="0cb54-152">Строка</span><span class="sxs-lookup"><span data-stu-id="0cb54-152">String</span></span>|<span data-ttu-id="0cb54-153">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-154">keywords</span><span class="sxs-lookup"><span data-stu-id="0cb54-154">keywords</span></span>|<span data-ttu-id="0cb54-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0cb54-155">String collection</span></span>|<span data-ttu-id="0cb54-156">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-157">провероч</span><span class="sxs-lookup"><span data-stu-id="0cb54-157">constraints</span></span>|<span data-ttu-id="0cb54-158">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="0cb54-159">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-160">зависящ</span><span class="sxs-lookup"><span data-stu-id="0cb54-160">dependencies</span></span>|<span data-ttu-id="0cb54-161">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="0cb54-162">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cb54-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0cb54-163">реализации</span><span class="sxs-lookup"><span data-stu-id="0cb54-163">implementations</span></span>|<span data-ttu-id="0cb54-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0cb54-164">String collection</span></span>|<span data-ttu-id="0cb54-165">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="0cb54-165">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="0cb54-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cb54-166">Response</span></span>
<span data-ttu-id="0cb54-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cb54-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cb54-168">Пример</span><span class="sxs-lookup"><span data-stu-id="0cb54-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cb54-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cb54-169">Request</span></span>
<span data-ttu-id="0cb54-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cb54-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="0cb54-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cb54-171">Response</span></span>
<span data-ttu-id="0cb54-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cb54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





