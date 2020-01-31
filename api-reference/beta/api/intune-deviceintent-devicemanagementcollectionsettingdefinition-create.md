---
title: Создание Девицеманажементколлектионсеттингдефинитион
description: Создание нового объекта Девицеманажементколлектионсеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 021d32e24c1ba8614ede4dc3708c9da3cbd9ba82
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636457"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="299e1-103">Создание Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="299e1-103">Create deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="299e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="299e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="299e1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="299e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="299e1-106">Создание нового объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="299e1-106">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="299e1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="299e1-107">Prerequisites</span></span>
<span data-ttu-id="299e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="299e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="299e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="299e1-110">Permission type</span></span>|<span data-ttu-id="299e1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="299e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="299e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="299e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="299e1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299e1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="299e1-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="299e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="299e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="299e1-115">Not supported.</span></span>|
|<span data-ttu-id="299e1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="299e1-116">Application</span></span>|<span data-ttu-id="299e1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299e1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="299e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="299e1-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="299e1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="299e1-119">Request headers</span></span>
|<span data-ttu-id="299e1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="299e1-120">Header</span></span>|<span data-ttu-id="299e1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="299e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="299e1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="299e1-122">Authorization</span></span>|<span data-ttu-id="299e1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="299e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="299e1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="299e1-124">Accept</span></span>|<span data-ttu-id="299e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="299e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="299e1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="299e1-126">Request body</span></span>
<span data-ttu-id="299e1-127">В тексте запроса добавьте представление объекта Девицеманажементколлектионсеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="299e1-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="299e1-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементколлектионсеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="299e1-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="299e1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="299e1-129">Property</span></span>|<span data-ttu-id="299e1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="299e1-130">Type</span></span>|<span data-ttu-id="299e1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="299e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="299e1-132">id</span><span class="sxs-lookup"><span data-stu-id="299e1-132">id</span></span>|<span data-ttu-id="299e1-133">String</span><span class="sxs-lookup"><span data-stu-id="299e1-133">String</span></span>|<span data-ttu-id="299e1-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-135">Типом</span><span class="sxs-lookup"><span data-stu-id="299e1-135">valueType</span></span>|[<span data-ttu-id="299e1-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="299e1-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="299e1-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="299e1-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="299e1-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="299e1-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="299e1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="299e1-139">displayName</span></span>|<span data-ttu-id="299e1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="299e1-140">String</span></span>|<span data-ttu-id="299e1-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="299e1-142">isTopLevel</span></span>|<span data-ttu-id="299e1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="299e1-143">Boolean</span></span>|<span data-ttu-id="299e1-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-145">description</span><span class="sxs-lookup"><span data-stu-id="299e1-145">description</span></span>|<span data-ttu-id="299e1-146">String</span><span class="sxs-lookup"><span data-stu-id="299e1-146">String</span></span>|<span data-ttu-id="299e1-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-148">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="299e1-148">placeholderText</span></span>|<span data-ttu-id="299e1-149">Строка</span><span class="sxs-lookup"><span data-stu-id="299e1-149">String</span></span>|<span data-ttu-id="299e1-150">Замещающий текст в качестве примера допустимых входных данных, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-151">документатионурл</span><span class="sxs-lookup"><span data-stu-id="299e1-151">documentationUrl</span></span>|<span data-ttu-id="299e1-152">Строка</span><span class="sxs-lookup"><span data-stu-id="299e1-152">String</span></span>|<span data-ttu-id="299e1-153">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-154">keywords</span><span class="sxs-lookup"><span data-stu-id="299e1-154">keywords</span></span>|<span data-ttu-id="299e1-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="299e1-155">String collection</span></span>|<span data-ttu-id="299e1-156">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-157">провероч</span><span class="sxs-lookup"><span data-stu-id="299e1-157">constraints</span></span>|<span data-ttu-id="299e1-158">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="299e1-159">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-160">зависящ</span><span class="sxs-lookup"><span data-stu-id="299e1-160">dependencies</span></span>|<span data-ttu-id="299e1-161">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="299e1-162">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="299e1-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="299e1-163">елементдефинитионид</span><span class="sxs-lookup"><span data-stu-id="299e1-163">elementDefinitionId</span></span>|<span data-ttu-id="299e1-164">Строка</span><span class="sxs-lookup"><span data-stu-id="299e1-164">String</span></span>|<span data-ttu-id="299e1-165">Идентификатор определения параметра, описывающий, как выглядит каждый элемент коллекции</span><span class="sxs-lookup"><span data-stu-id="299e1-165">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="299e1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="299e1-166">Response</span></span>
<span data-ttu-id="299e1-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="299e1-167">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="299e1-168">Пример</span><span class="sxs-lookup"><span data-stu-id="299e1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="299e1-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="299e1-169">Request</span></span>
<span data-ttu-id="299e1-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="299e1-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="299e1-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="299e1-171">Response</span></span>
<span data-ttu-id="299e1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="299e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





