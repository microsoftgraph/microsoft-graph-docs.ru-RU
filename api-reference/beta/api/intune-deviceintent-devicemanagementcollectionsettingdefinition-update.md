---
title: Обновление Девицеманажементколлектионсеттингдефинитион
description: Обновление свойств объекта Девицеманажементколлектионсеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d40a1f4a32b5ec57e96e6c5920ce1c4c64259231
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313435"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="19cd4-103">Обновление Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="19cd4-103">Update deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="19cd4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19cd4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19cd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19cd4-106">Обновление свойств объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="19cd4-106">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19cd4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19cd4-107">Prerequisites</span></span>
<span data-ttu-id="19cd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19cd4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19cd4-110">Permission type</span></span>|<span data-ttu-id="19cd4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19cd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19cd4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19cd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19cd4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19cd4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19cd4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19cd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19cd4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cd4-115">Not supported.</span></span>|
|<span data-ttu-id="19cd4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19cd4-116">Application</span></span>|<span data-ttu-id="19cd4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19cd4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19cd4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19cd4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="19cd4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19cd4-119">Request headers</span></span>
|<span data-ttu-id="19cd4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19cd4-120">Header</span></span>|<span data-ttu-id="19cd4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19cd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19cd4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19cd4-122">Authorization</span></span>|<span data-ttu-id="19cd4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19cd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19cd4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19cd4-124">Accept</span></span>|<span data-ttu-id="19cd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19cd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19cd4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19cd4-126">Request body</span></span>
<span data-ttu-id="19cd4-127">В тексте запроса добавьте представление объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19cd4-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="19cd4-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="19cd4-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="19cd4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="19cd4-129">Property</span></span>|<span data-ttu-id="19cd4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="19cd4-130">Type</span></span>|<span data-ttu-id="19cd4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="19cd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19cd4-132">id</span><span class="sxs-lookup"><span data-stu-id="19cd4-132">id</span></span>|<span data-ttu-id="19cd4-133">String</span><span class="sxs-lookup"><span data-stu-id="19cd4-133">String</span></span>|<span data-ttu-id="19cd4-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-135">Типом</span><span class="sxs-lookup"><span data-stu-id="19cd4-135">valueType</span></span>|[<span data-ttu-id="19cd4-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="19cd4-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="19cd4-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="19cd4-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="19cd4-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="19cd4-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="19cd4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="19cd4-139">displayName</span></span>|<span data-ttu-id="19cd4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="19cd4-140">String</span></span>|<span data-ttu-id="19cd4-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="19cd4-142">isTopLevel</span></span>|<span data-ttu-id="19cd4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="19cd4-143">Boolean</span></span>|<span data-ttu-id="19cd4-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-145">description</span><span class="sxs-lookup"><span data-stu-id="19cd4-145">description</span></span>|<span data-ttu-id="19cd4-146">String</span><span class="sxs-lookup"><span data-stu-id="19cd4-146">String</span></span>|<span data-ttu-id="19cd4-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-148">документатионурл</span><span class="sxs-lookup"><span data-stu-id="19cd4-148">documentationUrl</span></span>|<span data-ttu-id="19cd4-149">String</span><span class="sxs-lookup"><span data-stu-id="19cd4-149">String</span></span>|<span data-ttu-id="19cd4-150">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-151">keywords</span><span class="sxs-lookup"><span data-stu-id="19cd4-151">keywords</span></span>|<span data-ttu-id="19cd4-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="19cd4-152">String collection</span></span>|<span data-ttu-id="19cd4-153">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-154">провероч</span><span class="sxs-lookup"><span data-stu-id="19cd4-154">constraints</span></span>|<span data-ttu-id="19cd4-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="19cd4-156">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="19cd4-157">dependencies</span></span>|<span data-ttu-id="19cd4-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="19cd4-159">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="19cd4-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="19cd4-160">елементдефинитионид</span><span class="sxs-lookup"><span data-stu-id="19cd4-160">elementDefinitionId</span></span>|<span data-ttu-id="19cd4-161">String</span><span class="sxs-lookup"><span data-stu-id="19cd4-161">String</span></span>|<span data-ttu-id="19cd4-162">Идентификатор определения параметра, описывающий, как выглядит каждый элемент коллекции</span><span class="sxs-lookup"><span data-stu-id="19cd4-162">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="19cd4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="19cd4-163">Response</span></span>
<span data-ttu-id="19cd4-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19cd4-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19cd4-165">Пример</span><span class="sxs-lookup"><span data-stu-id="19cd4-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="19cd4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="19cd4-166">Request</span></span>
<span data-ttu-id="19cd4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19cd4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="19cd4-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="19cd4-168">Response</span></span>
<span data-ttu-id="19cd4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19cd4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  "elementDefinitionId": "Element Definition Id value"
}
```






