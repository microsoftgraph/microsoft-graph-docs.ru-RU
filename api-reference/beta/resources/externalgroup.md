---
title: Тип ресурса Екстерналграуп
description: Представляет внешнюю группу, используемую для установки разрешений для Екстерналитемс, добавленных в подключение Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193939"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="d0c97-103">Тип ресурса Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="d0c97-103">externalGroup resource type</span></span>

<span data-ttu-id="d0c97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0c97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0c97-105">Представляет внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="d0c97-105">Represents an external group.</span></span> <span data-ttu-id="d0c97-106">Внешние группы (наряду с пользователями и группами Azure Active Directory) используются для установки разрешений **екстерналитемс** , добавляемых в подключение Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d0c97-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="d0c97-107">Используйте **екстерналграупс** для представления групп, не относящихся к Azure Active Directory, или конструкций, подобных группам (таких как бизнес-единицы, Teams и налево), которые определяют разрешения на доступ к контенту во внешнем источнике данных.</span><span class="sxs-lookup"><span data-stu-id="d0c97-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="d0c97-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d0c97-108">Methods</span></span>

|<span data-ttu-id="d0c97-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d0c97-109">Method</span></span>|<span data-ttu-id="d0c97-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d0c97-110">Return type</span></span>|<span data-ttu-id="d0c97-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c97-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0c97-112">Создание Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="d0c97-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="d0c97-113">екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="d0c97-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="d0c97-114">Создание нового объекта **екстерналграуп** .</span><span class="sxs-lookup"><span data-stu-id="d0c97-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="d0c97-115">Удаление Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="d0c97-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="d0c97-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d0c97-116">None</span></span>|<span data-ttu-id="d0c97-117">Удаление объекта **екстерналграуп** .</span><span class="sxs-lookup"><span data-stu-id="d0c97-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="d0c97-118">Создание участников</span><span class="sxs-lookup"><span data-stu-id="d0c97-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="d0c97-119">екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="d0c97-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="d0c97-120">Создание нового объекта **екстерналграупмембер** .</span><span class="sxs-lookup"><span data-stu-id="d0c97-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0c97-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0c97-121">Properties</span></span>

| <span data-ttu-id="d0c97-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0c97-122">Property</span></span>    | <span data-ttu-id="d0c97-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c97-123">Type</span></span>   | <span data-ttu-id="d0c97-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c97-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d0c97-125">id</span><span class="sxs-lookup"><span data-stu-id="d0c97-125">id</span></span>          | <span data-ttu-id="d0c97-126">String</span><span class="sxs-lookup"><span data-stu-id="d0c97-126">String</span></span> | <span data-ttu-id="d0c97-127">Уникальный идентификатор внешней группы в подключении.</span><span class="sxs-lookup"><span data-stu-id="d0c97-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="d0c97-128">Он должен состоять из буквенно-цифровых символов и иметь длину до 128 символов.</span><span class="sxs-lookup"><span data-stu-id="d0c97-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="d0c97-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d0c97-129">displayName</span></span> | <span data-ttu-id="d0c97-130">String</span><span class="sxs-lookup"><span data-stu-id="d0c97-130">String</span></span> | <span data-ttu-id="d0c97-131">Понятное имя внешней группы.</span><span class="sxs-lookup"><span data-stu-id="d0c97-131">The friendly name of the external group.</span></span> <span data-ttu-id="d0c97-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d0c97-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="d0c97-133">description</span><span class="sxs-lookup"><span data-stu-id="d0c97-133">description</span></span> | <span data-ttu-id="d0c97-134">String</span><span class="sxs-lookup"><span data-stu-id="d0c97-134">String</span></span> | <span data-ttu-id="d0c97-135">Описание внешней группы.</span><span class="sxs-lookup"><span data-stu-id="d0c97-135">The description of the external group.</span></span> <span data-ttu-id="d0c97-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d0c97-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="d0c97-137">Связи</span><span class="sxs-lookup"><span data-stu-id="d0c97-137">Relationships</span></span>

| <span data-ttu-id="d0c97-138">Связь</span><span class="sxs-lookup"><span data-stu-id="d0c97-138">Relationship</span></span> | <span data-ttu-id="d0c97-139">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c97-139">Type</span></span>                                                                  | <span data-ttu-id="d0c97-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c97-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="d0c97-141">members</span><span class="sxs-lookup"><span data-stu-id="d0c97-141">members</span></span>      | <span data-ttu-id="d0c97-142">Коллекция [екстерналграупмембер](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="d0c97-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="d0c97-143">Член, добавленный в объект **екстерналграуп**.</span><span class="sxs-lookup"><span data-stu-id="d0c97-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="d0c97-144">Вы можете добавлять пользователей Azure Active Directory, группы Azure Active Directory или другие **екстерналграупс** в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="d0c97-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0c97-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0c97-145">JSON representation</span></span>

<span data-ttu-id="d0c97-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0c97-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
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
