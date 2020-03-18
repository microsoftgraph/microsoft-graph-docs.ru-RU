---
title: Обновление Девицеманажементсеттингдефинитион
description: Обновление свойств объекта Девицеманажементсеттингдефинитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f1b0540aa1696459c70783b5c31788276e71558
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815074"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="a22d4-103">Обновление Девицеманажементсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="a22d4-103">Update deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="a22d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a22d4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a22d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a22d4-106">Обновление свойств объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a22d4-106">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a22d4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a22d4-107">Prerequisites</span></span>
<span data-ttu-id="a22d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a22d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a22d4-110">Permission type</span></span>|<span data-ttu-id="a22d4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a22d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a22d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a22d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a22d4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a22d4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a22d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a22d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a22d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22d4-115">Not supported.</span></span>|
|<span data-ttu-id="a22d4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a22d4-116">Application</span></span>|<span data-ttu-id="a22d4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a22d4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a22d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a22d4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a22d4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a22d4-119">Request headers</span></span>
|<span data-ttu-id="a22d4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a22d4-120">Header</span></span>|<span data-ttu-id="a22d4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a22d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a22d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a22d4-122">Authorization</span></span>|<span data-ttu-id="a22d4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a22d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a22d4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a22d4-124">Accept</span></span>|<span data-ttu-id="a22d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a22d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a22d4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a22d4-126">Request body</span></span>
<span data-ttu-id="a22d4-127">В тексте запроса добавьте представление объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a22d4-127">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="a22d4-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a22d4-128">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="a22d4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a22d4-129">Property</span></span>|<span data-ttu-id="a22d4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a22d4-130">Type</span></span>|<span data-ttu-id="a22d4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a22d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a22d4-132">id</span><span class="sxs-lookup"><span data-stu-id="a22d4-132">id</span></span>|<span data-ttu-id="a22d4-133">String</span><span class="sxs-lookup"><span data-stu-id="a22d4-133">String</span></span>|<span data-ttu-id="a22d4-134">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="a22d4-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="a22d4-135">Типом</span><span class="sxs-lookup"><span data-stu-id="a22d4-135">valueType</span></span>|[<span data-ttu-id="a22d4-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="a22d4-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="a22d4-137">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="a22d4-137">The data type of the value.</span></span> <span data-ttu-id="a22d4-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="a22d4-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="a22d4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a22d4-139">displayName</span></span>|<span data-ttu-id="a22d4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a22d4-140">String</span></span>|<span data-ttu-id="a22d4-141">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="a22d4-141">The setting's display name</span></span>|
|<span data-ttu-id="a22d4-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="a22d4-142">isTopLevel</span></span>|<span data-ttu-id="a22d4-143">Логический</span><span class="sxs-lookup"><span data-stu-id="a22d4-143">Boolean</span></span>|<span data-ttu-id="a22d4-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.</span><span class="sxs-lookup"><span data-stu-id="a22d4-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="a22d4-145">description</span><span class="sxs-lookup"><span data-stu-id="a22d4-145">description</span></span>|<span data-ttu-id="a22d4-146">String</span><span class="sxs-lookup"><span data-stu-id="a22d4-146">String</span></span>|<span data-ttu-id="a22d4-147">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="a22d4-147">The setting's description</span></span>|
|<span data-ttu-id="a22d4-148">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="a22d4-148">placeholderText</span></span>|<span data-ttu-id="a22d4-149">String</span><span class="sxs-lookup"><span data-stu-id="a22d4-149">String</span></span>|<span data-ttu-id="a22d4-150">Замещающий текст в качестве примера допустимых входных данных</span><span class="sxs-lookup"><span data-stu-id="a22d4-150">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="a22d4-151">документатионурл</span><span class="sxs-lookup"><span data-stu-id="a22d4-151">documentationUrl</span></span>|<span data-ttu-id="a22d4-152">String</span><span class="sxs-lookup"><span data-stu-id="a22d4-152">String</span></span>|<span data-ttu-id="a22d4-153">URL-адрес для установки документации</span><span class="sxs-lookup"><span data-stu-id="a22d4-153">Url to setting documentation</span></span>|
|<span data-ttu-id="a22d4-154">keywords</span><span class="sxs-lookup"><span data-stu-id="a22d4-154">keywords</span></span>|<span data-ttu-id="a22d4-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a22d4-155">String collection</span></span>|<span data-ttu-id="a22d4-156">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="a22d4-156">Keywords associated with the setting</span></span>|
|<span data-ttu-id="a22d4-157">провероч</span><span class="sxs-lookup"><span data-stu-id="a22d4-157">constraints</span></span>|<span data-ttu-id="a22d4-158">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a22d4-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="a22d4-159">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="a22d4-159">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="a22d4-160">зависящ</span><span class="sxs-lookup"><span data-stu-id="a22d4-160">dependencies</span></span>|<span data-ttu-id="a22d4-161">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="a22d4-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="a22d4-162">Коллекция зависимостей для других параметров</span><span class="sxs-lookup"><span data-stu-id="a22d4-162">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="a22d4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22d4-163">Response</span></span>
<span data-ttu-id="a22d4-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a22d4-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a22d4-165">Пример</span><span class="sxs-lookup"><span data-stu-id="a22d4-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="a22d4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="a22d4-166">Request</span></span>
<span data-ttu-id="a22d4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a22d4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="a22d4-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22d4-168">Response</span></span>
<span data-ttu-id="a22d4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a22d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```




