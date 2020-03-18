---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e99b32687c0a93673cdbf8889b05e6423cc73c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783025"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="aeae1-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="aeae1-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="aeae1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeae1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeae1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aeae1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeae1-106">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="aeae1-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="aeae1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="aeae1-107">Methods</span></span>
|<span data-ttu-id="aeae1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="aeae1-108">Method</span></span>|<span data-ttu-id="aeae1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aeae1-109">Return Type</span></span>|<span data-ttu-id="aeae1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aeae1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aeae1-111">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="aeae1-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="aeae1-112">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="aeae1-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="aeae1-113">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="aeae1-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="aeae1-114">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="aeae1-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="aeae1-115">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="aeae1-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="aeae1-116">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="aeae1-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aeae1-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeae1-117">Properties</span></span>
|<span data-ttu-id="aeae1-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeae1-118">Property</span></span>|<span data-ttu-id="aeae1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aeae1-119">Type</span></span>|<span data-ttu-id="aeae1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aeae1-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeae1-121">класстипе</span><span class="sxs-lookup"><span data-stu-id="aeae1-121">classType</span></span>|[<span data-ttu-id="aeae1-122">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="aeae1-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="aeae1-123">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="aeae1-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="aeae1-124">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="aeae1-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="aeae1-125">displayName</span><span class="sxs-lookup"><span data-stu-id="aeae1-125">displayName</span></span>|<span data-ttu-id="aeae1-126">Строка</span><span class="sxs-lookup"><span data-stu-id="aeae1-126">String</span></span>|<span data-ttu-id="aeae1-127">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="aeae1-127">The localized policy name.</span></span>|
|<span data-ttu-id="aeae1-128">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="aeae1-128">explainText</span></span>|<span data-ttu-id="aeae1-129">String</span><span class="sxs-lookup"><span data-stu-id="aeae1-129">String</span></span>|<span data-ttu-id="aeae1-130">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="aeae1-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="aeae1-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="aeae1-131">The default value is empty.</span></span>|
|<span data-ttu-id="aeae1-132">категорипас</span><span class="sxs-lookup"><span data-stu-id="aeae1-132">categoryPath</span></span>|<span data-ttu-id="aeae1-133">String</span><span class="sxs-lookup"><span data-stu-id="aeae1-133">String</span></span>|<span data-ttu-id="aeae1-134">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="aeae1-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="aeae1-135">суппортедон</span><span class="sxs-lookup"><span data-stu-id="aeae1-135">supportedOn</span></span>|<span data-ttu-id="aeae1-136">String</span><span class="sxs-lookup"><span data-stu-id="aeae1-136">String</span></span>|<span data-ttu-id="aeae1-137">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="aeae1-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="aeae1-138">полицитипе</span><span class="sxs-lookup"><span data-stu-id="aeae1-138">policyType</span></span>|[<span data-ttu-id="aeae1-139">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="aeae1-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="aeae1-140">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="aeae1-140">Specifies the type of group policy.</span></span> <span data-ttu-id="aeae1-141">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="aeae1-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="aeae1-142">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="aeae1-142">groupPolicyCategoryId</span></span>|<span data-ttu-id="aeae1-143">GUID</span><span class="sxs-lookup"><span data-stu-id="aeae1-143">Guid</span></span>|<span data-ttu-id="aeae1-144">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="aeae1-144">The category id of the parent category</span></span>|
|<span data-ttu-id="aeae1-145">id</span><span class="sxs-lookup"><span data-stu-id="aeae1-145">id</span></span>|<span data-ttu-id="aeae1-146">String</span><span class="sxs-lookup"><span data-stu-id="aeae1-146">String</span></span>|<span data-ttu-id="aeae1-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aeae1-147">Key of the entity.</span></span>|
|<span data-ttu-id="aeae1-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aeae1-148">lastModifiedDateTime</span></span>|<span data-ttu-id="aeae1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeae1-149">DateTimeOffset</span></span>|<span data-ttu-id="aeae1-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aeae1-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeae1-151">Связи</span><span class="sxs-lookup"><span data-stu-id="aeae1-151">Relationships</span></span>
|<span data-ttu-id="aeae1-152">Связь</span><span class="sxs-lookup"><span data-stu-id="aeae1-152">Relationship</span></span>|<span data-ttu-id="aeae1-153">Тип</span><span class="sxs-lookup"><span data-stu-id="aeae1-153">Type</span></span>|<span data-ttu-id="aeae1-154">Описание</span><span class="sxs-lookup"><span data-stu-id="aeae1-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeae1-155">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="aeae1-155">definitionFile</span></span>|[<span data-ttu-id="aeae1-156">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="aeae1-156">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="aeae1-157">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="aeae1-157">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="aeae1-158">category</span><span class="sxs-lookup"><span data-stu-id="aeae1-158">category</span></span>|[<span data-ttu-id="aeae1-159">граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="aeae1-159">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="aeae1-160">Категория групповой политики, связанная с определением.</span><span class="sxs-lookup"><span data-stu-id="aeae1-160">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="aeae1-161">материалы</span><span class="sxs-lookup"><span data-stu-id="aeae1-161">presentations</span></span>|<span data-ttu-id="aeae1-162">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aeae1-162">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="aeae1-163">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="aeae1-163">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeae1-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aeae1-164">JSON Representation</span></span>
<span data-ttu-id="aeae1-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeae1-165">Here is a JSON representation of the resource.</span></span>
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



