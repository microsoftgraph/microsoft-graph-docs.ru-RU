---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 384b59a2c9e1b669cd71b294c6420c13b95d1102
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576489"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="64146-105">Тип ресурса Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="64146-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="64146-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64146-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64146-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64146-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64146-108">Сущность представляет XML-файл ADMX (административный шаблон).</span><span class="sxs-lookup"><span data-stu-id="64146-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="64146-109">ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории.</span><span class="sxs-lookup"><span data-stu-id="64146-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="64146-110">В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).</span><span class="sxs-lookup"><span data-stu-id="64146-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="64146-111">Методы</span><span class="sxs-lookup"><span data-stu-id="64146-111">Methods</span></span>
|<span data-ttu-id="64146-112">Метод</span><span class="sxs-lookup"><span data-stu-id="64146-112">Method</span></span>|<span data-ttu-id="64146-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64146-113">Return Type</span></span>|<span data-ttu-id="64146-114">Описание</span><span class="sxs-lookup"><span data-stu-id="64146-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64146-115">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="64146-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="64146-116">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="64146-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="64146-117">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="64146-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="64146-118">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="64146-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="64146-119">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="64146-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="64146-120">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="64146-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="64146-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="64146-121">Properties</span></span>
|<span data-ttu-id="64146-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="64146-122">Property</span></span>|<span data-ttu-id="64146-123">Тип</span><span class="sxs-lookup"><span data-stu-id="64146-123">Type</span></span>|<span data-ttu-id="64146-124">Описание</span><span class="sxs-lookup"><span data-stu-id="64146-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64146-125">displayName</span><span class="sxs-lookup"><span data-stu-id="64146-125">displayName</span></span>|<span data-ttu-id="64146-126">Строка</span><span class="sxs-lookup"><span data-stu-id="64146-126">String</span></span>|<span data-ttu-id="64146-127">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="64146-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="64146-128">description</span><span class="sxs-lookup"><span data-stu-id="64146-128">description</span></span>|<span data-ttu-id="64146-129">String</span><span class="sxs-lookup"><span data-stu-id="64146-129">String</span></span>|<span data-ttu-id="64146-130">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="64146-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="64146-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="64146-131">The default value is empty.</span></span>|
|<span data-ttu-id="64146-132">Лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="64146-132">languageCodes</span></span>|<span data-ttu-id="64146-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64146-133">String collection</span></span>|<span data-ttu-id="64146-134">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="64146-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="64146-135">Таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="64146-135">targetPrefix</span></span>|<span data-ttu-id="64146-136">String</span><span class="sxs-lookup"><span data-stu-id="64146-136">String</span></span>|<span data-ttu-id="64146-137">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="64146-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="64146-138">Атрибут</span><span class="sxs-lookup"><span data-stu-id="64146-138">targetNamespace</span></span>|<span data-ttu-id="64146-139">String</span><span class="sxs-lookup"><span data-stu-id="64146-139">String</span></span>|<span data-ttu-id="64146-140">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="64146-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="64146-141">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="64146-141">policyType</span></span>|[<span data-ttu-id="64146-142">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="64146-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="64146-143">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="64146-143">Specifies the type of group policy.</span></span> <span data-ttu-id="64146-144">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="64146-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="64146-145">последним</span><span class="sxs-lookup"><span data-stu-id="64146-145">revision</span></span>|<span data-ttu-id="64146-146">String</span><span class="sxs-lookup"><span data-stu-id="64146-146">String</span></span>|<span data-ttu-id="64146-147">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="64146-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="64146-148">id</span><span class="sxs-lookup"><span data-stu-id="64146-148">id</span></span>|<span data-ttu-id="64146-149">String</span><span class="sxs-lookup"><span data-stu-id="64146-149">String</span></span>|<span data-ttu-id="64146-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64146-150">Key of the entity.</span></span>|
|<span data-ttu-id="64146-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64146-151">lastModifiedDateTime</span></span>|<span data-ttu-id="64146-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64146-152">DateTimeOffset</span></span>|<span data-ttu-id="64146-153">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="64146-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64146-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="64146-154">Relationships</span></span>
|<span data-ttu-id="64146-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="64146-155">Relationship</span></span>|<span data-ttu-id="64146-156">Тип</span><span class="sxs-lookup"><span data-stu-id="64146-156">Type</span></span>|<span data-ttu-id="64146-157">Описание</span><span class="sxs-lookup"><span data-stu-id="64146-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64146-158">определения</span><span class="sxs-lookup"><span data-stu-id="64146-158">definitions</span></span>|<span data-ttu-id="64146-159">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="64146-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="64146-160">Определения групповой политики, связанные с файлом.</span><span class="sxs-lookup"><span data-stu-id="64146-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64146-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64146-161">JSON Representation</span></span>
<span data-ttu-id="64146-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64146-162">Here is a JSON representation of the resource.</span></span>
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
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



