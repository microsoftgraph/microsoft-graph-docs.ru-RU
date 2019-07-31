---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a68740101c79efda08f010b6e8410428c883bb2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998683"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="11323-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="11323-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="11323-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11323-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11323-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11323-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11323-106">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="11323-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="11323-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11323-107">Methods</span></span>
|<span data-ttu-id="11323-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11323-108">Method</span></span>|<span data-ttu-id="11323-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11323-109">Return Type</span></span>|<span data-ttu-id="11323-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11323-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11323-111">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="11323-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="11323-112">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="11323-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="11323-113">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="11323-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="11323-114">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="11323-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="11323-115">Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="11323-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="11323-116">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="11323-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11323-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="11323-117">Properties</span></span>
|<span data-ttu-id="11323-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="11323-118">Property</span></span>|<span data-ttu-id="11323-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11323-119">Type</span></span>|<span data-ttu-id="11323-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11323-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11323-121">Класстипе</span><span class="sxs-lookup"><span data-stu-id="11323-121">classType</span></span>|[<span data-ttu-id="11323-122">Граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="11323-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="11323-123">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="11323-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="11323-124">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="11323-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="11323-125">displayName</span><span class="sxs-lookup"><span data-stu-id="11323-125">displayName</span></span>|<span data-ttu-id="11323-126">Строка</span><span class="sxs-lookup"><span data-stu-id="11323-126">String</span></span>|<span data-ttu-id="11323-127">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="11323-127">The localized policy name.</span></span>|
|<span data-ttu-id="11323-128">Експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="11323-128">explainText</span></span>|<span data-ttu-id="11323-129">String</span><span class="sxs-lookup"><span data-stu-id="11323-129">String</span></span>|<span data-ttu-id="11323-130">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="11323-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="11323-131">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="11323-131">The default value is empty.</span></span>|
|<span data-ttu-id="11323-132">Категорипас</span><span class="sxs-lookup"><span data-stu-id="11323-132">categoryPath</span></span>|<span data-ttu-id="11323-133">String</span><span class="sxs-lookup"><span data-stu-id="11323-133">String</span></span>|<span data-ttu-id="11323-134">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="11323-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="11323-135">Суппортедон</span><span class="sxs-lookup"><span data-stu-id="11323-135">supportedOn</span></span>|<span data-ttu-id="11323-136">String</span><span class="sxs-lookup"><span data-stu-id="11323-136">String</span></span>|<span data-ttu-id="11323-137">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="11323-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="11323-138">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="11323-138">policyType</span></span>|[<span data-ttu-id="11323-139">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="11323-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="11323-140">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="11323-140">Specifies the type of group policy.</span></span> <span data-ttu-id="11323-141">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="11323-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="11323-142">id</span><span class="sxs-lookup"><span data-stu-id="11323-142">id</span></span>|<span data-ttu-id="11323-143">String</span><span class="sxs-lookup"><span data-stu-id="11323-143">String</span></span>|<span data-ttu-id="11323-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11323-144">Key of the entity.</span></span>|
|<span data-ttu-id="11323-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11323-145">lastModifiedDateTime</span></span>|<span data-ttu-id="11323-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11323-146">DateTimeOffset</span></span>|<span data-ttu-id="11323-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="11323-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11323-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="11323-148">Relationships</span></span>
|<span data-ttu-id="11323-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="11323-149">Relationship</span></span>|<span data-ttu-id="11323-150">Тип</span><span class="sxs-lookup"><span data-stu-id="11323-150">Type</span></span>|<span data-ttu-id="11323-151">Описание</span><span class="sxs-lookup"><span data-stu-id="11323-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11323-152">Дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="11323-152">definitionFile</span></span>|[<span data-ttu-id="11323-153">Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="11323-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="11323-154">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="11323-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="11323-155">материалы</span><span class="sxs-lookup"><span data-stu-id="11323-155">presentations</span></span>|<span data-ttu-id="11323-156">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="11323-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="11323-157">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="11323-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11323-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11323-158">JSON Representation</span></span>
<span data-ttu-id="11323-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11323-159">Here is a JSON representation of the resource.</span></span>
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





