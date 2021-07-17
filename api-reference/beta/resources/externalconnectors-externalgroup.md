---
title: тип ресурсов externalGroup
description: Представляет внешнюю группу, используемую для набора разрешений на externalItems, добавленных в подключение Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467827"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="5b8c9-103">тип ресурсов externalGroup</span><span class="sxs-lookup"><span data-stu-id="5b8c9-103">externalGroup resource type</span></span>

<span data-ttu-id="5b8c9-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="5b8c9-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b8c9-105">Представляет внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-105">Represents an external group.</span></span> <span data-ttu-id="5b8c9-106">Внешние группы (наряду Azure Active Directory пользователями и группами) используются для набора разрешений **на externalItems,** добавленных в подключение Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="5b8c9-107">Используйте **externalGroups** для представления Azure Active Directory групп или групп-подобных конструкций (например, бизнес-подразделений, Teams и son on), которые определяют разрешение на контент в внешнем источнике данных.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="5b8c9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5b8c9-108">Methods</span></span>

|<span data-ttu-id="5b8c9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5b8c9-109">Method</span></span>|<span data-ttu-id="5b8c9-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5b8c9-110">Return type</span></span>|<span data-ttu-id="5b8c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b8c9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b8c9-112">Создание externalGroup</span><span class="sxs-lookup"><span data-stu-id="5b8c9-112">Create externalGroup</span></span>](../api/externalconnectors-externalconnection-post-groups.md)|[<span data-ttu-id="5b8c9-113">microsoft.graph.externalConnectors.externalGroup</span><span class="sxs-lookup"><span data-stu-id="5b8c9-113">microsoft.graph.externalConnectors.externalGroup</span></span>](../resources/externalconnectors-externalgroup.md)|<span data-ttu-id="5b8c9-114">Создайте новый **объект externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="5b8c9-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="5b8c9-115">Удаление externalGroup</span><span class="sxs-lookup"><span data-stu-id="5b8c9-115">Delete externalGroup</span></span>](../api/externalconnectors-externalgroup-delete.md)|<span data-ttu-id="5b8c9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5b8c9-116">None</span></span>|<span data-ttu-id="5b8c9-117">Удаление **объекта externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="5b8c9-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="5b8c9-118">Создание участников</span><span class="sxs-lookup"><span data-stu-id="5b8c9-118">Create members</span></span>](../api/externalconnectors-externalgroup-post-members.md)|[<span data-ttu-id="5b8c9-119">microsoft.graph.externalConnectors.externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="5b8c9-119">microsoft.graph.externalConnectors.externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md)|<span data-ttu-id="5b8c9-120">Создание нового **внешнего объектаGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="5b8c9-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b8c9-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b8c9-121">Properties</span></span>

| <span data-ttu-id="5b8c9-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b8c9-122">Property</span></span>    | <span data-ttu-id="5b8c9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5b8c9-123">Type</span></span>   | <span data-ttu-id="5b8c9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5b8c9-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5b8c9-125">id</span><span class="sxs-lookup"><span data-stu-id="5b8c9-125">id</span></span>          | <span data-ttu-id="5b8c9-126">String</span><span class="sxs-lookup"><span data-stu-id="5b8c9-126">String</span></span> | <span data-ttu-id="5b8c9-127">Уникальный ID внешней группы в подключении.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="5b8c9-128">Он должен быть альфа-числом и может иметь длину до 128 символов.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="5b8c9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="5b8c9-129">displayName</span></span> | <span data-ttu-id="5b8c9-130">String</span><span class="sxs-lookup"><span data-stu-id="5b8c9-130">String</span></span> | <span data-ttu-id="5b8c9-131">Дружеское имя внешней группы.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-131">The friendly name of the external group.</span></span> <span data-ttu-id="5b8c9-132">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="5b8c9-133">description</span><span class="sxs-lookup"><span data-stu-id="5b8c9-133">description</span></span> | <span data-ttu-id="5b8c9-134">String</span><span class="sxs-lookup"><span data-stu-id="5b8c9-134">String</span></span> | <span data-ttu-id="5b8c9-135">Описание внешней группы.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-135">The description of the external group.</span></span> <span data-ttu-id="5b8c9-136">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="5b8c9-137">Связи</span><span class="sxs-lookup"><span data-stu-id="5b8c9-137">Relationships</span></span>

| <span data-ttu-id="5b8c9-138">Связь</span><span class="sxs-lookup"><span data-stu-id="5b8c9-138">Relationship</span></span> | <span data-ttu-id="5b8c9-139">Тип</span><span class="sxs-lookup"><span data-stu-id="5b8c9-139">Type</span></span>                                                                  | <span data-ttu-id="5b8c9-140">Описание</span><span class="sxs-lookup"><span data-stu-id="5b8c9-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="5b8c9-141">members</span><span class="sxs-lookup"><span data-stu-id="5b8c9-141">members</span></span>      | <span data-ttu-id="5b8c9-142">[коллекция microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="5b8c9-142">[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) collection</span></span> | <span data-ttu-id="5b8c9-143">Член, добавленный в **externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="5b8c9-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="5b8c9-144">В качестве участников можно Azure Active Directory пользователей, Azure Active Directory групп или других **внешних групп.**</span><span class="sxs-lookup"><span data-stu-id="5b8c9-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b8c9-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b8c9-145">JSON representation</span></span>

<span data-ttu-id="5b8c9-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b8c9-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
