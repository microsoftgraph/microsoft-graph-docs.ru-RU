---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89db03a54e2bbed52a4bc24266136cf9af272215
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259762"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="34c1a-105">Тип ресурса Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="34c1a-105">groupPolicyDefinitionFile resource type</span></span>

<span data-ttu-id="34c1a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34c1a-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34c1a-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34c1a-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34c1a-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34c1a-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34c1a-109">Сущность представляет XML-файл ADMX (административный шаблон).</span><span class="sxs-lookup"><span data-stu-id="34c1a-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="34c1a-110">ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории.</span><span class="sxs-lookup"><span data-stu-id="34c1a-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="34c1a-111">В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).</span><span class="sxs-lookup"><span data-stu-id="34c1a-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="34c1a-112">Методы</span><span class="sxs-lookup"><span data-stu-id="34c1a-112">Methods</span></span>
|<span data-ttu-id="34c1a-113">Метод</span><span class="sxs-lookup"><span data-stu-id="34c1a-113">Method</span></span>|<span data-ttu-id="34c1a-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34c1a-114">Return Type</span></span>|<span data-ttu-id="34c1a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="34c1a-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34c1a-116">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="34c1a-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="34c1a-117">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="34c1a-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="34c1a-118">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="34c1a-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="34c1a-119">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="34c1a-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="34c1a-120">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="34c1a-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="34c1a-121">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="34c1a-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34c1a-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="34c1a-122">Properties</span></span>
|<span data-ttu-id="34c1a-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="34c1a-123">Property</span></span>|<span data-ttu-id="34c1a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="34c1a-124">Type</span></span>|<span data-ttu-id="34c1a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="34c1a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c1a-126">displayName</span><span class="sxs-lookup"><span data-stu-id="34c1a-126">displayName</span></span>|<span data-ttu-id="34c1a-127">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-127">String</span></span>|<span data-ttu-id="34c1a-128">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="34c1a-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="34c1a-129">description</span><span class="sxs-lookup"><span data-stu-id="34c1a-129">description</span></span>|<span data-ttu-id="34c1a-130">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-130">String</span></span>|<span data-ttu-id="34c1a-131">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="34c1a-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="34c1a-132">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="34c1a-132">The default value is empty.</span></span>|
|<span data-ttu-id="34c1a-133">лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="34c1a-133">languageCodes</span></span>|<span data-ttu-id="34c1a-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="34c1a-134">String collection</span></span>|<span data-ttu-id="34c1a-135">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="34c1a-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="34c1a-136">таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="34c1a-136">targetPrefix</span></span>|<span data-ttu-id="34c1a-137">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-137">String</span></span>|<span data-ttu-id="34c1a-138">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="34c1a-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="34c1a-139">Атрибут</span><span class="sxs-lookup"><span data-stu-id="34c1a-139">targetNamespace</span></span>|<span data-ttu-id="34c1a-140">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-140">String</span></span>|<span data-ttu-id="34c1a-141">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="34c1a-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="34c1a-142">полицитипе</span><span class="sxs-lookup"><span data-stu-id="34c1a-142">policyType</span></span>|[<span data-ttu-id="34c1a-143">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="34c1a-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="34c1a-144">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="34c1a-144">Specifies the type of group policy.</span></span> <span data-ttu-id="34c1a-145">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="34c1a-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="34c1a-146">последним</span><span class="sxs-lookup"><span data-stu-id="34c1a-146">revision</span></span>|<span data-ttu-id="34c1a-147">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-147">String</span></span>|<span data-ttu-id="34c1a-148">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="34c1a-148">The revision version associated with the file.</span></span>|
|<span data-ttu-id="34c1a-149">id</span><span class="sxs-lookup"><span data-stu-id="34c1a-149">id</span></span>|<span data-ttu-id="34c1a-150">String</span><span class="sxs-lookup"><span data-stu-id="34c1a-150">String</span></span>|<span data-ttu-id="34c1a-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34c1a-151">Key of the entity.</span></span>|
|<span data-ttu-id="34c1a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34c1a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="34c1a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c1a-153">DateTimeOffset</span></span>|<span data-ttu-id="34c1a-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="34c1a-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34c1a-155">Связи</span><span class="sxs-lookup"><span data-stu-id="34c1a-155">Relationships</span></span>
|<span data-ttu-id="34c1a-156">Связь</span><span class="sxs-lookup"><span data-stu-id="34c1a-156">Relationship</span></span>|<span data-ttu-id="34c1a-157">Тип</span><span class="sxs-lookup"><span data-stu-id="34c1a-157">Type</span></span>|<span data-ttu-id="34c1a-158">Описание</span><span class="sxs-lookup"><span data-stu-id="34c1a-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c1a-159">определения</span><span class="sxs-lookup"><span data-stu-id="34c1a-159">definitions</span></span>|<span data-ttu-id="34c1a-160">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="34c1a-160">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="34c1a-161">Определения групповой политики, связанные с файлом.</span><span class="sxs-lookup"><span data-stu-id="34c1a-161">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34c1a-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34c1a-162">JSON Representation</span></span>
<span data-ttu-id="34c1a-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34c1a-163">Here is a JSON representation of the resource.</span></span>
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




