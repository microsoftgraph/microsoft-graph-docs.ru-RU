---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b7a2317927e9c486d105df01cd78001de7a0c66
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298556"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="8f992-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="8f992-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="8f992-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f992-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f992-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f992-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f992-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f992-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f992-107">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="8f992-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="8f992-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8f992-108">Methods</span></span>
|<span data-ttu-id="8f992-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8f992-109">Method</span></span>|<span data-ttu-id="8f992-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f992-110">Return Type</span></span>|<span data-ttu-id="8f992-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f992-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f992-112">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="8f992-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="8f992-113">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="8f992-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="8f992-114">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8f992-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="8f992-115">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="8f992-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="8f992-116">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="8f992-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="8f992-117">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8f992-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f992-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f992-118">Properties</span></span>
|<span data-ttu-id="8f992-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f992-119">Property</span></span>|<span data-ttu-id="8f992-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8f992-120">Type</span></span>|<span data-ttu-id="8f992-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8f992-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f992-122">класстипе</span><span class="sxs-lookup"><span data-stu-id="8f992-122">classType</span></span>|[<span data-ttu-id="8f992-123">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="8f992-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="8f992-124">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="8f992-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="8f992-125">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="8f992-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8f992-126">displayName</span><span class="sxs-lookup"><span data-stu-id="8f992-126">displayName</span></span>|<span data-ttu-id="8f992-127">String</span><span class="sxs-lookup"><span data-stu-id="8f992-127">String</span></span>|<span data-ttu-id="8f992-128">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="8f992-128">The localized policy name.</span></span>|
|<span data-ttu-id="8f992-129">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="8f992-129">explainText</span></span>|<span data-ttu-id="8f992-130">String</span><span class="sxs-lookup"><span data-stu-id="8f992-130">String</span></span>|<span data-ttu-id="8f992-131">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="8f992-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="8f992-132">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="8f992-132">The default value is empty.</span></span>|
|<span data-ttu-id="8f992-133">категорипас</span><span class="sxs-lookup"><span data-stu-id="8f992-133">categoryPath</span></span>|<span data-ttu-id="8f992-134">String</span><span class="sxs-lookup"><span data-stu-id="8f992-134">String</span></span>|<span data-ttu-id="8f992-135">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="8f992-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="8f992-136">суппортедон</span><span class="sxs-lookup"><span data-stu-id="8f992-136">supportedOn</span></span>|<span data-ttu-id="8f992-137">String</span><span class="sxs-lookup"><span data-stu-id="8f992-137">String</span></span>|<span data-ttu-id="8f992-138">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="8f992-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="8f992-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="8f992-139">policyType</span></span>|[<span data-ttu-id="8f992-140">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="8f992-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="8f992-141">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8f992-141">Specifies the type of group policy.</span></span> <span data-ttu-id="8f992-142">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="8f992-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="8f992-143">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="8f992-143">groupPolicyCategoryId</span></span>|<span data-ttu-id="8f992-144">Guid</span><span class="sxs-lookup"><span data-stu-id="8f992-144">Guid</span></span>|<span data-ttu-id="8f992-145">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="8f992-145">The category id of the parent category</span></span>|
|<span data-ttu-id="8f992-146">id</span><span class="sxs-lookup"><span data-stu-id="8f992-146">id</span></span>|<span data-ttu-id="8f992-147">String</span><span class="sxs-lookup"><span data-stu-id="8f992-147">String</span></span>|<span data-ttu-id="8f992-148">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f992-148">Key of the entity.</span></span>|
|<span data-ttu-id="8f992-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f992-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8f992-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f992-150">DateTimeOffset</span></span>|<span data-ttu-id="8f992-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8f992-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f992-152">Связи</span><span class="sxs-lookup"><span data-stu-id="8f992-152">Relationships</span></span>
|<span data-ttu-id="8f992-153">Связь</span><span class="sxs-lookup"><span data-stu-id="8f992-153">Relationship</span></span>|<span data-ttu-id="8f992-154">Тип</span><span class="sxs-lookup"><span data-stu-id="8f992-154">Type</span></span>|<span data-ttu-id="8f992-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8f992-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f992-156">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="8f992-156">definitionFile</span></span>|[<span data-ttu-id="8f992-157">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="8f992-157">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="8f992-158">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="8f992-158">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="8f992-159">category</span><span class="sxs-lookup"><span data-stu-id="8f992-159">category</span></span>|[<span data-ttu-id="8f992-160">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="8f992-160">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="8f992-161">Категория групповой политики, связанная с определением.</span><span class="sxs-lookup"><span data-stu-id="8f992-161">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="8f992-162">материалы</span><span class="sxs-lookup"><span data-stu-id="8f992-162">presentations</span></span>|<span data-ttu-id="8f992-163">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8f992-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="8f992-164">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="8f992-164">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f992-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f992-165">JSON Representation</span></span>
<span data-ttu-id="8f992-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f992-166">Here is a JSON representation of the resource.</span></span>
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




