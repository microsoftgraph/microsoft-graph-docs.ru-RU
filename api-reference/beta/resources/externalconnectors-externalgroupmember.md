---
title: тип ресурса externalGroupMember
description: Представляет члена externalGroup, используемого для набора разрешений на внешний контент, добавленный в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467823"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="29e3a-103">тип ресурса externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="29e3a-103">externalGroupMember resource type</span></span>

<span data-ttu-id="29e3a-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="29e3a-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29e3a-105">Представляет члена внешней [](externalconnectors-externalgroup.md) группы, используемой для набора разрешений на внешний контент, добавленный в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="29e3a-105">Represents a member of an [externalGroup](externalconnectors-externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="29e3a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="29e3a-106">Methods</span></span>

| <span data-ttu-id="29e3a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="29e3a-107">Method</span></span>                                                              | <span data-ttu-id="29e3a-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="29e3a-108">Return type</span></span>         | <span data-ttu-id="29e3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="29e3a-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="29e3a-110">Создание externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="29e3a-110">Create externalGroupMember</span></span>](../api/externalconnectors-externalgroup-post-members.md) | [<span data-ttu-id="29e3a-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="29e3a-111">externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md) | <span data-ttu-id="29e3a-112">Создание нового **внешнего объектаGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="29e3a-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="29e3a-113">Удаление externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="29e3a-113">Delete externalGroupMember</span></span>](../api/externalconnectors-externalgroupmember-delete.md)  | <span data-ttu-id="29e3a-114">Нет</span><span class="sxs-lookup"><span data-stu-id="29e3a-114">None</span></span>                | <span data-ttu-id="29e3a-115">Удаление **внешнего объектаGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="29e3a-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="29e3a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="29e3a-116">Properties</span></span>

| <span data-ttu-id="29e3a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="29e3a-117">Property</span></span>       | <span data-ttu-id="29e3a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="29e3a-118">Type</span></span>                    | <span data-ttu-id="29e3a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="29e3a-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="29e3a-120">id</span><span class="sxs-lookup"><span data-stu-id="29e3a-120">id</span></span>             | <span data-ttu-id="29e3a-121">String</span><span class="sxs-lookup"><span data-stu-id="29e3a-121">String</span></span>                  | <span data-ttu-id="29e3a-122">Уникальный ID участника.</span><span class="sxs-lookup"><span data-stu-id="29e3a-122">The unique ID of the member.</span></span> <span data-ttu-id="29e3a-123">Это будет objectId в случае Azure Active Directory пользователей или групп и **id** свойства **externalGroup** в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="29e3a-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="29e3a-124">type</span><span class="sxs-lookup"><span data-stu-id="29e3a-124">type</span></span>           | <span data-ttu-id="29e3a-125">microsoft.graph.externalConnectors.externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="29e3a-125">microsoft.graph.externalConnectors.externalGroupMemberType</span></span> | <span data-ttu-id="29e3a-126">Тип участника, добавленного во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="29e3a-126">The type of member added to the external group.</span></span> <span data-ttu-id="29e3a-127">Возможные значения: или когда identitySource является и только `user` `group`  `azureActiveDirectory` `group` тогда, когда **identitySource** `external` является .</span><span class="sxs-lookup"><span data-stu-id="29e3a-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="29e3a-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="29e3a-128">identitySource</span></span> | <span data-ttu-id="29e3a-129">microsoft.graph.externalConnectors.identitySourceType</span><span class="sxs-lookup"><span data-stu-id="29e3a-129">microsoft.graph.externalConnectors.identitySourceType</span></span>      | <span data-ttu-id="29e3a-130">Источник удостоверений, к которой принадлежит член.</span><span class="sxs-lookup"><span data-stu-id="29e3a-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="29e3a-131">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="29e3a-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="29e3a-132">Связи</span><span class="sxs-lookup"><span data-stu-id="29e3a-132">Relationships</span></span>

<span data-ttu-id="29e3a-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29e3a-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29e3a-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29e3a-134">JSON representation</span></span>

<span data-ttu-id="29e3a-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29e3a-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
