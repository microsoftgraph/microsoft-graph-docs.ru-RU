---
title: Обновление Девицеманажементабстракткомплекссеттингдефинитион
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингдефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7efaa164c8b86da08f190f651c7d49e000758bf1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916940"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="f8505-103">Обновление Девицеманажементабстракткомплекссеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="f8505-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="f8505-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8505-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8505-106">Обновление свойств объекта [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f8505-106">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8505-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8505-107">Prerequisites</span></span>
<span data-ttu-id="f8505-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8505-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8505-110">Permission type</span></span>|<span data-ttu-id="f8505-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8505-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8505-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8505-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8505-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8505-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8505-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8505-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8505-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8505-115">Not supported.</span></span>|
|<span data-ttu-id="f8505-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8505-116">Application</span></span>|<span data-ttu-id="f8505-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8505-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8505-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8505-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f8505-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8505-119">Request headers</span></span>
|<span data-ttu-id="f8505-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8505-120">Header</span></span>|<span data-ttu-id="f8505-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8505-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8505-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8505-122">Authorization</span></span>|<span data-ttu-id="f8505-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8505-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8505-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8505-124">Accept</span></span>|<span data-ttu-id="f8505-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8505-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8505-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8505-126">Request body</span></span>
<span data-ttu-id="f8505-127">В тексте запроса добавьте представление объекта [Девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8505-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="f8505-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f8505-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="f8505-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8505-129">Property</span></span>|<span data-ttu-id="f8505-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f8505-130">Type</span></span>|<span data-ttu-id="f8505-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f8505-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8505-132">id</span><span class="sxs-lookup"><span data-stu-id="f8505-132">id</span></span>|<span data-ttu-id="f8505-133">String</span><span class="sxs-lookup"><span data-stu-id="f8505-133">String</span></span>|<span data-ttu-id="f8505-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-135">Типом</span><span class="sxs-lookup"><span data-stu-id="f8505-135">valueType</span></span>|[<span data-ttu-id="f8505-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="f8505-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="f8505-137">Тип данных значения, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f8505-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="f8505-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="f8505-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="f8505-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f8505-139">displayName</span></span>|<span data-ttu-id="f8505-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f8505-140">String</span></span>|<span data-ttu-id="f8505-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-142">Истоплевел</span><span class="sxs-lookup"><span data-stu-id="f8505-142">isTopLevel</span></span>|<span data-ttu-id="f8505-143">Логический</span><span class="sxs-lookup"><span data-stu-id="f8505-143">Boolean</span></span>|<span data-ttu-id="f8505-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наследуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-145">description</span><span class="sxs-lookup"><span data-stu-id="f8505-145">description</span></span>|<span data-ttu-id="f8505-146">String</span><span class="sxs-lookup"><span data-stu-id="f8505-146">String</span></span>|<span data-ttu-id="f8505-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-148">Документатионурл</span><span class="sxs-lookup"><span data-stu-id="f8505-148">documentationUrl</span></span>|<span data-ttu-id="f8505-149">Строка</span><span class="sxs-lookup"><span data-stu-id="f8505-149">String</span></span>|<span data-ttu-id="f8505-150">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-151">keywords</span><span class="sxs-lookup"><span data-stu-id="f8505-151">keywords</span></span>|<span data-ttu-id="f8505-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f8505-152">String collection</span></span>|<span data-ttu-id="f8505-153">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-154">провероч</span><span class="sxs-lookup"><span data-stu-id="f8505-154">constraints</span></span>|<span data-ttu-id="f8505-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="f8505-156">Коллекция ограничений для значения параметра, наследуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="f8505-157">dependencies</span></span>|<span data-ttu-id="f8505-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="f8505-159">Коллекция зависимостей от других параметров, наследуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f8505-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f8505-160">реализации</span><span class="sxs-lookup"><span data-stu-id="f8505-160">implementations</span></span>|<span data-ttu-id="f8505-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f8505-161">String collection</span></span>|<span data-ttu-id="f8505-162">Список идентификаторов определений для всех возможных реализаций этого абстрактного сложного параметра</span><span class="sxs-lookup"><span data-stu-id="f8505-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="f8505-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8505-163">Response</span></span>
<span data-ttu-id="f8505-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингдефинитион](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8505-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8505-165">Пример</span><span class="sxs-lookup"><span data-stu-id="f8505-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8505-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8505-166">Request</span></span>
<span data-ttu-id="f8505-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8505-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="f8505-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8505-168">Response</span></span>
<span data-ttu-id="f8505-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8505-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




