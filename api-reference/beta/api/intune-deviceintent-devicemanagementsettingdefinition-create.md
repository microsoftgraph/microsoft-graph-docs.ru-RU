---
title: Создание Девицеманажементсеттингдефинитион
description: Создание нового объекта Девицеманажементсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba658fe605034703c2565f3f8f3a6d70cd6685de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427818"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="0194c-103">Создание Девицеманажементсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="0194c-103">Create deviceManagementSettingDefinition</span></span>

<span data-ttu-id="0194c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0194c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0194c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0194c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0194c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0194c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0194c-107">Создание нового объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0194c-107">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0194c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0194c-108">Prerequisites</span></span>
<span data-ttu-id="0194c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0194c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0194c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0194c-111">Permission type</span></span>|<span data-ttu-id="0194c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0194c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0194c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0194c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0194c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0194c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0194c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0194c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0194c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0194c-116">Not supported.</span></span>|
|<span data-ttu-id="0194c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0194c-117">Application</span></span>|<span data-ttu-id="0194c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0194c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0194c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0194c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0194c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0194c-120">Request headers</span></span>
|<span data-ttu-id="0194c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0194c-121">Header</span></span>|<span data-ttu-id="0194c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0194c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0194c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0194c-123">Authorization</span></span>|<span data-ttu-id="0194c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0194c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0194c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0194c-125">Accept</span></span>|<span data-ttu-id="0194c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0194c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0194c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0194c-127">Request body</span></span>
<span data-ttu-id="0194c-128">В тексте запроса добавьте представление объекта Девицеманажементсеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0194c-128">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="0194c-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="0194c-129">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="0194c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0194c-130">Property</span></span>|<span data-ttu-id="0194c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0194c-131">Type</span></span>|<span data-ttu-id="0194c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0194c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0194c-133">id</span><span class="sxs-lookup"><span data-stu-id="0194c-133">id</span></span>|<span data-ttu-id="0194c-134">String</span><span class="sxs-lookup"><span data-stu-id="0194c-134">String</span></span>|<span data-ttu-id="0194c-135">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="0194c-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="0194c-136">Типом</span><span class="sxs-lookup"><span data-stu-id="0194c-136">valueType</span></span>|[<span data-ttu-id="0194c-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="0194c-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="0194c-138">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="0194c-138">The data type of the value.</span></span> <span data-ttu-id="0194c-139">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="0194c-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="0194c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0194c-140">displayName</span></span>|<span data-ttu-id="0194c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0194c-141">String</span></span>|<span data-ttu-id="0194c-142">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="0194c-142">The setting's display name</span></span>|
|<span data-ttu-id="0194c-143">истоплевел</span><span class="sxs-lookup"><span data-stu-id="0194c-143">isTopLevel</span></span>|<span data-ttu-id="0194c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="0194c-144">Boolean</span></span>|<span data-ttu-id="0194c-145">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.</span><span class="sxs-lookup"><span data-stu-id="0194c-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="0194c-146">description</span><span class="sxs-lookup"><span data-stu-id="0194c-146">description</span></span>|<span data-ttu-id="0194c-147">String</span><span class="sxs-lookup"><span data-stu-id="0194c-147">String</span></span>|<span data-ttu-id="0194c-148">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="0194c-148">The setting's description</span></span>|
|<span data-ttu-id="0194c-149">плацехолдертекст</span><span class="sxs-lookup"><span data-stu-id="0194c-149">placeholderText</span></span>|<span data-ttu-id="0194c-150">String</span><span class="sxs-lookup"><span data-stu-id="0194c-150">String</span></span>|<span data-ttu-id="0194c-151">Замещающий текст в качестве примера допустимых входных данных</span><span class="sxs-lookup"><span data-stu-id="0194c-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="0194c-152">документатионурл</span><span class="sxs-lookup"><span data-stu-id="0194c-152">documentationUrl</span></span>|<span data-ttu-id="0194c-153">String</span><span class="sxs-lookup"><span data-stu-id="0194c-153">String</span></span>|<span data-ttu-id="0194c-154">URL-адрес для установки документации</span><span class="sxs-lookup"><span data-stu-id="0194c-154">Url to setting documentation</span></span>|
|<span data-ttu-id="0194c-155">keywords</span><span class="sxs-lookup"><span data-stu-id="0194c-155">keywords</span></span>|<span data-ttu-id="0194c-156">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0194c-156">String collection</span></span>|<span data-ttu-id="0194c-157">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="0194c-157">Keywords associated with the setting</span></span>|
|<span data-ttu-id="0194c-158">провероч</span><span class="sxs-lookup"><span data-stu-id="0194c-158">constraints</span></span>|<span data-ttu-id="0194c-159">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0194c-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="0194c-160">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="0194c-160">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="0194c-161">зависящ</span><span class="sxs-lookup"><span data-stu-id="0194c-161">dependencies</span></span>|<span data-ttu-id="0194c-162">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="0194c-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="0194c-163">Коллекция зависимостей для других параметров</span><span class="sxs-lookup"><span data-stu-id="0194c-163">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="0194c-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="0194c-164">Response</span></span>
<span data-ttu-id="0194c-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0194c-165">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0194c-166">Пример</span><span class="sxs-lookup"><span data-stu-id="0194c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="0194c-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="0194c-167">Request</span></span>
<span data-ttu-id="0194c-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0194c-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="0194c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="0194c-169">Response</span></span>
<span data-ttu-id="0194c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0194c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



