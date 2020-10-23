---
title: Обновление Девицеманажементсеттингдефинитион
description: Обновление свойств объекта Девицеманажементсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0931fe68689fdcb0c57531a74124dda46f84133c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724285"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="9fa94-103">Обновление Девицеманажементсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="9fa94-103">Update deviceManagementSettingDefinition</span></span>

<span data-ttu-id="9fa94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fa94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fa94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa94-107">Обновление свойств объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9fa94-107">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fa94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9fa94-108">Prerequisites</span></span>
<span data-ttu-id="9fa94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fa94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fa94-111">Permission type</span></span>|<span data-ttu-id="9fa94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fa94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fa94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fa94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fa94-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa94-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fa94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fa94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fa94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa94-116">Not supported.</span></span>|
|<span data-ttu-id="9fa94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fa94-117">Application</span></span>|<span data-ttu-id="9fa94-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa94-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fa94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fa94-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9fa94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fa94-120">Request headers</span></span>
|<span data-ttu-id="9fa94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fa94-121">Header</span></span>|<span data-ttu-id="9fa94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9fa94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fa94-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fa94-123">Authorization</span></span>|<span data-ttu-id="9fa94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fa94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fa94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fa94-125">Accept</span></span>|<span data-ttu-id="9fa94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fa94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fa94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fa94-127">Request body</span></span>
<span data-ttu-id="9fa94-128">В тексте запроса добавьте представление объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fa94-128">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="9fa94-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9fa94-129">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="9fa94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fa94-130">Property</span></span>|<span data-ttu-id="9fa94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9fa94-131">Type</span></span>|<span data-ttu-id="9fa94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa94-133">id</span><span class="sxs-lookup"><span data-stu-id="9fa94-133">id</span></span>|<span data-ttu-id="9fa94-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-134">String</span></span>|<span data-ttu-id="9fa94-135">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="9fa94-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="9fa94-136">Типом</span><span class="sxs-lookup"><span data-stu-id="9fa94-136">valueType</span></span>|[<span data-ttu-id="9fa94-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="9fa94-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="9fa94-138">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="9fa94-138">The data type of the value.</span></span> <span data-ttu-id="9fa94-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="9fa94-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="9fa94-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9fa94-140">displayName</span></span>|<span data-ttu-id="9fa94-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-141">String</span></span>|<span data-ttu-id="9fa94-142">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="9fa94-142">The setting's display name</span></span>|
|<span data-ttu-id="9fa94-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="9fa94-143">isTopLevel</span></span>|<span data-ttu-id="9fa94-144">Логический</span><span class="sxs-lookup"><span data-stu-id="9fa94-144">Boolean</span></span>|<span data-ttu-id="9fa94-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.</span><span class="sxs-lookup"><span data-stu-id="9fa94-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="9fa94-146">description</span><span class="sxs-lookup"><span data-stu-id="9fa94-146">description</span></span>|<span data-ttu-id="9fa94-147">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-147">String</span></span>|<span data-ttu-id="9fa94-148">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="9fa94-148">The setting's description</span></span>|
|<span data-ttu-id="9fa94-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="9fa94-149">placeholderText</span></span>|<span data-ttu-id="9fa94-150">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-150">String</span></span>|<span data-ttu-id="9fa94-151">Замещающий текст в качестве примера допустимых входных данных</span><span class="sxs-lookup"><span data-stu-id="9fa94-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="9fa94-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="9fa94-152">documentationUrl</span></span>|<span data-ttu-id="9fa94-153">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-153">String</span></span>|<span data-ttu-id="9fa94-154">URL-адрес для установки документации</span><span class="sxs-lookup"><span data-stu-id="9fa94-154">Url to setting documentation</span></span>|
|<span data-ttu-id="9fa94-155">хеадертитле</span><span class="sxs-lookup"><span data-stu-id="9fa94-155">headerTitle</span></span>|<span data-ttu-id="9fa94-156">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-156">String</span></span>|<span data-ttu-id="9fa94-157">Заголовок параметра "заголовок" представляет категорию или раздел параметров или параметров</span><span class="sxs-lookup"><span data-stu-id="9fa94-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="9fa94-158">хеадерсубтитле</span><span class="sxs-lookup"><span data-stu-id="9fa94-158">headerSubtitle</span></span>|<span data-ttu-id="9fa94-159">Строка</span><span class="sxs-lookup"><span data-stu-id="9fa94-159">String</span></span>|<span data-ttu-id="9fa94-160">Подзаголовок заголовка параметра для дополнительных сведений о категории или разделе</span><span class="sxs-lookup"><span data-stu-id="9fa94-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="9fa94-161">keywords</span><span class="sxs-lookup"><span data-stu-id="9fa94-161">keywords</span></span>|<span data-ttu-id="9fa94-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fa94-162">String collection</span></span>|<span data-ttu-id="9fa94-163">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="9fa94-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="9fa94-164">провероч</span><span class="sxs-lookup"><span data-stu-id="9fa94-164">constraints</span></span>|<span data-ttu-id="9fa94-165">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9fa94-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="9fa94-166">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="9fa94-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="9fa94-167">зависящ</span><span class="sxs-lookup"><span data-stu-id="9fa94-167">dependencies</span></span>|<span data-ttu-id="9fa94-168">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="9fa94-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="9fa94-169">Коллекция зависимостей для других параметров</span><span class="sxs-lookup"><span data-stu-id="9fa94-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="9fa94-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fa94-170">Response</span></span>
<span data-ttu-id="9fa94-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fa94-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fa94-172">Пример</span><span class="sxs-lookup"><span data-stu-id="9fa94-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fa94-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fa94-173">Request</span></span>
<span data-ttu-id="9fa94-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fa94-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1014

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="9fa94-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fa94-175">Response</span></span>
<span data-ttu-id="9fa94-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fa94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1063

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```





