---
title: Обновление Девицеманажементколлектионсеттингдефинитион
description: Обновление свойств объекта Девицеманажементколлектионсеттингдефинитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4240dd4f9b1d26aff07aebd46fb9a9376c6e98e7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730657"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="d6aa7-103">Обновление Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="d6aa7-103">Update deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="d6aa7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6aa7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6aa7-106">Обновление свойств объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d6aa7-106">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6aa7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6aa7-107">Prerequisites</span></span>
<span data-ttu-id="d6aa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6aa7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6aa7-110">Permission type</span></span>|<span data-ttu-id="d6aa7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6aa7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6aa7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6aa7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6aa7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6aa7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-115">Not supported.</span></span>|
|<span data-ttu-id="d6aa7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6aa7-116">Application</span></span>|<span data-ttu-id="d6aa7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6aa7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6aa7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6aa7-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d6aa7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6aa7-119">Request headers</span></span>
|<span data-ttu-id="d6aa7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6aa7-120">Header</span></span>|<span data-ttu-id="d6aa7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d6aa7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6aa7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6aa7-122">Authorization</span></span>|<span data-ttu-id="d6aa7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6aa7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d6aa7-124">Accept</span></span>|<span data-ttu-id="d6aa7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6aa7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6aa7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6aa7-126">Request body</span></span>
<span data-ttu-id="d6aa7-127">В тексте запроса добавьте представление объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="d6aa7-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d6aa7-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="d6aa7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6aa7-129">Property</span></span>|<span data-ttu-id="d6aa7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d6aa7-130">Type</span></span>|<span data-ttu-id="d6aa7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d6aa7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6aa7-132">id</span><span class="sxs-lookup"><span data-stu-id="d6aa7-132">id</span></span>|<span data-ttu-id="d6aa7-133">String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-133">String</span></span>|<span data-ttu-id="d6aa7-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-135">Типом</span><span class="sxs-lookup"><span data-stu-id="d6aa7-135">valueType</span></span>|[<span data-ttu-id="d6aa7-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="d6aa7-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="d6aa7-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d6aa7-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="d6aa7-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="d6aa7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d6aa7-139">displayName</span></span>|<span data-ttu-id="d6aa7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d6aa7-140">String</span></span>|<span data-ttu-id="d6aa7-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="d6aa7-142">isTopLevel</span></span>|<span data-ttu-id="d6aa7-143">Логический</span><span class="sxs-lookup"><span data-stu-id="d6aa7-143">Boolean</span></span>|<span data-ttu-id="d6aa7-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-145">description</span><span class="sxs-lookup"><span data-stu-id="d6aa7-145">description</span></span>|<span data-ttu-id="d6aa7-146">String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-146">String</span></span>|<span data-ttu-id="d6aa7-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-148">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="d6aa7-148">placeholderText</span></span>|<span data-ttu-id="d6aa7-149">String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-149">String</span></span>|<span data-ttu-id="d6aa7-150">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-151">документатионурл</span><span class="sxs-lookup"><span data-stu-id="d6aa7-151">documentationUrl</span></span>|<span data-ttu-id="d6aa7-152">String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-152">String</span></span>|<span data-ttu-id="d6aa7-153">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-154">keywords</span><span class="sxs-lookup"><span data-stu-id="d6aa7-154">keywords</span></span>|<span data-ttu-id="d6aa7-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-155">String collection</span></span>|<span data-ttu-id="d6aa7-156">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-157">провероч</span><span class="sxs-lookup"><span data-stu-id="d6aa7-157">constraints</span></span>|<span data-ttu-id="d6aa7-158">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="d6aa7-159">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-160">зависящ</span><span class="sxs-lookup"><span data-stu-id="d6aa7-160">dependencies</span></span>|<span data-ttu-id="d6aa7-161">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="d6aa7-162">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d6aa7-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d6aa7-163">елементдефинитионид</span><span class="sxs-lookup"><span data-stu-id="d6aa7-163">elementDefinitionId</span></span>|<span data-ttu-id="d6aa7-164">String</span><span class="sxs-lookup"><span data-stu-id="d6aa7-164">String</span></span>|<span data-ttu-id="d6aa7-165">Идентификатор определения параметра, описывающий, как выглядит каждый элемент коллекции</span><span class="sxs-lookup"><span data-stu-id="d6aa7-165">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="d6aa7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6aa7-166">Response</span></span>
<span data-ttu-id="d6aa7-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6aa7-168">Пример</span><span class="sxs-lookup"><span data-stu-id="d6aa7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6aa7-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6aa7-169">Request</span></span>
<span data-ttu-id="d6aa7-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 995

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="d6aa7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6aa7-171">Response</span></span>
<span data-ttu-id="d6aa7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6aa7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1044

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  "elementDefinitionId": "Element Definition Id value"
}
```




