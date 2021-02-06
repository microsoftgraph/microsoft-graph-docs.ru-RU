---
title: Сложный тип requestorSettings
description: Используется для `requestorSettings` свойства политики назначения пакета доступа. Предоставляет дополнительные параметры для выбора, кто может создать запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a9bd91605d106b488de21f29baefe4b31d28f323
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133730"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="2fd38-104">Тип ресурса requestorSettings</span><span class="sxs-lookup"><span data-stu-id="2fd38-104">requestorSettings resource type</span></span>

<span data-ttu-id="2fd38-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd38-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fd38-106">Используется для **свойства requestorSettings** политики [назначения пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fd38-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="2fd38-107">Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на пакет доступа для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2fd38-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="2fd38-108">Кто может запросить</span><span class="sxs-lookup"><span data-stu-id="2fd38-108">Who can request</span></span> | <span data-ttu-id="2fd38-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="2fd38-109">scopeType</span></span> | <span data-ttu-id="2fd38-110">Коллекция allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="2fd38-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="2fd38-111">Никто</span><span class="sxs-lookup"><span data-stu-id="2fd38-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="2fd38-112">пустой массив</span><span class="sxs-lookup"><span data-stu-id="2fd38-112">empty array</span></span>|
|<span data-ttu-id="2fd38-113">Конкретный пользователь в каталоге</span><span class="sxs-lookup"><span data-stu-id="2fd38-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="2fd38-114">singleUser</span><span class="sxs-lookup"><span data-stu-id="2fd38-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="2fd38-115">Пользователи в каталоге, которые являются участниками группы</span><span class="sxs-lookup"><span data-stu-id="2fd38-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="2fd38-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="2fd38-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="2fd38-117">Пользователи в каталоге со `userType` значением `member`</span><span class="sxs-lookup"><span data-stu-id="2fd38-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="2fd38-118">пустой массив</span><span class="sxs-lookup"><span data-stu-id="2fd38-118">empty array</span></span>|
|<span data-ttu-id="2fd38-119">Пользователи в каталоге</span><span class="sxs-lookup"><span data-stu-id="2fd38-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="2fd38-120">пустой массив</span><span class="sxs-lookup"><span data-stu-id="2fd38-120">empty array</span></span>|
|<span data-ttu-id="2fd38-121">Пользователи в определенных подключенных организациях</span><span class="sxs-lookup"><span data-stu-id="2fd38-121">Users in specific connected organizations</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="2fd38-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="2fd38-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="2fd38-123">Пользователи из всех подключенных организаций, для свойства состояния подключенной организации установлено состояние `configured` .</span><span class="sxs-lookup"><span data-stu-id="2fd38-123">Users from any connected organizations that have the state property of the connected organization set to `configured`.</span></span>|`AllConfiguredConnectedOrganizationSubjects`|<span data-ttu-id="2fd38-124">пустой массив</span><span class="sxs-lookup"><span data-stu-id="2fd38-124">empty array</span></span>|
|<span data-ttu-id="2fd38-125">Любой пользователь</span><span class="sxs-lookup"><span data-stu-id="2fd38-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="2fd38-126">пустой массив</span><span class="sxs-lookup"><span data-stu-id="2fd38-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="2fd38-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fd38-127">Properties</span></span>

| <span data-ttu-id="2fd38-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fd38-128">Property</span></span>                     | <span data-ttu-id="2fd38-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2fd38-129">Type</span></span>                      | <span data-ttu-id="2fd38-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2fd38-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2fd38-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="2fd38-131">scopeType</span></span> |<span data-ttu-id="2fd38-132">Строка</span><span class="sxs-lookup"><span data-stu-id="2fd38-132">String</span></span> |<span data-ttu-id="2fd38-133">Кто может запросить.</span><span class="sxs-lookup"><span data-stu-id="2fd38-133">Who can request.</span></span> <span data-ttu-id="2fd38-134">Один из `NoSubjects` , , , , , , или `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` .</span><span class="sxs-lookup"><span data-stu-id="2fd38-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllConfiguredConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="2fd38-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="2fd38-135">acceptRequests</span></span> | <span data-ttu-id="2fd38-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fd38-136">Boolean</span></span> | <span data-ttu-id="2fd38-137">Указывает, принимаются ли новые запросы для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2fd38-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="2fd38-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="2fd38-138">allowedRequestors</span></span> | <span data-ttu-id="2fd38-139">[Коллекция userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="2fd38-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="2fd38-140">Пользователи, которым разрешено запрашивать эту политику, которые могут быть [singleUser,](singleuser.md) [groupMembers](groupmembers.md)и [connectedOrganizationMembers.](connectedorganizationmembers.md)</span><span class="sxs-lookup"><span data-stu-id="2fd38-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2fd38-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2fd38-141">JSON representation</span></span>


<span data-ttu-id="2fd38-142">Ниже приводится представление свойства **requestorSettings** политики в JSON, которое позволяет участникам группы запрашивать запросы.</span><span class="sxs-lookup"><span data-stu-id="2fd38-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
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


