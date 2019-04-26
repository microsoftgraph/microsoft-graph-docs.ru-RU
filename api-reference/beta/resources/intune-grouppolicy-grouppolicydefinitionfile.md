---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ecccc683187b592c422d26a6f41bfd15b9d805b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575998"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="61233-105">Тип ресурса Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="61233-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="61233-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61233-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61233-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61233-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61233-108">Сущность представляет XML-файл ADMX (административный шаблон).</span><span class="sxs-lookup"><span data-stu-id="61233-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="61233-109">ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории.</span><span class="sxs-lookup"><span data-stu-id="61233-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="61233-110">В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).</span><span class="sxs-lookup"><span data-stu-id="61233-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="61233-111">Методы</span><span class="sxs-lookup"><span data-stu-id="61233-111">Methods</span></span>
|<span data-ttu-id="61233-112">Метод</span><span class="sxs-lookup"><span data-stu-id="61233-112">Method</span></span>|<span data-ttu-id="61233-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61233-113">Return Type</span></span>|<span data-ttu-id="61233-114">Описание</span><span class="sxs-lookup"><span data-stu-id="61233-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61233-115">Получение Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="61233-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="61233-116">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="61233-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="61233-117">Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="61233-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="61233-118">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="61233-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="61233-119">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="61233-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="61233-120">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="61233-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="61233-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="61233-121">Properties</span></span>
|<span data-ttu-id="61233-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="61233-122">Property</span></span>|<span data-ttu-id="61233-123">Тип</span><span class="sxs-lookup"><span data-stu-id="61233-123">Type</span></span>|<span data-ttu-id="61233-124">Описание</span><span class="sxs-lookup"><span data-stu-id="61233-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61233-125">displayName</span><span class="sxs-lookup"><span data-stu-id="61233-125">displayName</span></span>|<span data-ttu-id="61233-126">String</span><span class="sxs-lookup"><span data-stu-id="61233-126">String</span></span>|<span data-ttu-id="61233-127">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="61233-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="61233-128">description</span><span class="sxs-lookup"><span data-stu-id="61233-128">description</span></span>|<span data-ttu-id="61233-129">String</span><span class="sxs-lookup"><span data-stu-id="61233-129">String</span></span>|<span data-ttu-id="61233-130">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="61233-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="61233-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="61233-131">The default value is empty.</span></span>|
|<span data-ttu-id="61233-132">Лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="61233-132">languageCodes</span></span>|<span data-ttu-id="61233-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61233-133">String collection</span></span>|<span data-ttu-id="61233-134">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="61233-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="61233-135">Таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="61233-135">targetPrefix</span></span>|<span data-ttu-id="61233-136">String</span><span class="sxs-lookup"><span data-stu-id="61233-136">String</span></span>|<span data-ttu-id="61233-137">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="61233-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="61233-138">Атрибут</span><span class="sxs-lookup"><span data-stu-id="61233-138">targetNamespace</span></span>|<span data-ttu-id="61233-139">String</span><span class="sxs-lookup"><span data-stu-id="61233-139">String</span></span>|<span data-ttu-id="61233-140">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="61233-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="61233-141">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="61233-141">policyType</span></span>|[<span data-ttu-id="61233-142">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="61233-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="61233-143">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="61233-143">Specifies the type of group policy.</span></span> <span data-ttu-id="61233-144">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="61233-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="61233-145">id</span><span class="sxs-lookup"><span data-stu-id="61233-145">id</span></span>|<span data-ttu-id="61233-146">Строка</span><span class="sxs-lookup"><span data-stu-id="61233-146">String</span></span>|<span data-ttu-id="61233-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="61233-147">Key of the entity.</span></span>|
|<span data-ttu-id="61233-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61233-148">lastModifiedDateTime</span></span>|<span data-ttu-id="61233-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61233-149">DateTimeOffset</span></span>|<span data-ttu-id="61233-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="61233-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61233-151">Связи</span><span class="sxs-lookup"><span data-stu-id="61233-151">Relationships</span></span>
|<span data-ttu-id="61233-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="61233-152">Relationship</span></span>|<span data-ttu-id="61233-153">Тип</span><span class="sxs-lookup"><span data-stu-id="61233-153">Type</span></span>|<span data-ttu-id="61233-154">Описание</span><span class="sxs-lookup"><span data-stu-id="61233-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61233-155">определения</span><span class="sxs-lookup"><span data-stu-id="61233-155">definitions</span></span>|<span data-ttu-id="61233-156">Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="61233-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="61233-157">Определения групповой политики, связанные с файлом.</span><span class="sxs-lookup"><span data-stu-id="61233-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61233-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61233-158">JSON Representation</span></span>
<span data-ttu-id="61233-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61233-159">Here is a JSON representation of the resource.</span></span>
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





