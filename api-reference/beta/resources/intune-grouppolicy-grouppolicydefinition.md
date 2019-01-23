---
title: Тип ресурса groupPolicyDefinition
description: Сущность описаны все сведения об одном групповой политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430815"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="2ea90-103">Тип ресурса groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea90-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="2ea90-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ea90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ea90-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ea90-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ea90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ea90-107">Сущность описаны все сведения об одном групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2ea90-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="2ea90-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2ea90-108">Methods</span></span>
|<span data-ttu-id="2ea90-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2ea90-109">Method</span></span>|<span data-ttu-id="2ea90-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2ea90-110">Return Type</span></span>|<span data-ttu-id="2ea90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea90-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ea90-112">Получение groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea90-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="2ea90-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea90-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="2ea90-114">Чтение свойства и связи объекта [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2ea90-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="2ea90-115">Обновление groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea90-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="2ea90-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea90-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="2ea90-117">Обновление свойства объекта [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2ea90-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ea90-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ea90-118">Properties</span></span>
|<span data-ttu-id="2ea90-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ea90-119">Property</span></span>|<span data-ttu-id="2ea90-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2ea90-120">Type</span></span>|<span data-ttu-id="2ea90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea90-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea90-122">classType</span><span class="sxs-lookup"><span data-stu-id="2ea90-122">classType</span></span>|[<span data-ttu-id="2ea90-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="2ea90-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="2ea90-124">Идентифицирует тип групп, которые могут применена политика.</span><span class="sxs-lookup"><span data-stu-id="2ea90-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="2ea90-125">Возможные значения: `user`, `machine`, `both`.</span><span class="sxs-lookup"><span data-stu-id="2ea90-125">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="2ea90-126">displayName</span><span class="sxs-lookup"><span data-stu-id="2ea90-126">displayName</span></span>|<span data-ttu-id="2ea90-127">String</span><span class="sxs-lookup"><span data-stu-id="2ea90-127">String</span></span>|<span data-ttu-id="2ea90-128">Имя политики локализованные.</span><span class="sxs-lookup"><span data-stu-id="2ea90-128">The localized policy name.</span></span>|
|<span data-ttu-id="2ea90-129">explainText</span><span class="sxs-lookup"><span data-stu-id="2ea90-129">explainText</span></span>|<span data-ttu-id="2ea90-130">String</span><span class="sxs-lookup"><span data-stu-id="2ea90-130">String</span></span>|<span data-ttu-id="2ea90-131">Локализованные объяснение или справки текст, связанного с политикой.</span><span class="sxs-lookup"><span data-stu-id="2ea90-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="2ea90-132">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="2ea90-132">The default value is empty.</span></span>|
|<span data-ttu-id="2ea90-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="2ea90-133">categoryPath</span></span>|<span data-ttu-id="2ea90-134">String</span><span class="sxs-lookup"><span data-stu-id="2ea90-134">String</span></span>|<span data-ttu-id="2ea90-135">Локализованные категории полный путь для политики.</span><span class="sxs-lookup"><span data-stu-id="2ea90-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="2ea90-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="2ea90-136">supportedOn</span></span>|<span data-ttu-id="2ea90-137">String</span><span class="sxs-lookup"><span data-stu-id="2ea90-137">String</span></span>|<span data-ttu-id="2ea90-138">Локализованные строки, используется, чтобы указать, какие приложения версия операционной системы или определяется политики.</span><span class="sxs-lookup"><span data-stu-id="2ea90-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="2ea90-139">policyType</span><span class="sxs-lookup"><span data-stu-id="2ea90-139">policyType</span></span>|[<span data-ttu-id="2ea90-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="2ea90-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2ea90-141">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2ea90-141">Specifies the type of group policy.</span></span> <span data-ttu-id="2ea90-142">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2ea90-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2ea90-143">id</span><span class="sxs-lookup"><span data-stu-id="2ea90-143">id</span></span>|<span data-ttu-id="2ea90-144">String</span><span class="sxs-lookup"><span data-stu-id="2ea90-144">String</span></span>|<span data-ttu-id="2ea90-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ea90-145">Key of the entity.</span></span>|
|<span data-ttu-id="2ea90-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ea90-146">lastModifiedDateTime</span></span>|<span data-ttu-id="2ea90-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ea90-147">DateTimeOffset</span></span>|<span data-ttu-id="2ea90-148">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2ea90-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ea90-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ea90-149">Relationships</span></span>
|<span data-ttu-id="2ea90-150">Связь</span><span class="sxs-lookup"><span data-stu-id="2ea90-150">Relationship</span></span>|<span data-ttu-id="2ea90-151">Тип</span><span class="sxs-lookup"><span data-stu-id="2ea90-151">Type</span></span>|<span data-ttu-id="2ea90-152">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea90-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea90-153">definitionFile</span><span class="sxs-lookup"><span data-stu-id="2ea90-153">definitionFile</span></span>|[<span data-ttu-id="2ea90-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="2ea90-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="2ea90-155">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="2ea90-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="2ea90-156">презентации</span><span class="sxs-lookup"><span data-stu-id="2ea90-156">presentations</span></span>|<span data-ttu-id="2ea90-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2ea90-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="2ea90-158">Презентаций групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="2ea90-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ea90-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ea90-159">JSON Representation</span></span>
<span data-ttu-id="2ea90-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ea90-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




