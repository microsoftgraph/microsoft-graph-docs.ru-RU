---
title: Создание Девицеманажементабстракткомплекссеттингдефинитион
description: Создание нового объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c5307ea1bc05cfef1a1c9ed3b8c34f6f112c5508
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181282"
---
# <a name="create-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="31ce8-103">Создание Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="31ce8-103">Create deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="31ce8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31ce8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31ce8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31ce8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31ce8-106">Создание нового объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="31ce8-106">Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31ce8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31ce8-107">Prerequisites</span></span>
<span data-ttu-id="31ce8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31ce8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31ce8-110">Permission type</span></span>|<span data-ttu-id="31ce8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31ce8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31ce8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31ce8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31ce8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31ce8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31ce8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31ce8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31ce8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31ce8-115">Not supported.</span></span>|
|<span data-ttu-id="31ce8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31ce8-116">Application</span></span>|<span data-ttu-id="31ce8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31ce8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31ce8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31ce8-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="31ce8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31ce8-119">Request headers</span></span>
|<span data-ttu-id="31ce8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31ce8-120">Header</span></span>|<span data-ttu-id="31ce8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31ce8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31ce8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31ce8-122">Authorization</span></span>|<span data-ttu-id="31ce8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31ce8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31ce8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31ce8-124">Accept</span></span>|<span data-ttu-id="31ce8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31ce8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31ce8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31ce8-126">Request body</span></span>
<span data-ttu-id="31ce8-127">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31ce8-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingDefinition object.</span></span>

<span data-ttu-id="31ce8-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="31ce8-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingDefinition.</span></span>

|<span data-ttu-id="31ce8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="31ce8-129">Property</span></span>|<span data-ttu-id="31ce8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31ce8-130">Type</span></span>|<span data-ttu-id="31ce8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31ce8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ce8-132">id</span><span class="sxs-lookup"><span data-stu-id="31ce8-132">id</span></span>|<span data-ttu-id="31ce8-133">String</span><span class="sxs-lookup"><span data-stu-id="31ce8-133">String</span></span>|<span data-ttu-id="31ce8-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-135">Типом</span><span class="sxs-lookup"><span data-stu-id="31ce8-135">valueType</span></span>|[<span data-ttu-id="31ce8-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="31ce8-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="31ce8-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ce8-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="31ce8-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="31ce8-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="31ce8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="31ce8-139">displayName</span></span>|<span data-ttu-id="31ce8-140">Строка</span><span class="sxs-lookup"><span data-stu-id="31ce8-140">String</span></span>|<span data-ttu-id="31ce8-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-142">истоплевел</span><span class="sxs-lookup"><span data-stu-id="31ce8-142">isTopLevel</span></span>|<span data-ttu-id="31ce8-143">Boolean.</span><span class="sxs-lookup"><span data-stu-id="31ce8-143">Boolean</span></span>|<span data-ttu-id="31ce8-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-145">description</span><span class="sxs-lookup"><span data-stu-id="31ce8-145">description</span></span>|<span data-ttu-id="31ce8-146">String</span><span class="sxs-lookup"><span data-stu-id="31ce8-146">String</span></span>|<span data-ttu-id="31ce8-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-148">документатионурл</span><span class="sxs-lookup"><span data-stu-id="31ce8-148">documentationUrl</span></span>|<span data-ttu-id="31ce8-149">String.</span><span class="sxs-lookup"><span data-stu-id="31ce8-149">String</span></span>|<span data-ttu-id="31ce8-150">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-151">keywords</span><span class="sxs-lookup"><span data-stu-id="31ce8-151">keywords</span></span>|<span data-ttu-id="31ce8-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="31ce8-152">String collection</span></span>|<span data-ttu-id="31ce8-153">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-154">провероч</span><span class="sxs-lookup"><span data-stu-id="31ce8-154">constraints</span></span>|<span data-ttu-id="31ce8-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="31ce8-156">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="31ce8-157">dependencies</span></span>|<span data-ttu-id="31ce8-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="31ce8-159">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ce8-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="31ce8-160">реализации</span><span class="sxs-lookup"><span data-stu-id="31ce8-160">implementations</span></span>|<span data-ttu-id="31ce8-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="31ce8-161">String collection</span></span>|<span data-ttu-id="31ce8-162">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="31ce8-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="31ce8-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="31ce8-163">Response</span></span>
<span data-ttu-id="31ce8-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31ce8-164">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31ce8-165">Пример</span><span class="sxs-lookup"><span data-stu-id="31ce8-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="31ce8-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="31ce8-166">Request</span></span>
<span data-ttu-id="31ce8-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31ce8-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 802

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="31ce8-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="31ce8-168">Response</span></span>
<span data-ttu-id="31ce8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31ce8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 851

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




