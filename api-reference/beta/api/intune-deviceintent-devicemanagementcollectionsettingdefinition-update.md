---
title: Обновление Девицеманажементколлектионсеттингдефинитион
description: Обновление свойств объекта Девицеманажементколлектионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3e13e1c34b87f65f24eb9294082eae17a3f85f8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290163"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="efcf5-103">Обновление Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="efcf5-103">Update deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="efcf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efcf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efcf5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efcf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efcf5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efcf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efcf5-107">Обновление свойств объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="efcf5-107">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efcf5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efcf5-108">Prerequisites</span></span>
<span data-ttu-id="efcf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efcf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efcf5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efcf5-111">Permission type</span></span>|<span data-ttu-id="efcf5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efcf5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efcf5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efcf5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efcf5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcf5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efcf5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efcf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efcf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efcf5-116">Not supported.</span></span>|
|<span data-ttu-id="efcf5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efcf5-117">Application</span></span>|<span data-ttu-id="efcf5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcf5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efcf5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efcf5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="efcf5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efcf5-120">Request headers</span></span>
|<span data-ttu-id="efcf5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efcf5-121">Header</span></span>|<span data-ttu-id="efcf5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="efcf5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efcf5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efcf5-123">Authorization</span></span>|<span data-ttu-id="efcf5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efcf5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efcf5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efcf5-125">Accept</span></span>|<span data-ttu-id="efcf5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efcf5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efcf5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efcf5-127">Request body</span></span>
<span data-ttu-id="efcf5-128">В тексте запроса добавьте представление объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efcf5-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="efcf5-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="efcf5-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="efcf5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="efcf5-130">Property</span></span>|<span data-ttu-id="efcf5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="efcf5-131">Type</span></span>|<span data-ttu-id="efcf5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="efcf5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efcf5-133">id</span><span class="sxs-lookup"><span data-stu-id="efcf5-133">id</span></span>|<span data-ttu-id="efcf5-134">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-134">String</span></span>|<span data-ttu-id="efcf5-135">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-136">Типом</span><span class="sxs-lookup"><span data-stu-id="efcf5-136">valueType</span></span>|[<span data-ttu-id="efcf5-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="efcf5-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="efcf5-138">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="efcf5-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="efcf5-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="efcf5-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="efcf5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="efcf5-140">displayName</span></span>|<span data-ttu-id="efcf5-141">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-141">String</span></span>|<span data-ttu-id="efcf5-142">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="efcf5-143">isTopLevel</span></span>|<span data-ttu-id="efcf5-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="efcf5-144">Boolean</span></span>|<span data-ttu-id="efcf5-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-146">description</span><span class="sxs-lookup"><span data-stu-id="efcf5-146">description</span></span>|<span data-ttu-id="efcf5-147">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-147">String</span></span>|<span data-ttu-id="efcf5-148">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="efcf5-149">placeholderText</span></span>|<span data-ttu-id="efcf5-150">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-150">String</span></span>|<span data-ttu-id="efcf5-151">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="efcf5-152">documentationUrl</span></span>|<span data-ttu-id="efcf5-153">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-153">String</span></span>|<span data-ttu-id="efcf5-154">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="efcf5-155">headerTitle</span></span>|<span data-ttu-id="efcf5-156">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-156">String</span></span>|<span data-ttu-id="efcf5-157">название заголовка параметра представляет категорию или раздел параметров/параметров, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="efcf5-158">headerSubtitle</span></span>|<span data-ttu-id="efcf5-159">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-159">String</span></span>|<span data-ttu-id="efcf5-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе, унаследованных из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-161">keywords</span><span class="sxs-lookup"><span data-stu-id="efcf5-161">keywords</span></span>|<span data-ttu-id="efcf5-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="efcf5-162">String collection</span></span>|<span data-ttu-id="efcf5-163">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-164">провероч</span><span class="sxs-lookup"><span data-stu-id="efcf5-164">constraints</span></span>|<span data-ttu-id="efcf5-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="efcf5-166">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="efcf5-167">dependencies</span></span>|<span data-ttu-id="efcf5-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="efcf5-169">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="efcf5-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="efcf5-170">елементдефинитионид</span><span class="sxs-lookup"><span data-stu-id="efcf5-170">elementDefinitionId</span></span>|<span data-ttu-id="efcf5-171">String</span><span class="sxs-lookup"><span data-stu-id="efcf5-171">String</span></span>|<span data-ttu-id="efcf5-172">Идентификатор определения параметра, описывающий, как выглядит каждый элемент коллекции</span><span class="sxs-lookup"><span data-stu-id="efcf5-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="efcf5-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="efcf5-173">Response</span></span>
<span data-ttu-id="efcf5-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efcf5-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efcf5-175">Пример</span><span class="sxs-lookup"><span data-stu-id="efcf5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="efcf5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="efcf5-176">Request</span></span>
<span data-ttu-id="efcf5-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efcf5-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="efcf5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="efcf5-178">Response</span></span>
<span data-ttu-id="efcf5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efcf5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




