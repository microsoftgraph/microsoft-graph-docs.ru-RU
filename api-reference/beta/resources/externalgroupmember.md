---
title: Тип ресурса Екстерналграупмембер
description: Представляет члена объекта Екстерналграуп, используемого для установки разрешений на доступ к внешнему контенту, добавленному в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193936"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="5fc26-103">Тип ресурса Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="5fc26-103">externalGroupMember resource type</span></span>

<span data-ttu-id="5fc26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc26-105">Представляет члена объекта [екстерналграуп](externalgroup.md) , используемого для установки разрешений на доступ к внешнему контенту, добавленному в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fc26-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="5fc26-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5fc26-106">Methods</span></span>

| <span data-ttu-id="5fc26-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5fc26-107">Method</span></span>                                                              | <span data-ttu-id="5fc26-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5fc26-108">Return type</span></span>         | <span data-ttu-id="5fc26-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc26-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="5fc26-110">Создание Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="5fc26-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="5fc26-111">екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="5fc26-111">externalGroupMember</span></span> | <span data-ttu-id="5fc26-112">Создание нового объекта **екстерналграупмембер** .</span><span class="sxs-lookup"><span data-stu-id="5fc26-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="5fc26-113">Удаление Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="5fc26-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="5fc26-114">Нет</span><span class="sxs-lookup"><span data-stu-id="5fc26-114">None</span></span>                | <span data-ttu-id="5fc26-115">Удаление объекта **екстерналграупмембер** .</span><span class="sxs-lookup"><span data-stu-id="5fc26-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="5fc26-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fc26-116">Properties</span></span>

| <span data-ttu-id="5fc26-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fc26-117">Property</span></span>       | <span data-ttu-id="5fc26-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5fc26-118">Type</span></span>                    | <span data-ttu-id="5fc26-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc26-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="5fc26-120">id</span><span class="sxs-lookup"><span data-stu-id="5fc26-120">id</span></span>             | <span data-ttu-id="5fc26-121">String</span><span class="sxs-lookup"><span data-stu-id="5fc26-121">String</span></span>                  | <span data-ttu-id="5fc26-122">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="5fc26-122">The unique ID of the member.</span></span> <span data-ttu-id="5fc26-123">Это идентификатор objectId в случае с пользователями или группами Azure Active Directory, а также свойством **ID** **екстерналграуп** в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="5fc26-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="5fc26-124">type</span><span class="sxs-lookup"><span data-stu-id="5fc26-124">type</span></span>           | <span data-ttu-id="5fc26-125">екстерналграупмембертипе</span><span class="sxs-lookup"><span data-stu-id="5fc26-125">externalGroupMemberType</span></span> | <span data-ttu-id="5fc26-126">Тип элемента, добавляемого во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="5fc26-126">The type of member added to the external group.</span></span> <span data-ttu-id="5fc26-127">Возможные значения: `user` или `group` , если **идентитисаурце** , `azureActiveDirectory` и только в том `group` случае, если **идентитисаурце** `external` .</span><span class="sxs-lookup"><span data-stu-id="5fc26-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="5fc26-128">идентитисаурце</span><span class="sxs-lookup"><span data-stu-id="5fc26-128">identitySource</span></span> | <span data-ttu-id="5fc26-129">идентитисаурцетипе</span><span class="sxs-lookup"><span data-stu-id="5fc26-129">identitySourceType</span></span>      | <span data-ttu-id="5fc26-130">Источник удостоверения, к которому принадлежит член.</span><span class="sxs-lookup"><span data-stu-id="5fc26-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="5fc26-131">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="5fc26-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="5fc26-132">Связи</span><span class="sxs-lookup"><span data-stu-id="5fc26-132">Relationships</span></span>

<span data-ttu-id="5fc26-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5fc26-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fc26-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5fc26-134">JSON representation</span></span>

<span data-ttu-id="5fc26-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fc26-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
