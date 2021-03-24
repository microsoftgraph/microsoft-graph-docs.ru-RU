---
title: Обновление deviceManagementSettingDefinition
description: Обновление свойств объекта deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343971cccdbcf64bbb04279de069ac3e0020362f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146575"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="7196c-103">Обновление deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="7196c-103">Update deviceManagementSettingDefinition</span></span>

<span data-ttu-id="7196c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7196c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7196c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7196c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7196c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7196c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7196c-107">Обновление свойств объекта [deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7196c-107">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7196c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7196c-108">Prerequisites</span></span>
<span data-ttu-id="7196c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7196c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7196c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7196c-111">Permission type</span></span>|<span data-ttu-id="7196c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7196c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7196c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7196c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7196c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7196c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7196c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7196c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7196c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7196c-116">Not supported.</span></span>|
|<span data-ttu-id="7196c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7196c-117">Application</span></span>|<span data-ttu-id="7196c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7196c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7196c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7196c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7196c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7196c-120">Request headers</span></span>
|<span data-ttu-id="7196c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7196c-121">Header</span></span>|<span data-ttu-id="7196c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7196c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7196c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7196c-123">Authorization</span></span>|<span data-ttu-id="7196c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7196c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7196c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7196c-125">Accept</span></span>|<span data-ttu-id="7196c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7196c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7196c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7196c-127">Request body</span></span>
<span data-ttu-id="7196c-128">В теле запроса поставляем представление JSON для [объекта deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7196c-128">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="7196c-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7196c-129">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="7196c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7196c-130">Property</span></span>|<span data-ttu-id="7196c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7196c-131">Type</span></span>|<span data-ttu-id="7196c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7196c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7196c-133">id</span><span class="sxs-lookup"><span data-stu-id="7196c-133">id</span></span>|<span data-ttu-id="7196c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-134">String</span></span>|<span data-ttu-id="7196c-135">ID определения параметра</span><span class="sxs-lookup"><span data-stu-id="7196c-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="7196c-136">valueType</span><span class="sxs-lookup"><span data-stu-id="7196c-136">valueType</span></span>|[<span data-ttu-id="7196c-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="7196c-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="7196c-138">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="7196c-138">The data type of the value.</span></span> <span data-ttu-id="7196c-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="7196c-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="7196c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7196c-140">displayName</span></span>|<span data-ttu-id="7196c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-141">String</span></span>|<span data-ttu-id="7196c-142">Имя отображения параметра</span><span class="sxs-lookup"><span data-stu-id="7196c-142">The setting's display name</span></span>|
|<span data-ttu-id="7196c-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="7196c-143">isTopLevel</span></span>|<span data-ttu-id="7196c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="7196c-144">Boolean</span></span>|<span data-ttu-id="7196c-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр</span><span class="sxs-lookup"><span data-stu-id="7196c-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="7196c-146">description</span><span class="sxs-lookup"><span data-stu-id="7196c-146">description</span></span>|<span data-ttu-id="7196c-147">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-147">String</span></span>|<span data-ttu-id="7196c-148">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="7196c-148">The setting's description</span></span>|
|<span data-ttu-id="7196c-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="7196c-149">placeholderText</span></span>|<span data-ttu-id="7196c-150">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-150">String</span></span>|<span data-ttu-id="7196c-151">Текст placeholder в качестве примера допустимого ввода</span><span class="sxs-lookup"><span data-stu-id="7196c-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="7196c-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="7196c-152">documentationUrl</span></span>|<span data-ttu-id="7196c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-153">String</span></span>|<span data-ttu-id="7196c-154">URL-адрес для настройки документации</span><span class="sxs-lookup"><span data-stu-id="7196c-154">Url to setting documentation</span></span>|
|<span data-ttu-id="7196c-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="7196c-155">headerTitle</span></span>|<span data-ttu-id="7196c-156">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-156">String</span></span>|<span data-ttu-id="7196c-157">заголовок параметра представляет категорию/раздел параметра/параметров</span><span class="sxs-lookup"><span data-stu-id="7196c-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="7196c-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="7196c-158">headerSubtitle</span></span>|<span data-ttu-id="7196c-159">Строка</span><span class="sxs-lookup"><span data-stu-id="7196c-159">String</span></span>|<span data-ttu-id="7196c-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе</span><span class="sxs-lookup"><span data-stu-id="7196c-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="7196c-161">keywords</span><span class="sxs-lookup"><span data-stu-id="7196c-161">keywords</span></span>|<span data-ttu-id="7196c-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7196c-162">String collection</span></span>|<span data-ttu-id="7196c-163">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="7196c-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="7196c-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="7196c-164">constraints</span></span>|<span data-ttu-id="7196c-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="7196c-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="7196c-166">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="7196c-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="7196c-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="7196c-167">dependencies</span></span>|<span data-ttu-id="7196c-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="7196c-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="7196c-169">Коллекция зависимостей от других параметров</span><span class="sxs-lookup"><span data-stu-id="7196c-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="7196c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="7196c-170">Response</span></span>
<span data-ttu-id="7196c-171">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7196c-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7196c-172">Пример</span><span class="sxs-lookup"><span data-stu-id="7196c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7196c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="7196c-173">Request</span></span>
<span data-ttu-id="7196c-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7196c-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7196c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="7196c-175">Response</span></span>
<span data-ttu-id="7196c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7196c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




