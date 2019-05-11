---
title: Создание Девицеманажементсеттингдефинитион
description: Создание нового объекта Девицеманажементсеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9062c48fbf3be9ab33f8abc3f7ecebc40eeef0b6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915671"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="55efc-103">Создание Девицеманажементсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="55efc-103">Create deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="55efc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55efc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55efc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55efc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55efc-106">Создание нового объекта [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="55efc-106">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55efc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55efc-107">Prerequisites</span></span>
<span data-ttu-id="55efc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55efc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55efc-110">Permission type</span></span>|<span data-ttu-id="55efc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55efc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55efc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55efc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55efc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55efc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55efc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55efc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55efc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55efc-115">Not supported.</span></span>|
|<span data-ttu-id="55efc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55efc-116">Application</span></span>|<span data-ttu-id="55efc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55efc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55efc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55efc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="55efc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55efc-119">Request headers</span></span>
|<span data-ttu-id="55efc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55efc-120">Header</span></span>|<span data-ttu-id="55efc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55efc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55efc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55efc-122">Authorization</span></span>|<span data-ttu-id="55efc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55efc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55efc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55efc-124">Accept</span></span>|<span data-ttu-id="55efc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55efc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55efc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55efc-126">Request body</span></span>
<span data-ttu-id="55efc-127">В тексте запроса добавьте представление объекта Девицеманажементсеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55efc-127">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="55efc-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементсеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="55efc-128">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="55efc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55efc-129">Property</span></span>|<span data-ttu-id="55efc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55efc-130">Type</span></span>|<span data-ttu-id="55efc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55efc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55efc-132">id</span><span class="sxs-lookup"><span data-stu-id="55efc-132">id</span></span>|<span data-ttu-id="55efc-133">String</span><span class="sxs-lookup"><span data-stu-id="55efc-133">String</span></span>|<span data-ttu-id="55efc-134">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="55efc-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="55efc-135">Типом</span><span class="sxs-lookup"><span data-stu-id="55efc-135">valueType</span></span>|[<span data-ttu-id="55efc-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="55efc-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="55efc-137">Тип данных значения.</span><span class="sxs-lookup"><span data-stu-id="55efc-137">The data type of the value.</span></span> <span data-ttu-id="55efc-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="55efc-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="55efc-139">displayName</span><span class="sxs-lookup"><span data-stu-id="55efc-139">displayName</span></span>|<span data-ttu-id="55efc-140">Строка</span><span class="sxs-lookup"><span data-stu-id="55efc-140">String</span></span>|<span data-ttu-id="55efc-141">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="55efc-141">The setting's display name</span></span>|
|<span data-ttu-id="55efc-142">Истоплевел</span><span class="sxs-lookup"><span data-stu-id="55efc-142">isTopLevel</span></span>|<span data-ttu-id="55efc-143">Логический</span><span class="sxs-lookup"><span data-stu-id="55efc-143">Boolean</span></span>|<span data-ttu-id="55efc-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр.</span><span class="sxs-lookup"><span data-stu-id="55efc-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="55efc-145">description</span><span class="sxs-lookup"><span data-stu-id="55efc-145">description</span></span>|<span data-ttu-id="55efc-146">String</span><span class="sxs-lookup"><span data-stu-id="55efc-146">String</span></span>|<span data-ttu-id="55efc-147">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="55efc-147">The setting's description</span></span>|
|<span data-ttu-id="55efc-148">Документатионурл</span><span class="sxs-lookup"><span data-stu-id="55efc-148">documentationUrl</span></span>|<span data-ttu-id="55efc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="55efc-149">String</span></span>|<span data-ttu-id="55efc-150">URL-адрес для установки документации</span><span class="sxs-lookup"><span data-stu-id="55efc-150">Url to setting documentation</span></span>|
|<span data-ttu-id="55efc-151">keywords</span><span class="sxs-lookup"><span data-stu-id="55efc-151">keywords</span></span>|<span data-ttu-id="55efc-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="55efc-152">String collection</span></span>|<span data-ttu-id="55efc-153">Ключевые слова, связанные с параметром</span><span class="sxs-lookup"><span data-stu-id="55efc-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="55efc-154">провероч</span><span class="sxs-lookup"><span data-stu-id="55efc-154">constraints</span></span>|<span data-ttu-id="55efc-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="55efc-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="55efc-156">Коллекция ограничений для значения параметра</span><span class="sxs-lookup"><span data-stu-id="55efc-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="55efc-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="55efc-157">dependencies</span></span>|<span data-ttu-id="55efc-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="55efc-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="55efc-159">Коллекция зависимостей для других параметров</span><span class="sxs-lookup"><span data-stu-id="55efc-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="55efc-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="55efc-160">Response</span></span>
<span data-ttu-id="55efc-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55efc-161">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55efc-162">Пример</span><span class="sxs-lookup"><span data-stu-id="55efc-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="55efc-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="55efc-163">Request</span></span>
<span data-ttu-id="55efc-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55efc-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="55efc-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="55efc-165">Response</span></span>
<span data-ttu-id="55efc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55efc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```




