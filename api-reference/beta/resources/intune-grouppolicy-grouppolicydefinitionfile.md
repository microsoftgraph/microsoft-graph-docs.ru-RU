---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a872671186e55524002b2d0a5f85b2ce1bbf2466
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975940"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="088e3-105">Тип ресурса Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="088e3-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="088e3-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="088e3-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="088e3-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="088e3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="088e3-108">Сущность представляет XML-файл ADMX (административный шаблон).</span><span class="sxs-lookup"><span data-stu-id="088e3-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="088e3-109">ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории.</span><span class="sxs-lookup"><span data-stu-id="088e3-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="088e3-110">В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).</span><span class="sxs-lookup"><span data-stu-id="088e3-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="088e3-111">Методы</span><span class="sxs-lookup"><span data-stu-id="088e3-111">Methods</span></span>
|<span data-ttu-id="088e3-112">Метод</span><span class="sxs-lookup"><span data-stu-id="088e3-112">Method</span></span>|<span data-ttu-id="088e3-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="088e3-113">Return Type</span></span>|<span data-ttu-id="088e3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="088e3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="088e3-115">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="088e3-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="088e3-116">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="088e3-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="088e3-117">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="088e3-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="088e3-118">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="088e3-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="088e3-119">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="088e3-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="088e3-120">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="088e3-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="088e3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="088e3-121">Properties</span></span>
|<span data-ttu-id="088e3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="088e3-122">Property</span></span>|<span data-ttu-id="088e3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="088e3-123">Type</span></span>|<span data-ttu-id="088e3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="088e3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="088e3-125">displayName</span><span class="sxs-lookup"><span data-stu-id="088e3-125">displayName</span></span>|<span data-ttu-id="088e3-126">Строка</span><span class="sxs-lookup"><span data-stu-id="088e3-126">String</span></span>|<span data-ttu-id="088e3-127">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="088e3-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="088e3-128">description</span><span class="sxs-lookup"><span data-stu-id="088e3-128">description</span></span>|<span data-ttu-id="088e3-129">String</span><span class="sxs-lookup"><span data-stu-id="088e3-129">String</span></span>|<span data-ttu-id="088e3-130">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="088e3-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="088e3-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="088e3-131">The default value is empty.</span></span>|
|<span data-ttu-id="088e3-132">Лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="088e3-132">languageCodes</span></span>|<span data-ttu-id="088e3-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="088e3-133">String collection</span></span>|<span data-ttu-id="088e3-134">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="088e3-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="088e3-135">Таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="088e3-135">targetPrefix</span></span>|<span data-ttu-id="088e3-136">String</span><span class="sxs-lookup"><span data-stu-id="088e3-136">String</span></span>|<span data-ttu-id="088e3-137">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="088e3-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="088e3-138">Атрибут</span><span class="sxs-lookup"><span data-stu-id="088e3-138">targetNamespace</span></span>|<span data-ttu-id="088e3-139">String</span><span class="sxs-lookup"><span data-stu-id="088e3-139">String</span></span>|<span data-ttu-id="088e3-140">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="088e3-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="088e3-141">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="088e3-141">policyType</span></span>|[<span data-ttu-id="088e3-142">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="088e3-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="088e3-143">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="088e3-143">Specifies the type of group policy.</span></span> <span data-ttu-id="088e3-144">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="088e3-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="088e3-145">id</span><span class="sxs-lookup"><span data-stu-id="088e3-145">id</span></span>|<span data-ttu-id="088e3-146">String</span><span class="sxs-lookup"><span data-stu-id="088e3-146">String</span></span>|<span data-ttu-id="088e3-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="088e3-147">Key of the entity.</span></span>|
|<span data-ttu-id="088e3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="088e3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="088e3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="088e3-149">DateTimeOffset</span></span>|<span data-ttu-id="088e3-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="088e3-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="088e3-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="088e3-151">Relationships</span></span>
|<span data-ttu-id="088e3-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="088e3-152">Relationship</span></span>|<span data-ttu-id="088e3-153">Тип</span><span class="sxs-lookup"><span data-stu-id="088e3-153">Type</span></span>|<span data-ttu-id="088e3-154">Описание</span><span class="sxs-lookup"><span data-stu-id="088e3-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="088e3-155">определения</span><span class="sxs-lookup"><span data-stu-id="088e3-155">definitions</span></span>|<span data-ttu-id="088e3-156">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="088e3-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="088e3-157">Определения групповой политики, связанные с файлом.</span><span class="sxs-lookup"><span data-stu-id="088e3-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="088e3-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="088e3-158">JSON Representation</span></span>
<span data-ttu-id="088e3-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="088e3-159">Here is a JSON representation of the resource.</span></span>
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





