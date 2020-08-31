---
title: сложный тип Рекуесторсеттингс
description: Используется для `requestorSettings` Свойства политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора пользователей, которые могут создавать запросы.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f54a0c00c7a906e67d8c2861eae7c8437a28fad0
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311839"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="19c75-104">Тип ресурса Рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="19c75-104">requestorSettings resource type</span></span>

<span data-ttu-id="19c75-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19c75-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19c75-106">Используется для свойства **рекуесторсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19c75-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="19c75-107">Предоставляет дополнительные параметры для выбора пользователей, которые могут создать запрос для пакета доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="19c75-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="19c75-108">Кто может запрашивать</span><span class="sxs-lookup"><span data-stu-id="19c75-108">Who can request</span></span> | <span data-ttu-id="19c75-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="19c75-109">scopeType</span></span> | <span data-ttu-id="19c75-110">Коллекция Алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="19c75-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="19c75-111">Никто</span><span class="sxs-lookup"><span data-stu-id="19c75-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="19c75-112">пустой массив</span><span class="sxs-lookup"><span data-stu-id="19c75-112">empty array</span></span>|
|<span data-ttu-id="19c75-113">Отдельный пользователь в каталоге</span><span class="sxs-lookup"><span data-stu-id="19c75-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="19c75-114">SingleUser.</span><span class="sxs-lookup"><span data-stu-id="19c75-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="19c75-115">Пользователи в каталоге, которые являются участниками группы</span><span class="sxs-lookup"><span data-stu-id="19c75-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="19c75-116">граупмемберс</span><span class="sxs-lookup"><span data-stu-id="19c75-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="19c75-117">Пользователи в каталоге со `userType` значением `member`</span><span class="sxs-lookup"><span data-stu-id="19c75-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="19c75-118">пустой массив</span><span class="sxs-lookup"><span data-stu-id="19c75-118">empty array</span></span>|
|<span data-ttu-id="19c75-119">Пользователи в каталоге</span><span class="sxs-lookup"><span data-stu-id="19c75-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="19c75-120">пустой массив</span><span class="sxs-lookup"><span data-stu-id="19c75-120">empty array</span></span>|
|<span data-ttu-id="19c75-121">Пользователи в определенных подключенных организациях</span><span class="sxs-lookup"><span data-stu-id="19c75-121">Users in specific connected organizations</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="19c75-122">коннектедорганизатионмемберс</span><span class="sxs-lookup"><span data-stu-id="19c75-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="19c75-123">Пользователи из любых подключенных организаций, у которых в свойстве State для связанной организации задано значение `configured` .</span><span class="sxs-lookup"><span data-stu-id="19c75-123">Users from any connected organizations that have the state property of the connected organization set to `configured`.</span></span>|`AllConfiguredConnectedOrganizationSubjects`|<span data-ttu-id="19c75-124">пустой массив</span><span class="sxs-lookup"><span data-stu-id="19c75-124">empty array</span></span>|
|<span data-ttu-id="19c75-125">Любой пользователь</span><span class="sxs-lookup"><span data-stu-id="19c75-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="19c75-126">пустой массив</span><span class="sxs-lookup"><span data-stu-id="19c75-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="19c75-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="19c75-127">Properties</span></span>

| <span data-ttu-id="19c75-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="19c75-128">Property</span></span>                     | <span data-ttu-id="19c75-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19c75-129">Type</span></span>                      | <span data-ttu-id="19c75-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19c75-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="19c75-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="19c75-131">scopeType</span></span> |<span data-ttu-id="19c75-132">String</span><span class="sxs-lookup"><span data-stu-id="19c75-132">String</span></span> |<span data-ttu-id="19c75-133">Кто может запрашивать.</span><span class="sxs-lookup"><span data-stu-id="19c75-133">Who can request.</span></span> <span data-ttu-id="19c75-134">Один из `NoSubjects` ,,,,, `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` или `AllExternalSubjects` .</span><span class="sxs-lookup"><span data-stu-id="19c75-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="19c75-135">акцептрекуестс</span><span class="sxs-lookup"><span data-stu-id="19c75-135">acceptRequests</span></span> | <span data-ttu-id="19c75-136">Логический</span><span class="sxs-lookup"><span data-stu-id="19c75-136">Boolean</span></span> | <span data-ttu-id="19c75-137">Указывает, принимаются ли новые запросы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="19c75-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="19c75-138">алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="19c75-138">allowedRequestors</span></span> | <span data-ttu-id="19c75-139">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="19c75-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="19c75-140">Пользователи, которым разрешено запрашивать эту политику, которая может быть [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md)и [коннектедорганизатионмемберс](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="19c75-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19c75-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19c75-141">JSON representation</span></span>


<span data-ttu-id="19c75-142">Ниже приведено представление объекта **рекуесторсеттингс** в формате JSON, которое позволяет членам группы запрашивать.</span><span class="sxs-lookup"><span data-stu-id="19c75-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

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
