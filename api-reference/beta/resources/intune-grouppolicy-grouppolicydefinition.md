---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bea1b7bda5532cbb310930bcb65759b0f125d384
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697373"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="9255b-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9255b-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="9255b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9255b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9255b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9255b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9255b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9255b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9255b-107">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="9255b-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9255b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9255b-108">Methods</span></span>
|<span data-ttu-id="9255b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9255b-109">Method</span></span>|<span data-ttu-id="9255b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9255b-110">Return Type</span></span>|<span data-ttu-id="9255b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9255b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9255b-112">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9255b-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="9255b-113">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9255b-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9255b-114">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9255b-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="9255b-115">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9255b-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="9255b-116">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="9255b-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9255b-117">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9255b-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9255b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9255b-118">Properties</span></span>
|<span data-ttu-id="9255b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9255b-119">Property</span></span>|<span data-ttu-id="9255b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9255b-120">Type</span></span>|<span data-ttu-id="9255b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9255b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9255b-122">класстипе</span><span class="sxs-lookup"><span data-stu-id="9255b-122">classType</span></span>|[<span data-ttu-id="9255b-123">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="9255b-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="9255b-124">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="9255b-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="9255b-125">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="9255b-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9255b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9255b-126">displayName</span></span>|<span data-ttu-id="9255b-127">Строка</span><span class="sxs-lookup"><span data-stu-id="9255b-127">String</span></span>|<span data-ttu-id="9255b-128">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="9255b-128">The localized policy name.</span></span>|
|<span data-ttu-id="9255b-129">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="9255b-129">explainText</span></span>|<span data-ttu-id="9255b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9255b-130">String</span></span>|<span data-ttu-id="9255b-131">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="9255b-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="9255b-132">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="9255b-132">The default value is empty.</span></span>|
|<span data-ttu-id="9255b-133">категорипас</span><span class="sxs-lookup"><span data-stu-id="9255b-133">categoryPath</span></span>|<span data-ttu-id="9255b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9255b-134">String</span></span>|<span data-ttu-id="9255b-135">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="9255b-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="9255b-136">суппортедон</span><span class="sxs-lookup"><span data-stu-id="9255b-136">supportedOn</span></span>|<span data-ttu-id="9255b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9255b-137">String</span></span>|<span data-ttu-id="9255b-138">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="9255b-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="9255b-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="9255b-139">policyType</span></span>|[<span data-ttu-id="9255b-140">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="9255b-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9255b-141">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9255b-141">Specifies the type of group policy.</span></span> <span data-ttu-id="9255b-142">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="9255b-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9255b-143">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="9255b-143">groupPolicyCategoryId</span></span>|<span data-ttu-id="9255b-144">Guid</span><span class="sxs-lookup"><span data-stu-id="9255b-144">Guid</span></span>|<span data-ttu-id="9255b-145">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="9255b-145">The category id of the parent category</span></span>|
|<span data-ttu-id="9255b-146">id</span><span class="sxs-lookup"><span data-stu-id="9255b-146">id</span></span>|<span data-ttu-id="9255b-147">Строка</span><span class="sxs-lookup"><span data-stu-id="9255b-147">String</span></span>|<span data-ttu-id="9255b-148">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9255b-148">Key of the entity.</span></span>|
|<span data-ttu-id="9255b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9255b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9255b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9255b-150">DateTimeOffset</span></span>|<span data-ttu-id="9255b-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9255b-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9255b-152">Связи</span><span class="sxs-lookup"><span data-stu-id="9255b-152">Relationships</span></span>
|<span data-ttu-id="9255b-153">Связь</span><span class="sxs-lookup"><span data-stu-id="9255b-153">Relationship</span></span>|<span data-ttu-id="9255b-154">Тип</span><span class="sxs-lookup"><span data-stu-id="9255b-154">Type</span></span>|<span data-ttu-id="9255b-155">Описание</span><span class="sxs-lookup"><span data-stu-id="9255b-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9255b-156">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="9255b-156">definitionFile</span></span>|[<span data-ttu-id="9255b-157">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="9255b-157">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9255b-158">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="9255b-158">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="9255b-159">category</span><span class="sxs-lookup"><span data-stu-id="9255b-159">category</span></span>|[<span data-ttu-id="9255b-160">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="9255b-160">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="9255b-161">Категория групповой политики, связанная с определением.</span><span class="sxs-lookup"><span data-stu-id="9255b-161">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="9255b-162">материалы</span><span class="sxs-lookup"><span data-stu-id="9255b-162">presentations</span></span>|<span data-ttu-id="9255b-163">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9255b-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="9255b-164">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="9255b-164">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9255b-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9255b-165">JSON Representation</span></span>
<span data-ttu-id="9255b-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9255b-166">Here is a JSON representation of the resource.</span></span>
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





