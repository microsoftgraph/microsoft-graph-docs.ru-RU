---
title: сложный тип Рекуесторсеттингс
description: Используется для `requestorSettings` свойства политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора пользователей, которые могут создавать запросы.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b52f3276185f819ccd0e7149dbd5420b4f6e1781
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521119"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="e6101-104">Тип ресурса Рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="e6101-104">requestorSettings resource type</span></span>

<span data-ttu-id="e6101-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6101-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6101-106">Используется для свойства **рекуесторсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6101-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="e6101-107">Предоставляет дополнительные параметры для выбора пользователей, которые могут создать запрос для пакета доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="e6101-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="e6101-108">Кто может запрашивать</span><span class="sxs-lookup"><span data-stu-id="e6101-108">Who can request</span></span> | <span data-ttu-id="e6101-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="e6101-109">scopeType</span></span> | <span data-ttu-id="e6101-110">Коллекция Алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="e6101-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="e6101-111">Никто</span><span class="sxs-lookup"><span data-stu-id="e6101-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="e6101-112">пустой массив</span><span class="sxs-lookup"><span data-stu-id="e6101-112">empty array</span></span>|
|<span data-ttu-id="e6101-113">Отдельный пользователь в каталоге</span><span class="sxs-lookup"><span data-stu-id="e6101-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="e6101-114">SingleUser.</span><span class="sxs-lookup"><span data-stu-id="e6101-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="e6101-115">Пользователи в каталоге, которые являются участниками группы</span><span class="sxs-lookup"><span data-stu-id="e6101-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="e6101-116">граупмемберс</span><span class="sxs-lookup"><span data-stu-id="e6101-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="e6101-117">Пользователи в каталоге со `userType` значением`member`</span><span class="sxs-lookup"><span data-stu-id="e6101-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="e6101-118">пустой массив</span><span class="sxs-lookup"><span data-stu-id="e6101-118">empty array</span></span>|
|<span data-ttu-id="e6101-119">Пользователи в каталоге</span><span class="sxs-lookup"><span data-stu-id="e6101-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="e6101-120">пустой массив</span><span class="sxs-lookup"><span data-stu-id="e6101-120">empty array</span></span>|
|<span data-ttu-id="e6101-121">Пользователи, уже настроенные в определенных организациях</span><span class="sxs-lookup"><span data-stu-id="e6101-121">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="e6101-122">коннектедорганизатионмемберс</span><span class="sxs-lookup"><span data-stu-id="e6101-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="e6101-123">Пользователи из других подключенных организаций, уже настроенных</span><span class="sxs-lookup"><span data-stu-id="e6101-123">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="e6101-124">пустой массив</span><span class="sxs-lookup"><span data-stu-id="e6101-124">empty array</span></span>|
|<span data-ttu-id="e6101-125">Любой пользователь</span><span class="sxs-lookup"><span data-stu-id="e6101-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="e6101-126">пустой массив</span><span class="sxs-lookup"><span data-stu-id="e6101-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="e6101-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6101-127">Properties</span></span>

| <span data-ttu-id="e6101-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6101-128">Property</span></span>                     | <span data-ttu-id="e6101-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e6101-129">Type</span></span>                      | <span data-ttu-id="e6101-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e6101-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="e6101-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="e6101-131">scopeType</span></span> |<span data-ttu-id="e6101-132">String</span><span class="sxs-lookup"><span data-stu-id="e6101-132">String</span></span> |<span data-ttu-id="e6101-133">Кто может запрашивать.</span><span class="sxs-lookup"><span data-stu-id="e6101-133">Who can request.</span></span> <span data-ttu-id="e6101-134">Один из `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers`,, `AllExistingDirectorySubjects` или `AllExternalSubjects`.</span><span class="sxs-lookup"><span data-stu-id="e6101-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="e6101-135">акцептрекуестс</span><span class="sxs-lookup"><span data-stu-id="e6101-135">acceptRequests</span></span> | <span data-ttu-id="e6101-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6101-136">Boolean</span></span> | <span data-ttu-id="e6101-137">Указывает, принимаются ли новые запросы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6101-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="e6101-138">алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="e6101-138">allowedRequestors</span></span> | <span data-ttu-id="e6101-139">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="e6101-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="e6101-140">Пользователи, которым разрешено запрашивать эту политику, которая может быть [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md)и [коннектедорганизатионмемберс](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="e6101-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6101-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6101-141">JSON representation</span></span>


<span data-ttu-id="e6101-142">Ниже приведено представление объекта **рекуесторсеттингс** в формате JSON, которое позволяет членам группы запрашивать.</span><span class="sxs-lookup"><span data-stu-id="e6101-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
