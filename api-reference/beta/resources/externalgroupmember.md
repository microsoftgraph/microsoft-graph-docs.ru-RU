---
title: Тип ресурса externalGroupMember
description: Представляет члена внешней группы, используемой для изменения разрешений для внешнего контента, добавленного в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161693"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="609e4-103">Тип ресурса externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="609e4-103">externalGroupMember resource type</span></span>

<span data-ttu-id="609e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="609e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="609e4-105">Представляет члена внешней группы, [используемой для](externalgroup.md) изменения разрешений для внешнего контента, добавленного в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="609e4-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="609e4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="609e4-106">Methods</span></span>

| <span data-ttu-id="609e4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="609e4-107">Method</span></span>                                                              | <span data-ttu-id="609e4-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="609e4-108">Return type</span></span>         | <span data-ttu-id="609e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="609e4-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="609e4-110">Создание externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="609e4-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="609e4-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="609e4-111">externalGroupMember</span></span> | <span data-ttu-id="609e4-112">Создание объекта **externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="609e4-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="609e4-113">Удаление externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="609e4-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="609e4-114">Нет</span><span class="sxs-lookup"><span data-stu-id="609e4-114">None</span></span>                | <span data-ttu-id="609e4-115">Удаление объекта **externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="609e4-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="609e4-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="609e4-116">Properties</span></span>

| <span data-ttu-id="609e4-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="609e4-117">Property</span></span>       | <span data-ttu-id="609e4-118">Тип</span><span class="sxs-lookup"><span data-stu-id="609e4-118">Type</span></span>                    | <span data-ttu-id="609e4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="609e4-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="609e4-120">id</span><span class="sxs-lookup"><span data-stu-id="609e4-120">id</span></span>             | <span data-ttu-id="609e4-121">String</span><span class="sxs-lookup"><span data-stu-id="609e4-121">String</span></span>                  | <span data-ttu-id="609e4-122">Уникальный ИД участника.</span><span class="sxs-lookup"><span data-stu-id="609e4-122">The unique ID of the member.</span></span> <span data-ttu-id="609e4-123">Это будет objectId в случае пользователей или групп Azure Active Directory и свойство **id** **внешней группы** в случае внешних групп.</span><span class="sxs-lookup"><span data-stu-id="609e4-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="609e4-124">type</span><span class="sxs-lookup"><span data-stu-id="609e4-124">type</span></span>           | <span data-ttu-id="609e4-125">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="609e4-125">externalGroupMemberType</span></span> | <span data-ttu-id="609e4-126">Тип участника, добавленного во внешнюю группу.</span><span class="sxs-lookup"><span data-stu-id="609e4-126">The type of member added to the external group.</span></span> <span data-ttu-id="609e4-127">Возможные значения: `user` или когда идентификатор `group` **identitySource** и только `azureActiveDirectory` `group` тогда, когда идентификатор **identitySource** имеет значение `external` .</span><span class="sxs-lookup"><span data-stu-id="609e4-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="609e4-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="609e4-128">identitySource</span></span> | <span data-ttu-id="609e4-129">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="609e4-129">identitySourceType</span></span>      | <span data-ttu-id="609e4-130">Источник удостоверений, к которой принадлежит участник.</span><span class="sxs-lookup"><span data-stu-id="609e4-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="609e4-131">Возможные значения: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="609e4-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="609e4-132">Связи</span><span class="sxs-lookup"><span data-stu-id="609e4-132">Relationships</span></span>

<span data-ttu-id="609e4-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="609e4-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="609e4-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="609e4-134">JSON representation</span></span>

<span data-ttu-id="609e4-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="609e4-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
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
