---
title: Обновление Девицеманажементабстракткомплекссеттингдефинитион
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 838da51da670a2c7e957be5e8922b926f273dbb4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974473"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="4722f-103">Обновление Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="4722f-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="4722f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4722f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4722f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4722f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4722f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4722f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4722f-107">Обновление свойств объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="4722f-107">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4722f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4722f-108">Prerequisites</span></span>
<span data-ttu-id="4722f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4722f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4722f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4722f-111">Permission type</span></span>|<span data-ttu-id="4722f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4722f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4722f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4722f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4722f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4722f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4722f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4722f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4722f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4722f-116">Not supported.</span></span>|
|<span data-ttu-id="4722f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4722f-117">Application</span></span>|<span data-ttu-id="4722f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4722f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4722f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4722f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4722f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4722f-120">Request headers</span></span>
|<span data-ttu-id="4722f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4722f-121">Header</span></span>|<span data-ttu-id="4722f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4722f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4722f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4722f-123">Authorization</span></span>|<span data-ttu-id="4722f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4722f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4722f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4722f-125">Accept</span></span>|<span data-ttu-id="4722f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4722f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4722f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4722f-127">Request body</span></span>
<span data-ttu-id="4722f-128">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4722f-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="4722f-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4722f-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="4722f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4722f-130">Property</span></span>|<span data-ttu-id="4722f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4722f-131">Type</span></span>|<span data-ttu-id="4722f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4722f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4722f-133">id</span><span class="sxs-lookup"><span data-stu-id="4722f-133">id</span></span>|<span data-ttu-id="4722f-134">String</span><span class="sxs-lookup"><span data-stu-id="4722f-134">String</span></span>|<span data-ttu-id="4722f-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-136">Типом</span><span class="sxs-lookup"><span data-stu-id="4722f-136">valueType</span></span>|[<span data-ttu-id="4722f-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="4722f-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="4722f-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4722f-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="4722f-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="4722f-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="4722f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4722f-140">displayName</span></span>|<span data-ttu-id="4722f-141">String</span><span class="sxs-lookup"><span data-stu-id="4722f-141">String</span></span>|<span data-ttu-id="4722f-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="4722f-143">isTopLevel</span></span>|<span data-ttu-id="4722f-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="4722f-144">Boolean</span></span>|<span data-ttu-id="4722f-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-146">description</span><span class="sxs-lookup"><span data-stu-id="4722f-146">description</span></span>|<span data-ttu-id="4722f-147">String</span><span class="sxs-lookup"><span data-stu-id="4722f-147">String</span></span>|<span data-ttu-id="4722f-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="4722f-149">placeholderText</span></span>|<span data-ttu-id="4722f-150">String</span><span class="sxs-lookup"><span data-stu-id="4722f-150">String</span></span>|<span data-ttu-id="4722f-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="4722f-152">documentationUrl</span></span>|<span data-ttu-id="4722f-153">String</span><span class="sxs-lookup"><span data-stu-id="4722f-153">String</span></span>|<span data-ttu-id="4722f-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-155">keywords</span><span class="sxs-lookup"><span data-stu-id="4722f-155">keywords</span></span>|<span data-ttu-id="4722f-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4722f-156">String collection</span></span>|<span data-ttu-id="4722f-157">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-158">провероч</span><span class="sxs-lookup"><span data-stu-id="4722f-158">constraints</span></span>|<span data-ttu-id="4722f-159">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="4722f-160">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-161">зависящ</span><span class="sxs-lookup"><span data-stu-id="4722f-161">dependencies</span></span>|<span data-ttu-id="4722f-162">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="4722f-163">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4722f-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4722f-164">реализации</span><span class="sxs-lookup"><span data-stu-id="4722f-164">implementations</span></span>|<span data-ttu-id="4722f-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4722f-165">String collection</span></span>|<span data-ttu-id="4722f-166">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="4722f-166">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="4722f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4722f-167">Response</span></span>
<span data-ttu-id="4722f-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4722f-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4722f-169">Пример</span><span class="sxs-lookup"><span data-stu-id="4722f-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="4722f-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="4722f-170">Request</span></span>
<span data-ttu-id="4722f-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4722f-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4722f-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="4722f-172">Response</span></span>
<span data-ttu-id="4722f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4722f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






