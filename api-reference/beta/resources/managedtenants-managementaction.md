---
title: тип ресурса managementAction
description: Представляет базовое действие управления для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403169"
---
# <a name="managementaction-resource-type"></a><span data-ttu-id="583cb-103">тип ресурса managementAction</span><span class="sxs-lookup"><span data-stu-id="583cb-103">managementAction resource type</span></span>

<span data-ttu-id="583cb-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="583cb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="583cb-105">Представляет базовое действие управления для данного управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="583cb-105">Represents a baseline management action for a given managed tenant.</span></span> <span data-ttu-id="583cb-106">Примерами действий управления являются шифрование устройств, выполнение конфигураций для Azure Active Directory регистрации устройства и многофакторная проверка подлинности для администраторов.</span><span class="sxs-lookup"><span data-stu-id="583cb-106">Examples of management actions are device encryption, perform configurations to allow Azure Active Directory device enrollment, and require multi-factor authentication for admins.</span></span>

## <a name="methods"></a><span data-ttu-id="583cb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="583cb-107">Methods</span></span>
|<span data-ttu-id="583cb-108">Метод</span><span class="sxs-lookup"><span data-stu-id="583cb-108">Method</span></span>|<span data-ttu-id="583cb-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="583cb-109">Return type</span></span>|<span data-ttu-id="583cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="583cb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="583cb-111">Управление спискамиActions</span><span class="sxs-lookup"><span data-stu-id="583cb-111">List managementActions</span></span>](../api/managedtenants-managedtenant-list-managementactions.md)|<span data-ttu-id="583cb-112">[коллекция microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="583cb-112">[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) collection</span></span>|<span data-ttu-id="583cb-113">Получите список объектов [managementAction](../resources/managedtenants-managementaction.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="583cb-113">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>|
|[<span data-ttu-id="583cb-114">Get managementAction</span><span class="sxs-lookup"><span data-stu-id="583cb-114">Get managementAction</span></span>](../api/managedtenants-managementaction-get.md)|[<span data-ttu-id="583cb-115">microsoft.graph.managedTenants.managementAction</span><span class="sxs-lookup"><span data-stu-id="583cb-115">microsoft.graph.managedTenants.managementAction</span></span>](../resources/managedtenants-managementaction.md)|<span data-ttu-id="583cb-116">Ознакомьтесь с свойствами и отношениями объекта [managementAction.](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="583cb-116">Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.</span></span>|
|[<span data-ttu-id="583cb-117">применение</span><span class="sxs-lookup"><span data-stu-id="583cb-117">apply</span></span>](../api/managedtenants-managementaction-apply.md)|[<span data-ttu-id="583cb-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="583cb-118">microsoft.graph.managedTenants.managementActionDeploymentStatus</span></span>](../resources/managedtenants-managementactiondeploymentstatus.md)|<span data-ttu-id="583cb-119">Применяет действия управления к управляемому клиенту.</span><span class="sxs-lookup"><span data-stu-id="583cb-119">Applies the management actions against the managed tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="583cb-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="583cb-120">Properties</span></span>
|<span data-ttu-id="583cb-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="583cb-121">Property</span></span>|<span data-ttu-id="583cb-122">Тип</span><span class="sxs-lookup"><span data-stu-id="583cb-122">Type</span></span>|<span data-ttu-id="583cb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="583cb-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="583cb-124">category</span><span class="sxs-lookup"><span data-stu-id="583cb-124">category</span></span>|<span data-ttu-id="583cb-125">managementCategory</span><span class="sxs-lookup"><span data-stu-id="583cb-125">managementCategory</span></span>|<span data-ttu-id="583cb-126">Категория для действия управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-126">The category for the management action.</span></span> <span data-ttu-id="583cb-127">Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="583cb-127">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="583cb-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="583cb-128">Optional.</span></span> <span data-ttu-id="583cb-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-129">Read-only.</span></span>|
|<span data-ttu-id="583cb-130">description</span><span class="sxs-lookup"><span data-stu-id="583cb-130">description</span></span>|<span data-ttu-id="583cb-131">String</span><span class="sxs-lookup"><span data-stu-id="583cb-131">String</span></span>|<span data-ttu-id="583cb-132">Описание действия управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-132">The description for the management action.</span></span> <span data-ttu-id="583cb-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="583cb-133">Optional.</span></span> <span data-ttu-id="583cb-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-134">Read-only.</span></span>|
|<span data-ttu-id="583cb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="583cb-135">displayName</span></span>|<span data-ttu-id="583cb-136">String</span><span class="sxs-lookup"><span data-stu-id="583cb-136">String</span></span>|<span data-ttu-id="583cb-137">Отображает имя для действия управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-137">The display name for the management action.</span></span> <span data-ttu-id="583cb-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="583cb-138">Optional.</span></span> <span data-ttu-id="583cb-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-139">Read-only.</span></span>|
|<span data-ttu-id="583cb-140">id</span><span class="sxs-lookup"><span data-stu-id="583cb-140">id</span></span>|<span data-ttu-id="583cb-141">String</span><span class="sxs-lookup"><span data-stu-id="583cb-141">String</span></span>|<span data-ttu-id="583cb-142">Уникальный идентификатор для действия управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-142">The unique identifier for the management action.</span></span> <span data-ttu-id="583cb-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="583cb-143">Required.</span></span> <span data-ttu-id="583cb-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-144">Read-only.</span></span>|
|<span data-ttu-id="583cb-145">referenceTemplateId</span><span class="sxs-lookup"><span data-stu-id="583cb-145">referenceTemplateId</span></span>|<span data-ttu-id="583cb-146">String</span><span class="sxs-lookup"><span data-stu-id="583cb-146">String</span></span>|<span data-ttu-id="583cb-147">Ссылка на шаблон управления, используемый для создания действия управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-147">The reference for the management template used to generate the management action.</span></span> <span data-ttu-id="583cb-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="583cb-148">Required.</span></span> <span data-ttu-id="583cb-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-149">Read-only.</span></span>|
|<span data-ttu-id="583cb-150">workloadActions</span><span class="sxs-lookup"><span data-stu-id="583cb-150">workloadActions</span></span>|<span data-ttu-id="583cb-151">[коллекция microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)</span><span class="sxs-lookup"><span data-stu-id="583cb-151">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="583cb-152">Набор действий рабочей нагрузки, связанных с действием управления.</span><span class="sxs-lookup"><span data-stu-id="583cb-152">The collection of workload actions associated with the management action.</span></span> <span data-ttu-id="583cb-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="583cb-153">Required.</span></span> <span data-ttu-id="583cb-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="583cb-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="583cb-155">Связи</span><span class="sxs-lookup"><span data-stu-id="583cb-155">Relationships</span></span>
<span data-ttu-id="583cb-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="583cb-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="583cb-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="583cb-157">JSON representation</span></span>
<span data-ttu-id="583cb-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="583cb-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
