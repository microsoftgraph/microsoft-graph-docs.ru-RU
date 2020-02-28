---
title: сложный тип Рекуесторсеттингс
description: Используется для `requestorSettings` свойства политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора пользователей, которые могут создавать запросы.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3205a6ef07c5cf09d8faeb07d19d760872d1e6
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331401"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="1317e-104">Тип ресурса Рекуесторсеттингс</span><span class="sxs-lookup"><span data-stu-id="1317e-104">requestorSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1317e-105">Используется для свойства **рекуесторсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1317e-105">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="1317e-106">Предоставляет дополнительные параметры для выбора пользователей, которые могут создать запрос для пакета доступа в этой политике.</span><span class="sxs-lookup"><span data-stu-id="1317e-106">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="1317e-107">Кто может запрашивать</span><span class="sxs-lookup"><span data-stu-id="1317e-107">Who can request</span></span> | <span data-ttu-id="1317e-108">scopeType</span><span class="sxs-lookup"><span data-stu-id="1317e-108">scopeType</span></span> | <span data-ttu-id="1317e-109">Коллекция Алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="1317e-109">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="1317e-110">Никто</span><span class="sxs-lookup"><span data-stu-id="1317e-110">No one</span></span>|`NoSubjects`|<span data-ttu-id="1317e-111">пустой массив</span><span class="sxs-lookup"><span data-stu-id="1317e-111">empty array</span></span>|
|<span data-ttu-id="1317e-112">Отдельный пользователь в каталоге</span><span class="sxs-lookup"><span data-stu-id="1317e-112">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="1317e-113">SingleUser.</span><span class="sxs-lookup"><span data-stu-id="1317e-113">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="1317e-114">Пользователи в каталоге, которые являются участниками группы</span><span class="sxs-lookup"><span data-stu-id="1317e-114">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="1317e-115">граупмемберс</span><span class="sxs-lookup"><span data-stu-id="1317e-115">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="1317e-116">Пользователи в каталоге со `userType` значением`member`</span><span class="sxs-lookup"><span data-stu-id="1317e-116">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="1317e-117">пустой массив</span><span class="sxs-lookup"><span data-stu-id="1317e-117">empty array</span></span>|
|<span data-ttu-id="1317e-118">Пользователи в каталоге</span><span class="sxs-lookup"><span data-stu-id="1317e-118">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="1317e-119">пустой массив</span><span class="sxs-lookup"><span data-stu-id="1317e-119">empty array</span></span>|
|<span data-ttu-id="1317e-120">Пользователи, уже настроенные в определенных организациях</span><span class="sxs-lookup"><span data-stu-id="1317e-120">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="1317e-121">коннектедорганизатионмемберс</span><span class="sxs-lookup"><span data-stu-id="1317e-121">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="1317e-122">Пользователи из других подключенных организаций, уже настроенных</span><span class="sxs-lookup"><span data-stu-id="1317e-122">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="1317e-123">пустой массив</span><span class="sxs-lookup"><span data-stu-id="1317e-123">empty array</span></span>|
|<span data-ttu-id="1317e-124">Любой пользователь</span><span class="sxs-lookup"><span data-stu-id="1317e-124">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="1317e-125">пустой массив</span><span class="sxs-lookup"><span data-stu-id="1317e-125">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="1317e-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="1317e-126">Properties</span></span>

| <span data-ttu-id="1317e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1317e-127">Property</span></span>                     | <span data-ttu-id="1317e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1317e-128">Type</span></span>                      | <span data-ttu-id="1317e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1317e-129">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="1317e-130">scopeType</span><span class="sxs-lookup"><span data-stu-id="1317e-130">scopeType</span></span> |<span data-ttu-id="1317e-131">String</span><span class="sxs-lookup"><span data-stu-id="1317e-131">String</span></span> |<span data-ttu-id="1317e-132">Кто может запрашивать.</span><span class="sxs-lookup"><span data-stu-id="1317e-132">Who can request.</span></span> <span data-ttu-id="1317e-133">Один из `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers`,, `AllExistingDirectorySubjects` или `AllExternalSubjects`.</span><span class="sxs-lookup"><span data-stu-id="1317e-133">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="1317e-134">акцептрекуестс</span><span class="sxs-lookup"><span data-stu-id="1317e-134">acceptRequests</span></span> | <span data-ttu-id="1317e-135">Логический</span><span class="sxs-lookup"><span data-stu-id="1317e-135">Boolean</span></span> | <span data-ttu-id="1317e-136">Указывает, принимаются ли новые запросы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1317e-136">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="1317e-137">алловедрекуесторс</span><span class="sxs-lookup"><span data-stu-id="1317e-137">allowedRequestors</span></span> | <span data-ttu-id="1317e-138">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="1317e-138">[userSet](userset.md) collection</span></span>| <span data-ttu-id="1317e-139">Пользователи, которым разрешено запрашивать эту политику, которая может быть [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md)и [коннектедорганизатионмемберс](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="1317e-139">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1317e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1317e-140">JSON representation</span></span>


<span data-ttu-id="1317e-141">Ниже приведено представление объекта **рекуесторсеттингс** в формате JSON, которое позволяет членам группы запрашивать.</span><span class="sxs-lookup"><span data-stu-id="1317e-141">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

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
