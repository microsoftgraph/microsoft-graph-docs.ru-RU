---
title: Создание Девицеманажементабстракткомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f3d726b4da7d7c226dbcacdfa80c06b4bb26ea2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974529"
---
# <a name="create-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="a2b71-103">Создание Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="a2b71-103">Create deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="a2b71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2b71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2b71-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2b71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2b71-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2b71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2b71-107">Создание нового объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a2b71-107">Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b71-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2b71-108">Prerequisites</span></span>
<span data-ttu-id="a2b71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2b71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2b71-111">Permission type</span></span>|<span data-ttu-id="a2b71-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2b71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b71-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2b71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2b71-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2b71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2b71-116">Not supported.</span></span>|
|<span data-ttu-id="a2b71-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2b71-117">Application</span></span>|<span data-ttu-id="a2b71-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b71-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b71-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2b71-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a2b71-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2b71-120">Request headers</span></span>
|<span data-ttu-id="a2b71-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2b71-121">Header</span></span>|<span data-ttu-id="a2b71-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2b71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b71-123">Authorization</span></span>|<span data-ttu-id="a2b71-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2b71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2b71-125">Accept</span></span>|<span data-ttu-id="a2b71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b71-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2b71-127">Request body</span></span>
<span data-ttu-id="a2b71-128">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2b71-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingDefinition object.</span></span>

<span data-ttu-id="a2b71-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="a2b71-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingDefinition.</span></span>

|<span data-ttu-id="a2b71-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2b71-130">Property</span></span>|<span data-ttu-id="a2b71-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2b71-131">Type</span></span>|<span data-ttu-id="a2b71-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2b71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b71-133">id</span><span class="sxs-lookup"><span data-stu-id="a2b71-133">id</span></span>|<span data-ttu-id="a2b71-134">String</span><span class="sxs-lookup"><span data-stu-id="a2b71-134">String</span></span>|<span data-ttu-id="a2b71-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-136">Типом</span><span class="sxs-lookup"><span data-stu-id="a2b71-136">valueType</span></span>|[<span data-ttu-id="a2b71-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="a2b71-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="a2b71-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a2b71-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="a2b71-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="a2b71-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="a2b71-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a2b71-140">displayName</span></span>|<span data-ttu-id="a2b71-141">String</span><span class="sxs-lookup"><span data-stu-id="a2b71-141">String</span></span>|<span data-ttu-id="a2b71-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="a2b71-143">isTopLevel</span></span>|<span data-ttu-id="a2b71-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b71-144">Boolean</span></span>|<span data-ttu-id="a2b71-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-146">description</span><span class="sxs-lookup"><span data-stu-id="a2b71-146">description</span></span>|<span data-ttu-id="a2b71-147">String</span><span class="sxs-lookup"><span data-stu-id="a2b71-147">String</span></span>|<span data-ttu-id="a2b71-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="a2b71-149">placeholderText</span></span>|<span data-ttu-id="a2b71-150">String</span><span class="sxs-lookup"><span data-stu-id="a2b71-150">String</span></span>|<span data-ttu-id="a2b71-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="a2b71-152">documentationUrl</span></span>|<span data-ttu-id="a2b71-153">String</span><span class="sxs-lookup"><span data-stu-id="a2b71-153">String</span></span>|<span data-ttu-id="a2b71-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-155">keywords</span><span class="sxs-lookup"><span data-stu-id="a2b71-155">keywords</span></span>|<span data-ttu-id="a2b71-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2b71-156">String collection</span></span>|<span data-ttu-id="a2b71-157">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-158">провероч</span><span class="sxs-lookup"><span data-stu-id="a2b71-158">constraints</span></span>|<span data-ttu-id="a2b71-159">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="a2b71-160">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-161">зависящ</span><span class="sxs-lookup"><span data-stu-id="a2b71-161">dependencies</span></span>|<span data-ttu-id="a2b71-162">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="a2b71-163">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2b71-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="a2b71-164">реализации</span><span class="sxs-lookup"><span data-stu-id="a2b71-164">implementations</span></span>|<span data-ttu-id="a2b71-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2b71-165">String collection</span></span>|<span data-ttu-id="a2b71-166">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="a2b71-166">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="a2b71-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2b71-167">Response</span></span>
<span data-ttu-id="a2b71-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2b71-168">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b71-169">Пример</span><span class="sxs-lookup"><span data-stu-id="a2b71-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b71-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2b71-170">Request</span></span>
<span data-ttu-id="a2b71-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2b71-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2b71-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2b71-172">Response</span></span>
<span data-ttu-id="a2b71-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2b71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






