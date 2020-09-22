---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9ba5a4c415b0bc94b60479530ac6a7ca35f3c75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031013"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="1f852-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="1f852-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="1f852-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f852-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f852-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f852-107">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="1f852-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="1f852-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1f852-108">Methods</span></span>
|<span data-ttu-id="1f852-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1f852-109">Method</span></span>|<span data-ttu-id="1f852-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f852-110">Return Type</span></span>|<span data-ttu-id="1f852-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f852-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f852-112">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="1f852-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="1f852-113">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="1f852-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="1f852-114">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="1f852-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="1f852-115">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="1f852-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="1f852-116">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="1f852-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="1f852-117">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="1f852-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f852-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f852-118">Properties</span></span>
|<span data-ttu-id="1f852-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f852-119">Property</span></span>|<span data-ttu-id="1f852-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1f852-120">Type</span></span>|<span data-ttu-id="1f852-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1f852-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f852-122">класстипе</span><span class="sxs-lookup"><span data-stu-id="1f852-122">classType</span></span>|[<span data-ttu-id="1f852-123">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="1f852-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="1f852-124">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="1f852-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="1f852-125">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="1f852-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="1f852-126">displayName</span><span class="sxs-lookup"><span data-stu-id="1f852-126">displayName</span></span>|<span data-ttu-id="1f852-127">String</span><span class="sxs-lookup"><span data-stu-id="1f852-127">String</span></span>|<span data-ttu-id="1f852-128">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="1f852-128">The localized policy name.</span></span>|
|<span data-ttu-id="1f852-129">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="1f852-129">explainText</span></span>|<span data-ttu-id="1f852-130">String</span><span class="sxs-lookup"><span data-stu-id="1f852-130">String</span></span>|<span data-ttu-id="1f852-131">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="1f852-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="1f852-132">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="1f852-132">The default value is empty.</span></span>|
|<span data-ttu-id="1f852-133">категорипас</span><span class="sxs-lookup"><span data-stu-id="1f852-133">categoryPath</span></span>|<span data-ttu-id="1f852-134">String</span><span class="sxs-lookup"><span data-stu-id="1f852-134">String</span></span>|<span data-ttu-id="1f852-135">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="1f852-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="1f852-136">суппортедон</span><span class="sxs-lookup"><span data-stu-id="1f852-136">supportedOn</span></span>|<span data-ttu-id="1f852-137">String</span><span class="sxs-lookup"><span data-stu-id="1f852-137">String</span></span>|<span data-ttu-id="1f852-138">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="1f852-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="1f852-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="1f852-139">policyType</span></span>|[<span data-ttu-id="1f852-140">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="1f852-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="1f852-141">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1f852-141">Specifies the type of group policy.</span></span> <span data-ttu-id="1f852-142">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="1f852-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="1f852-143">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="1f852-143">groupPolicyCategoryId</span></span>|<span data-ttu-id="1f852-144">Guid</span><span class="sxs-lookup"><span data-stu-id="1f852-144">Guid</span></span>|<span data-ttu-id="1f852-145">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="1f852-145">The category id of the parent category</span></span>|
|<span data-ttu-id="1f852-146">id</span><span class="sxs-lookup"><span data-stu-id="1f852-146">id</span></span>|<span data-ttu-id="1f852-147">String</span><span class="sxs-lookup"><span data-stu-id="1f852-147">String</span></span>|<span data-ttu-id="1f852-148">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f852-148">Key of the entity.</span></span>|
|<span data-ttu-id="1f852-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f852-149">lastModifiedDateTime</span></span>|<span data-ttu-id="1f852-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f852-150">DateTimeOffset</span></span>|<span data-ttu-id="1f852-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1f852-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f852-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f852-152">Relationships</span></span>
|<span data-ttu-id="1f852-153">Связь</span><span class="sxs-lookup"><span data-stu-id="1f852-153">Relationship</span></span>|<span data-ttu-id="1f852-154">Тип</span><span class="sxs-lookup"><span data-stu-id="1f852-154">Type</span></span>|<span data-ttu-id="1f852-155">Описание</span><span class="sxs-lookup"><span data-stu-id="1f852-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f852-156">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="1f852-156">definitionFile</span></span>|[<span data-ttu-id="1f852-157">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="1f852-157">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="1f852-158">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="1f852-158">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="1f852-159">category</span><span class="sxs-lookup"><span data-stu-id="1f852-159">category</span></span>|[<span data-ttu-id="1f852-160">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="1f852-160">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="1f852-161">Категория групповой политики, связанная с определением.</span><span class="sxs-lookup"><span data-stu-id="1f852-161">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="1f852-162">материалы</span><span class="sxs-lookup"><span data-stu-id="1f852-162">presentations</span></span>|<span data-ttu-id="1f852-163">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1f852-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="1f852-164">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="1f852-164">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f852-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f852-165">JSON Representation</span></span>
<span data-ttu-id="1f852-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f852-166">Here is a JSON representation of the resource.</span></span>
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
  "groupPolicyCategoryId": "Guid",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






