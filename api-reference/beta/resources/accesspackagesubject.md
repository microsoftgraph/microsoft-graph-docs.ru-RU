---
title: тип ресурсов accessPackageSubject
description: В управлении правами Azure AD субъект назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0adfca021ec463029a4b35c047ac85f8ce52921b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467066"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="ee7fc-103">тип ресурсов accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ee7fc-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="ee7fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee7fc-105">В управлении правами [Azure AD](entitlementmanagement-root.md)субъект пакета доступа — это пользователь, руководитель службы или другая сущность, которую можно настроить для запроса или присвоения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>  <span data-ttu-id="ee7fc-106">Он может представлять запросителя из связанной организации, который еще не находится в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-106">It may represent a requestor from a connected organization who is not yet in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="ee7fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee7fc-107">Properties</span></span>

| <span data-ttu-id="ee7fc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee7fc-108">Property</span></span>     | <span data-ttu-id="ee7fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7fc-109">Type</span></span>        | <span data-ttu-id="ee7fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7fc-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee7fc-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7fc-111">displayName</span></span>|<span data-ttu-id="ee7fc-112">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-112">String</span></span>|<span data-ttu-id="ee7fc-113">Отображение имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-113">The display name of the subject.</span></span>|
|<span data-ttu-id="ee7fc-114">email</span><span class="sxs-lookup"><span data-stu-id="ee7fc-114">email</span></span>|<span data-ttu-id="ee7fc-115">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-115">String</span></span>|<span data-ttu-id="ee7fc-116">Адрес электронной почты субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-116">The email address of the subject.</span></span>|
|<span data-ttu-id="ee7fc-117">id</span><span class="sxs-lookup"><span data-stu-id="ee7fc-117">id</span></span>|<span data-ttu-id="ee7fc-118">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-118">String</span></span>| <span data-ttu-id="ee7fc-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-119">Read-only.</span></span>|
|<span data-ttu-id="ee7fc-120">objectId</span><span class="sxs-lookup"><span data-stu-id="ee7fc-120">objectId</span></span>|<span data-ttu-id="ee7fc-121">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-121">String</span></span>|<span data-ttu-id="ee7fc-122">Идентификатор объекта субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-122">The object identifier of the subject.</span></span> <span data-ttu-id="ee7fc-123">`null` если субъект еще не является пользователем в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-123">`null` if the subject is not yet a user in the tenant.</span></span>|
|<span data-ttu-id="ee7fc-124">principalName</span><span class="sxs-lookup"><span data-stu-id="ee7fc-124">principalName</span></span>|<span data-ttu-id="ee7fc-125">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-125">String</span></span>|<span data-ttu-id="ee7fc-126">Основное имя, если известно, субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-126">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="ee7fc-127">type</span><span class="sxs-lookup"><span data-stu-id="ee7fc-127">type</span></span>|<span data-ttu-id="ee7fc-128">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-128">String</span></span>|<span data-ttu-id="ee7fc-129">Тип ресурса субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-129">The resource type of the subject.</span></span>|
|<span data-ttu-id="ee7fc-130">connectedOrganizationId</span><span class="sxs-lookup"><span data-stu-id="ee7fc-130">connectedOrganizationId</span></span>|<span data-ttu-id="ee7fc-131">String</span><span class="sxs-lookup"><span data-stu-id="ee7fc-131">String</span></span>|<span data-ttu-id="ee7fc-132">Идентификатор связанной организации субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-132">The identifier of the connected organization of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee7fc-133">Связи</span><span class="sxs-lookup"><span data-stu-id="ee7fc-133">Relationships</span></span>

| <span data-ttu-id="ee7fc-134">Связь</span><span class="sxs-lookup"><span data-stu-id="ee7fc-134">Relationship</span></span> | <span data-ttu-id="ee7fc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7fc-135">Type</span></span>        | <span data-ttu-id="ee7fc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7fc-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee7fc-137">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ee7fc-137">connectedOrganization</span></span>|[<span data-ttu-id="ee7fc-138">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ee7fc-138">connectedOrganization</span></span>](connectedorganization.md)| <span data-ttu-id="ee7fc-139">Подключенная организация субъекта.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-139">The connected organization of the subject.</span></span> <span data-ttu-id="ee7fc-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-140">Read-only.</span></span> <span data-ttu-id="ee7fc-141">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-141">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ee7fc-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee7fc-142">JSON representation</span></span>

<span data-ttu-id="ee7fc-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee7fc-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

