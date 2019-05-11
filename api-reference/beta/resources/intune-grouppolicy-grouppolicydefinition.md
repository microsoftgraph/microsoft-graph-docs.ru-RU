---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17fef49d7d08f94f5ebafd02636d9536a05b87f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941172"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="af2d7-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="af2d7-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="af2d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af2d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af2d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af2d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af2d7-106">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="af2d7-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="af2d7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="af2d7-107">Methods</span></span>
|<span data-ttu-id="af2d7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="af2d7-108">Method</span></span>|<span data-ttu-id="af2d7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af2d7-109">Return Type</span></span>|<span data-ttu-id="af2d7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af2d7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af2d7-111">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="af2d7-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="af2d7-112">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="af2d7-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="af2d7-113">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="af2d7-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="af2d7-114">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="af2d7-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="af2d7-115">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="af2d7-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="af2d7-116">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="af2d7-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af2d7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="af2d7-117">Properties</span></span>
|<span data-ttu-id="af2d7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="af2d7-118">Property</span></span>|<span data-ttu-id="af2d7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="af2d7-119">Type</span></span>|<span data-ttu-id="af2d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="af2d7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2d7-121">Класстипе</span><span class="sxs-lookup"><span data-stu-id="af2d7-121">classType</span></span>|[<span data-ttu-id="af2d7-122">Граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="af2d7-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="af2d7-123">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="af2d7-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="af2d7-124">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="af2d7-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="af2d7-125">displayName</span><span class="sxs-lookup"><span data-stu-id="af2d7-125">displayName</span></span>|<span data-ttu-id="af2d7-126">Строка</span><span class="sxs-lookup"><span data-stu-id="af2d7-126">String</span></span>|<span data-ttu-id="af2d7-127">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="af2d7-127">The localized policy name.</span></span>|
|<span data-ttu-id="af2d7-128">Експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="af2d7-128">explainText</span></span>|<span data-ttu-id="af2d7-129">Строка</span><span class="sxs-lookup"><span data-stu-id="af2d7-129">String</span></span>|<span data-ttu-id="af2d7-130">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="af2d7-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="af2d7-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="af2d7-131">The default value is empty.</span></span>|
|<span data-ttu-id="af2d7-132">Категорипас</span><span class="sxs-lookup"><span data-stu-id="af2d7-132">categoryPath</span></span>|<span data-ttu-id="af2d7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="af2d7-133">String</span></span>|<span data-ttu-id="af2d7-134">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="af2d7-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="af2d7-135">Суппортедон</span><span class="sxs-lookup"><span data-stu-id="af2d7-135">supportedOn</span></span>|<span data-ttu-id="af2d7-136">Строка</span><span class="sxs-lookup"><span data-stu-id="af2d7-136">String</span></span>|<span data-ttu-id="af2d7-137">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="af2d7-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="af2d7-138">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="af2d7-138">policyType</span></span>|[<span data-ttu-id="af2d7-139">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="af2d7-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="af2d7-140">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="af2d7-140">Specifies the type of group policy.</span></span> <span data-ttu-id="af2d7-141">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="af2d7-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="af2d7-142">id</span><span class="sxs-lookup"><span data-stu-id="af2d7-142">id</span></span>|<span data-ttu-id="af2d7-143">String</span><span class="sxs-lookup"><span data-stu-id="af2d7-143">String</span></span>|<span data-ttu-id="af2d7-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af2d7-144">Key of the entity.</span></span>|
|<span data-ttu-id="af2d7-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af2d7-145">lastModifiedDateTime</span></span>|<span data-ttu-id="af2d7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2d7-146">DateTimeOffset</span></span>|<span data-ttu-id="af2d7-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="af2d7-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2d7-148">Связи</span><span class="sxs-lookup"><span data-stu-id="af2d7-148">Relationships</span></span>
|<span data-ttu-id="af2d7-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="af2d7-149">Relationship</span></span>|<span data-ttu-id="af2d7-150">Тип</span><span class="sxs-lookup"><span data-stu-id="af2d7-150">Type</span></span>|<span data-ttu-id="af2d7-151">Описание</span><span class="sxs-lookup"><span data-stu-id="af2d7-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2d7-152">Дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="af2d7-152">definitionFile</span></span>|[<span data-ttu-id="af2d7-153">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="af2d7-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="af2d7-154">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="af2d7-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="af2d7-155">материалы</span><span class="sxs-lookup"><span data-stu-id="af2d7-155">presentations</span></span>|<span data-ttu-id="af2d7-156">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="af2d7-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="af2d7-157">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="af2d7-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af2d7-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af2d7-158">JSON Representation</span></span>
<span data-ttu-id="af2d7-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af2d7-159">Here is a JSON representation of the resource.</span></span>
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




