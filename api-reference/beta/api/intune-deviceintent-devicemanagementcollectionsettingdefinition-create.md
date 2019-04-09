---
title: Создание Девицеманажементколлектионсеттингдефинитион
description: Создание нового объекта Девицеманажементколлектионсеттингдефинитион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9f484bf5bfccd0600b735d2f826a742784e87ca
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522568"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="6aa23-103">Создание Девицеманажементколлектионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="6aa23-103">Create deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="6aa23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aa23-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6aa23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aa23-106">Создание нового объекта [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6aa23-106">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aa23-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6aa23-107">Prerequisites</span></span>
<span data-ttu-id="6aa23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa23-110">Permission type</span></span>|<span data-ttu-id="6aa23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aa23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aa23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aa23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa23-115">Not supported.</span></span>|
|<span data-ttu-id="6aa23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aa23-116">Application</span></span>|<span data-ttu-id="6aa23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aa23-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6aa23-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6aa23-119">Request headers</span></span>
|<span data-ttu-id="6aa23-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aa23-120">Header</span></span>|<span data-ttu-id="6aa23-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6aa23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aa23-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6aa23-122">Authorization</span></span>|<span data-ttu-id="6aa23-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aa23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aa23-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6aa23-124">Accept</span></span>|<span data-ttu-id="6aa23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa23-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aa23-126">Request body</span></span>
<span data-ttu-id="6aa23-127">В тексте запроса добавьте представление объекта Девицеманажементколлектионсеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa23-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="6aa23-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементколлектионсеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="6aa23-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="6aa23-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aa23-129">Property</span></span>|<span data-ttu-id="6aa23-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6aa23-130">Type</span></span>|<span data-ttu-id="6aa23-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aa23-132">id</span><span class="sxs-lookup"><span data-stu-id="6aa23-132">id</span></span>|<span data-ttu-id="6aa23-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6aa23-133">String</span></span>|<span data-ttu-id="6aa23-134">Идентификатор определения параметра, унаследованного от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-135">Типом</span><span class="sxs-lookup"><span data-stu-id="6aa23-135">valueType</span></span>|[<span data-ttu-id="6aa23-136">Девицемананжементинтентвалуетипе</span><span class="sxs-lookup"><span data-stu-id="6aa23-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="6aa23-137">Тип данных значения, наСледуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6aa23-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="6aa23-138">Возможные значения: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="6aa23-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="6aa23-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6aa23-139">displayName</span></span>|<span data-ttu-id="6aa23-140">String</span><span class="sxs-lookup"><span data-stu-id="6aa23-140">String</span></span>|<span data-ttu-id="6aa23-141">Отображаемое имя параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-142">Истоплевел</span><span class="sxs-lookup"><span data-stu-id="6aa23-142">isTopLevel</span></span>|<span data-ttu-id="6aa23-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aa23-143">Boolean</span></span>|<span data-ttu-id="6aa23-144">Если параметр находится в верхнем уровне, его можно настроить без переноса в коллекцию или сложный параметр, наСледуемый от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-145">description</span><span class="sxs-lookup"><span data-stu-id="6aa23-145">description</span></span>|<span data-ttu-id="6aa23-146">String</span><span class="sxs-lookup"><span data-stu-id="6aa23-146">String</span></span>|<span data-ttu-id="6aa23-147">Описание параметра, унаследованное от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-148">Документатионурл</span><span class="sxs-lookup"><span data-stu-id="6aa23-148">documentationUrl</span></span>|<span data-ttu-id="6aa23-149">String</span><span class="sxs-lookup"><span data-stu-id="6aa23-149">String</span></span>|<span data-ttu-id="6aa23-150">URL-адрес для установки документации, унаследованной от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-151">keywords</span><span class="sxs-lookup"><span data-stu-id="6aa23-151">keywords</span></span>|<span data-ttu-id="6aa23-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6aa23-152">String collection</span></span>|<span data-ttu-id="6aa23-153">Ключевые слова, связанные с параметром, унаследованным от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-154">провероч</span><span class="sxs-lookup"><span data-stu-id="6aa23-154">constraints</span></span>|<span data-ttu-id="6aa23-155">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="6aa23-156">Коллекция ограничений для значения параметра, наСледуемого из [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-157">зависящ</span><span class="sxs-lookup"><span data-stu-id="6aa23-157">dependencies</span></span>|<span data-ttu-id="6aa23-158">Коллекция [девицеманажементсеттингдепенденци](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="6aa23-159">Коллекция зависимостей от других параметров, наСледуемых от [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6aa23-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="6aa23-160">Елементдефинитионид</span><span class="sxs-lookup"><span data-stu-id="6aa23-160">elementDefinitionId</span></span>|<span data-ttu-id="6aa23-161">String</span><span class="sxs-lookup"><span data-stu-id="6aa23-161">String</span></span>|<span data-ttu-id="6aa23-162">Идентификатор определения параметра, описывающий, как выглядит каждый элемент коллекции</span><span class="sxs-lookup"><span data-stu-id="6aa23-162">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="6aa23-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa23-163">Response</span></span>
<span data-ttu-id="6aa23-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементколлектионсеттингдефинитион](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6aa23-164">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa23-165">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa23-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aa23-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aa23-166">Request</span></span>
<span data-ttu-id="6aa23-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aa23-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="6aa23-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa23-168">Response</span></span>
<span data-ttu-id="6aa23-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aa23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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







