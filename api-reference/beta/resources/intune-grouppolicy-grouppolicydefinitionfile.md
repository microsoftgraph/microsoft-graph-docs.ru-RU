---
title: Тип ресурса groupPolicyDefinitionFile
description: Объект представляет ADMX (административных шаблонов) XML-файла. Файл ADMX содержит коллекцию определений групповой политики и их расположение по пути к категории. Файл определения групповой политике также содержит языки, поддерживаемые согласно языковых файлов языка зависимые ADML (административный шаблон).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431711"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="29999-105">Тип ресурса groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="29999-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="29999-106">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29999-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29999-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29999-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29999-108">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29999-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29999-109">Объект представляет ADMX (административных шаблонов) XML-файла.</span><span class="sxs-lookup"><span data-stu-id="29999-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="29999-110">Файл ADMX содержит коллекцию определений групповой политики и их расположение по пути к категории.</span><span class="sxs-lookup"><span data-stu-id="29999-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="29999-111">Файл определения групповой политике также содержит языки, поддерживаемые согласно языковых файлов языка зависимые ADML (административный шаблон).</span><span class="sxs-lookup"><span data-stu-id="29999-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="29999-112">Методы</span><span class="sxs-lookup"><span data-stu-id="29999-112">Methods</span></span>
|<span data-ttu-id="29999-113">Метод</span><span class="sxs-lookup"><span data-stu-id="29999-113">Method</span></span>|<span data-ttu-id="29999-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29999-114">Return Type</span></span>|<span data-ttu-id="29999-115">Описание</span><span class="sxs-lookup"><span data-stu-id="29999-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29999-116">Получение groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="29999-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="29999-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="29999-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="29999-118">Чтение свойства и связи объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="29999-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="29999-119">Обновление groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="29999-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="29999-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="29999-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="29999-121">Обновление свойства объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="29999-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29999-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="29999-122">Properties</span></span>
|<span data-ttu-id="29999-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="29999-123">Property</span></span>|<span data-ttu-id="29999-124">Тип</span><span class="sxs-lookup"><span data-stu-id="29999-124">Type</span></span>|<span data-ttu-id="29999-125">Описание</span><span class="sxs-lookup"><span data-stu-id="29999-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29999-126">displayName</span><span class="sxs-lookup"><span data-stu-id="29999-126">displayName</span></span>|<span data-ttu-id="29999-127">String</span><span class="sxs-lookup"><span data-stu-id="29999-127">String</span></span>|<span data-ttu-id="29999-128">Локализованные понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="29999-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="29999-129">description</span><span class="sxs-lookup"><span data-stu-id="29999-129">description</span></span>|<span data-ttu-id="29999-130">String</span><span class="sxs-lookup"><span data-stu-id="29999-130">String</span></span>|<span data-ttu-id="29999-131">Локализованное описание параметров политики в ADMX-файле.</span><span class="sxs-lookup"><span data-stu-id="29999-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="29999-132">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="29999-132">The default value is empty.</span></span>|
|<span data-ttu-id="29999-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="29999-133">languageCodes</span></span>|<span data-ttu-id="29999-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="29999-134">String collection</span></span>|<span data-ttu-id="29999-135">Коды поддерживаемых языков для файлов ADMX.</span><span class="sxs-lookup"><span data-stu-id="29999-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="29999-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="29999-136">targetPrefix</span></span>|<span data-ttu-id="29999-137">String</span><span class="sxs-lookup"><span data-stu-id="29999-137">String</span></span>|<span data-ttu-id="29999-138">Задает логическое имя, которое относится к области имен файлах.</span><span class="sxs-lookup"><span data-stu-id="29999-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="29999-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="29999-139">targetNamespace</span></span>|<span data-ttu-id="29999-140">String</span><span class="sxs-lookup"><span data-stu-id="29999-140">String</span></span>|<span data-ttu-id="29999-141">Указывает URI, используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="29999-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="29999-142">policyType</span><span class="sxs-lookup"><span data-stu-id="29999-142">policyType</span></span>|[<span data-ttu-id="29999-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="29999-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="29999-144">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="29999-144">Specifies the type of group policy.</span></span> <span data-ttu-id="29999-145">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="29999-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="29999-146">id</span><span class="sxs-lookup"><span data-stu-id="29999-146">id</span></span>|<span data-ttu-id="29999-147">String</span><span class="sxs-lookup"><span data-stu-id="29999-147">String</span></span>|<span data-ttu-id="29999-148">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="29999-148">Key of the entity.</span></span>|
|<span data-ttu-id="29999-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29999-149">lastModifiedDateTime</span></span>|<span data-ttu-id="29999-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29999-150">DateTimeOffset</span></span>|<span data-ttu-id="29999-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="29999-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29999-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="29999-152">Relationships</span></span>
|<span data-ttu-id="29999-153">Связь</span><span class="sxs-lookup"><span data-stu-id="29999-153">Relationship</span></span>|<span data-ttu-id="29999-154">Тип</span><span class="sxs-lookup"><span data-stu-id="29999-154">Type</span></span>|<span data-ttu-id="29999-155">Описание</span><span class="sxs-lookup"><span data-stu-id="29999-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29999-156">определения</span><span class="sxs-lookup"><span data-stu-id="29999-156">definitions</span></span>|<span data-ttu-id="29999-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="29999-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="29999-158">Определения групповой политики, связанные с этим файлом.</span><span class="sxs-lookup"><span data-stu-id="29999-158">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29999-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29999-159">JSON Representation</span></span>
<span data-ttu-id="29999-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29999-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




