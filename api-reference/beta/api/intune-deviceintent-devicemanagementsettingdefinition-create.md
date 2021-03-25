---
title: Создание deviceManagementSettingDefinition
description: Создание нового объекта deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e93bd4424d4e09fb27528d719898067f192aa345
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154583"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="df6a8-103">Создание deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="df6a8-103">Create deviceManagementSettingDefinition</span></span>

<span data-ttu-id="df6a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df6a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df6a8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df6a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df6a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df6a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df6a8-107">Создание нового [объекта deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="df6a8-107">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df6a8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df6a8-108">Prerequisites</span></span>
<span data-ttu-id="df6a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df6a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df6a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df6a8-111">Permission type</span></span>|<span data-ttu-id="df6a8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df6a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df6a8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df6a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df6a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df6a8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df6a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df6a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df6a8-116">Not supported.</span></span>|
|<span data-ttu-id="df6a8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="df6a8-117">Application</span></span>|<span data-ttu-id="df6a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df6a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df6a8-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="df6a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df6a8-120">Request headers</span></span>
|<span data-ttu-id="df6a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df6a8-121">Header</span></span>|<span data-ttu-id="df6a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df6a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df6a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df6a8-123">Authorization</span></span>|<span data-ttu-id="df6a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df6a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df6a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df6a8-125">Accept</span></span>|<span data-ttu-id="df6a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df6a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df6a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df6a8-127">Request body</span></span>
<span data-ttu-id="df6a8-128">В теле запроса поставляем представление JSON для объекта deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="df6a8-128">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="df6a8-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="df6a8-129">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="df6a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df6a8-130">Property</span></span>|<span data-ttu-id="df6a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df6a8-131">Type</span></span>|<span data-ttu-id="df6a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df6a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df6a8-133">id</span><span class="sxs-lookup"><span data-stu-id="df6a8-133">id</span></span>|<span data-ttu-id="df6a8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-134">String</span></span>|<span data-ttu-id="df6a8-135">ID определения параметра</span><span class="sxs-lookup"><span data-stu-id="df6a8-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="df6a8-136">valueType</span><span class="sxs-lookup"><span data-stu-id="df6a8-136">valueType</span></span>|[<span data-ttu-id="df6a8-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="df6a8-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="df6a8-138">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="df6a8-138">The data type of the value.</span></span> <span data-ttu-id="df6a8-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="df6a8-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="df6a8-140">displayName</span><span class="sxs-lookup"><span data-stu-id="df6a8-140">displayName</span></span>|<span data-ttu-id="df6a8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-141">String</span></span>|<span data-ttu-id="df6a8-142">Имя отображения параметра</span><span class="sxs-lookup"><span data-stu-id="df6a8-142">The setting's display name</span></span>|
|<span data-ttu-id="df6a8-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="df6a8-143">isTopLevel</span></span>|<span data-ttu-id="df6a8-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="df6a8-144">Boolean</span></span>|<span data-ttu-id="df6a8-145">Если параметр верхнего уровня, его можно настроить без необходимости завернутой в коллекцию или сложный параметр</span><span class="sxs-lookup"><span data-stu-id="df6a8-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="df6a8-146">description</span><span class="sxs-lookup"><span data-stu-id="df6a8-146">description</span></span>|<span data-ttu-id="df6a8-147">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-147">String</span></span>|<span data-ttu-id="df6a8-148">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="df6a8-148">The setting's description</span></span>|
|<span data-ttu-id="df6a8-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="df6a8-149">placeholderText</span></span>|<span data-ttu-id="df6a8-150">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-150">String</span></span>|<span data-ttu-id="df6a8-151">Текст placeholder в качестве примера допустимого ввода</span><span class="sxs-lookup"><span data-stu-id="df6a8-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="df6a8-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="df6a8-152">documentationUrl</span></span>|<span data-ttu-id="df6a8-153">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-153">String</span></span>|<span data-ttu-id="df6a8-154">URL-адрес для настройки документации</span><span class="sxs-lookup"><span data-stu-id="df6a8-154">Url to setting documentation</span></span>|
|<span data-ttu-id="df6a8-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="df6a8-155">headerTitle</span></span>|<span data-ttu-id="df6a8-156">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-156">String</span></span>|<span data-ttu-id="df6a8-157">заголовок параметра представляет категорию/раздел параметра/параметров</span><span class="sxs-lookup"><span data-stu-id="df6a8-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="df6a8-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="df6a8-158">headerSubtitle</span></span>|<span data-ttu-id="df6a8-159">Строка</span><span class="sxs-lookup"><span data-stu-id="df6a8-159">String</span></span>|<span data-ttu-id="df6a8-160">субтитры заголовок параметра для получения дополнительных сведений о категории/разделе</span><span class="sxs-lookup"><span data-stu-id="df6a8-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="df6a8-161">keywords</span><span class="sxs-lookup"><span data-stu-id="df6a8-161">keywords</span></span>|<span data-ttu-id="df6a8-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="df6a8-162">String collection</span></span>|<span data-ttu-id="df6a8-163">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="df6a8-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="df6a8-164">ограничения</span><span class="sxs-lookup"><span data-stu-id="df6a8-164">constraints</span></span>|<span data-ttu-id="df6a8-165">[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="df6a8-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="df6a8-166">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="df6a8-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="df6a8-167">зависимости</span><span class="sxs-lookup"><span data-stu-id="df6a8-167">dependencies</span></span>|<span data-ttu-id="df6a8-168">[коллекция deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="df6a8-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="df6a8-169">Коллекция зависимостей от других параметров</span><span class="sxs-lookup"><span data-stu-id="df6a8-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="df6a8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="df6a8-170">Response</span></span>
<span data-ttu-id="df6a8-171">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="df6a8-171">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df6a8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="df6a8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="df6a8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="df6a8-173">Request</span></span>
<span data-ttu-id="df6a8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df6a8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="df6a8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="df6a8-175">Response</span></span>
<span data-ttu-id="df6a8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df6a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




