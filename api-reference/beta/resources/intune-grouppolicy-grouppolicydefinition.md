---
title: Тип ресурса Граупполицидефинитион
description: Сущность описывает все сведения об одной групповой политике.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 038647f4e40036db89ecf61cdece531662658c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528091"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="286e5-103">Тип ресурса Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="286e5-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="286e5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="286e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="286e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="286e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="286e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="286e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="286e5-107">Сущность описывает все сведения об одной групповой политике.</span><span class="sxs-lookup"><span data-stu-id="286e5-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="286e5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="286e5-108">Methods</span></span>
|<span data-ttu-id="286e5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="286e5-109">Method</span></span>|<span data-ttu-id="286e5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="286e5-110">Return Type</span></span>|<span data-ttu-id="286e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="286e5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="286e5-112">Получение Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="286e5-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="286e5-113">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="286e5-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="286e5-114">Чтение свойств и связей объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="286e5-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="286e5-115">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="286e5-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="286e5-116">граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="286e5-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="286e5-117">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="286e5-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="286e5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="286e5-118">Properties</span></span>
|<span data-ttu-id="286e5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="286e5-119">Property</span></span>|<span data-ttu-id="286e5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="286e5-120">Type</span></span>|<span data-ttu-id="286e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="286e5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="286e5-122">класстипе</span><span class="sxs-lookup"><span data-stu-id="286e5-122">classType</span></span>|[<span data-ttu-id="286e5-123">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="286e5-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="286e5-124">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="286e5-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="286e5-125">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="286e5-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="286e5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="286e5-126">displayName</span></span>|<span data-ttu-id="286e5-127">Строка</span><span class="sxs-lookup"><span data-stu-id="286e5-127">String</span></span>|<span data-ttu-id="286e5-128">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="286e5-128">The localized policy name.</span></span>|
|<span data-ttu-id="286e5-129">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="286e5-129">explainText</span></span>|<span data-ttu-id="286e5-130">String</span><span class="sxs-lookup"><span data-stu-id="286e5-130">String</span></span>|<span data-ttu-id="286e5-131">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="286e5-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="286e5-132">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="286e5-132">The default value is empty.</span></span>|
|<span data-ttu-id="286e5-133">категорипас</span><span class="sxs-lookup"><span data-stu-id="286e5-133">categoryPath</span></span>|<span data-ttu-id="286e5-134">String</span><span class="sxs-lookup"><span data-stu-id="286e5-134">String</span></span>|<span data-ttu-id="286e5-135">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="286e5-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="286e5-136">суппортедон</span><span class="sxs-lookup"><span data-stu-id="286e5-136">supportedOn</span></span>|<span data-ttu-id="286e5-137">String</span><span class="sxs-lookup"><span data-stu-id="286e5-137">String</span></span>|<span data-ttu-id="286e5-138">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="286e5-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="286e5-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="286e5-139">policyType</span></span>|[<span data-ttu-id="286e5-140">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="286e5-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="286e5-141">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="286e5-141">Specifies the type of group policy.</span></span> <span data-ttu-id="286e5-142">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="286e5-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="286e5-143">id</span><span class="sxs-lookup"><span data-stu-id="286e5-143">id</span></span>|<span data-ttu-id="286e5-144">String</span><span class="sxs-lookup"><span data-stu-id="286e5-144">String</span></span>|<span data-ttu-id="286e5-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="286e5-145">Key of the entity.</span></span>|
|<span data-ttu-id="286e5-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="286e5-146">lastModifiedDateTime</span></span>|<span data-ttu-id="286e5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="286e5-147">DateTimeOffset</span></span>|<span data-ttu-id="286e5-148">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="286e5-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="286e5-149">Связи</span><span class="sxs-lookup"><span data-stu-id="286e5-149">Relationships</span></span>
|<span data-ttu-id="286e5-150">Связь</span><span class="sxs-lookup"><span data-stu-id="286e5-150">Relationship</span></span>|<span data-ttu-id="286e5-151">Тип</span><span class="sxs-lookup"><span data-stu-id="286e5-151">Type</span></span>|<span data-ttu-id="286e5-152">Описание</span><span class="sxs-lookup"><span data-stu-id="286e5-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="286e5-153">дефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="286e5-153">definitionFile</span></span>|[<span data-ttu-id="286e5-154">граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="286e5-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="286e5-155">Файл групповой политики, связанный с определением.</span><span class="sxs-lookup"><span data-stu-id="286e5-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="286e5-156">материалы</span><span class="sxs-lookup"><span data-stu-id="286e5-156">presentations</span></span>|<span data-ttu-id="286e5-157">Коллекция [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="286e5-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="286e5-158">Презентации групповой политики, связанные с определением.</span><span class="sxs-lookup"><span data-stu-id="286e5-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="286e5-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="286e5-159">JSON Representation</span></span>
<span data-ttu-id="286e5-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="286e5-160">Here is a JSON representation of the resource.</span></span>
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



