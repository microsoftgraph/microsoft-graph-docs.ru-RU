---
title: Тип ресурса externalGroup
description: Представляет внешнюю группу, используемую для изменения разрешений для externalItems, добавленных к подключению Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161714"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="6d1af-103">Тип ресурса externalGroup</span><span class="sxs-lookup"><span data-stu-id="6d1af-103">externalGroup resource type</span></span>

<span data-ttu-id="6d1af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d1af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1af-105">Представляет внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="6d1af-105">Represents an external group.</span></span> <span data-ttu-id="6d1af-106">Внешние группы (наряду с пользователями и группами Azure Active Directory) используются для изменения разрешений **для externalItems,** добавленных к подключению Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6d1af-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="6d1af-107">Используйте **externalGroups** для представления групп, не в том числе Azure Active Directory, или конструкций, похожих на группы (таких как бизнес-единицы, Teams и другие), которые определяют разрешения на содержимое во внешнем источнике данных.</span><span class="sxs-lookup"><span data-stu-id="6d1af-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="6d1af-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6d1af-108">Methods</span></span>

|<span data-ttu-id="6d1af-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6d1af-109">Method</span></span>|<span data-ttu-id="6d1af-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6d1af-110">Return type</span></span>|<span data-ttu-id="6d1af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d1af-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d1af-112">Создание externalGroup</span><span class="sxs-lookup"><span data-stu-id="6d1af-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="6d1af-113">externalGroup</span><span class="sxs-lookup"><span data-stu-id="6d1af-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="6d1af-114">Создание объекта **externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="6d1af-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="6d1af-115">Удаление externalGroup</span><span class="sxs-lookup"><span data-stu-id="6d1af-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="6d1af-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6d1af-116">None</span></span>|<span data-ttu-id="6d1af-117">Удаление объекта **externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="6d1af-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="6d1af-118">Создание участников</span><span class="sxs-lookup"><span data-stu-id="6d1af-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="6d1af-119">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="6d1af-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="6d1af-120">Создание объекта **externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="6d1af-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d1af-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d1af-121">Properties</span></span>

| <span data-ttu-id="6d1af-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d1af-122">Property</span></span>    | <span data-ttu-id="6d1af-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6d1af-123">Type</span></span>   | <span data-ttu-id="6d1af-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6d1af-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6d1af-125">id</span><span class="sxs-lookup"><span data-stu-id="6d1af-125">id</span></span>          | <span data-ttu-id="6d1af-126">String</span><span class="sxs-lookup"><span data-stu-id="6d1af-126">String</span></span> | <span data-ttu-id="6d1af-127">Уникальный ИД внешней группы в соединении.</span><span class="sxs-lookup"><span data-stu-id="6d1af-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="6d1af-128">Она должна быть букво-цифрой и длиной до 128 символов.</span><span class="sxs-lookup"><span data-stu-id="6d1af-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="6d1af-129">displayName</span><span class="sxs-lookup"><span data-stu-id="6d1af-129">displayName</span></span> | <span data-ttu-id="6d1af-130">String</span><span class="sxs-lookup"><span data-stu-id="6d1af-130">String</span></span> | <span data-ttu-id="6d1af-131">Имя внешней группы.</span><span class="sxs-lookup"><span data-stu-id="6d1af-131">The friendly name of the external group.</span></span> <span data-ttu-id="6d1af-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6d1af-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="6d1af-133">description</span><span class="sxs-lookup"><span data-stu-id="6d1af-133">description</span></span> | <span data-ttu-id="6d1af-134">String</span><span class="sxs-lookup"><span data-stu-id="6d1af-134">String</span></span> | <span data-ttu-id="6d1af-135">Описание внешней группы.</span><span class="sxs-lookup"><span data-stu-id="6d1af-135">The description of the external group.</span></span> <span data-ttu-id="6d1af-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6d1af-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="6d1af-137">Связи</span><span class="sxs-lookup"><span data-stu-id="6d1af-137">Relationships</span></span>

| <span data-ttu-id="6d1af-138">Связь</span><span class="sxs-lookup"><span data-stu-id="6d1af-138">Relationship</span></span> | <span data-ttu-id="6d1af-139">Тип</span><span class="sxs-lookup"><span data-stu-id="6d1af-139">Type</span></span>                                                                  | <span data-ttu-id="6d1af-140">Описание</span><span class="sxs-lookup"><span data-stu-id="6d1af-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="6d1af-141">members</span><span class="sxs-lookup"><span data-stu-id="6d1af-141">members</span></span>      | <span data-ttu-id="6d1af-142">[Коллекция externalGroupMember](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="6d1af-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="6d1af-143">Член, добавленный в **внешнюю группу.**</span><span class="sxs-lookup"><span data-stu-id="6d1af-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="6d1af-144">В качестве участников можно добавить пользователей Azure Active Directory, группы Azure Active Directory или другие **внешние группы.**</span><span class="sxs-lookup"><span data-stu-id="6d1af-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d1af-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d1af-145">JSON representation</span></span>

<span data-ttu-id="6d1af-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d1af-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
