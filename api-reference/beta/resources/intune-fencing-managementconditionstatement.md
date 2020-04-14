---
title: Тип ресурса Манажементкондитионстатемент
description: Оператор условия управления — это группа условий управления, которые позволяют включать и отключать конфигурации устройств и приложений при выполнении всех включенных условий управления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd52a4c78873a55c6b7635538cac11c2c5168542
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439712"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="1b4bc-103">Тип ресурса Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-103">managementConditionStatement resource type</span></span>

<span data-ttu-id="1b4bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b4bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b4bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b4bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b4bc-107">Оператор условия управления — это группа условий управления, которые позволяют включать и отключать конфигурации устройств и приложений при выполнении всех включенных условий управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="1b4bc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1b4bc-108">Methods</span></span>
|<span data-ttu-id="1b4bc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1b4bc-109">Method</span></span>|<span data-ttu-id="1b4bc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b4bc-110">Return Type</span></span>|<span data-ttu-id="1b4bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4bc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b4bc-112">Список Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="1b4bc-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="1b4bc-113">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="1b4bc-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1b4bc-114">Список свойств и связей объектов [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1b4bc-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="1b4bc-115">Получение Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="1b4bc-116">манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="1b4bc-117">Чтение свойств и связей объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1b4bc-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="1b4bc-118">Создание Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="1b4bc-119">манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="1b4bc-120">Создание нового объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1b4bc-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="1b4bc-121">Удаление Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="1b4bc-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1b4bc-122">None</span></span>|<span data-ttu-id="1b4bc-123">Удаляет объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md).</span><span class="sxs-lookup"><span data-stu-id="1b4bc-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="1b4bc-124">Обновление Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="1b4bc-125">манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="1b4bc-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="1b4bc-126">Обновление свойств объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1b4bc-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="1b4bc-127">Функция Жетманажементкондитионстатементекспрессионстринг</span><span class="sxs-lookup"><span data-stu-id="1b4bc-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="1b4bc-128">манажементкондитионекспрессионстринг</span><span class="sxs-lookup"><span data-stu-id="1b4bc-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="1b4bc-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-129">Not yet documented</span></span>|
|[<span data-ttu-id="1b4bc-130">Функция Жетманажементкондитионстатементсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="1b4bc-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="1b4bc-131">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="1b4bc-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1b4bc-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1b4bc-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1b4bc-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b4bc-133">Properties</span></span>
|<span data-ttu-id="1b4bc-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b4bc-134">Property</span></span>|<span data-ttu-id="1b4bc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4bc-135">Type</span></span>|<span data-ttu-id="1b4bc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4bc-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b4bc-137">id</span><span class="sxs-lookup"><span data-stu-id="1b4bc-137">id</span></span>|<span data-ttu-id="1b4bc-138">String</span><span class="sxs-lookup"><span data-stu-id="1b4bc-138">String</span></span>|<span data-ttu-id="1b4bc-139">Уникальный идентификатор оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="1b4bc-140">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1b4bc-141">displayName</span><span class="sxs-lookup"><span data-stu-id="1b4bc-141">displayName</span></span>|<span data-ttu-id="1b4bc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="1b4bc-142">String</span></span>|<span data-ttu-id="1b4bc-143">Имя, определенное администратором оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="1b4bc-144">description</span><span class="sxs-lookup"><span data-stu-id="1b4bc-144">description</span></span>|<span data-ttu-id="1b4bc-145">String</span><span class="sxs-lookup"><span data-stu-id="1b4bc-145">String</span></span>|<span data-ttu-id="1b4bc-146">Заданное администратором описание оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="1b4bc-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b4bc-147">createdDateTime</span></span>|<span data-ttu-id="1b4bc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b4bc-148">DateTimeOffset</span></span>|<span data-ttu-id="1b4bc-149">Время создания оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-149">The time the management condition statement was created.</span></span> <span data-ttu-id="1b4bc-150">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-150">Generated service side.</span></span>|
|<span data-ttu-id="1b4bc-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b4bc-151">modifiedDateTime</span></span>|<span data-ttu-id="1b4bc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b4bc-152">DateTimeOffset</span></span>|<span data-ttu-id="1b4bc-153">Время последнего изменения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="1b4bc-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-154">Updated service side.</span></span>|
|<span data-ttu-id="1b4bc-155">выражение</span><span class="sxs-lookup"><span data-stu-id="1b4bc-155">expression</span></span>|[<span data-ttu-id="1b4bc-156">манажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="1b4bc-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="1b4bc-157">Выражение оператора условия управления, используемое для оценки активации или деактивации оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="1b4bc-158">eTag</span><span class="sxs-lookup"><span data-stu-id="1b4bc-158">eTag</span></span>|<span data-ttu-id="1b4bc-159">String</span><span class="sxs-lookup"><span data-stu-id="1b4bc-159">String</span></span>|<span data-ttu-id="1b4bc-160">Тег ETag оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-160">ETag of the management condition statement.</span></span> <span data-ttu-id="1b4bc-161">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-161">Updated service side.</span></span>|
|<span data-ttu-id="1b4bc-162">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="1b4bc-162">applicablePlatforms</span></span>|<span data-ttu-id="1b4bc-163">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1b4bc-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1b4bc-164">Соответствующие платформы для этого оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="1b4bc-165">Это рассчитывается на основе условий управления, связанных с оператором условия управления, и поиском пересечения соответствующих платформ.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b4bc-166">Связи</span><span class="sxs-lookup"><span data-stu-id="1b4bc-166">Relationships</span></span>
|<span data-ttu-id="1b4bc-167">Связь</span><span class="sxs-lookup"><span data-stu-id="1b4bc-167">Relationship</span></span>|<span data-ttu-id="1b4bc-168">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4bc-168">Type</span></span>|<span data-ttu-id="1b4bc-169">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4bc-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b4bc-170">манажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="1b4bc-170">managementConditions</span></span>|<span data-ttu-id="1b4bc-171">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1b4bc-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1b4bc-172">Условия управления, связанные с оператором условия управления.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b4bc-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b4bc-173">JSON Representation</span></span>
<span data-ttu-id="1b4bc-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b4bc-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



