---
title: Тип ресурса accessPackageSubject
description: В управлении правами Azure AD субъект назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f5bbd3147b27193d8a8e8a3e4bea3914719124c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161784"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="25dad-103">Тип ресурса accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="25dad-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="25dad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25dad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25dad-105">В управлении правами [Azure AD](entitlementmanagement-root.md)субъектом пакета доступа является пользователь, субъект-служба или другая сущность, которую можно настроить для запроса или получения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="25dad-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="25dad-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25dad-106">Properties</span></span>

| <span data-ttu-id="25dad-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25dad-107">Property</span></span>     | <span data-ttu-id="25dad-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25dad-108">Type</span></span>        | <span data-ttu-id="25dad-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25dad-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25dad-110">displayName</span><span class="sxs-lookup"><span data-stu-id="25dad-110">displayName</span></span>|<span data-ttu-id="25dad-111">String</span><span class="sxs-lookup"><span data-stu-id="25dad-111">String</span></span>|<span data-ttu-id="25dad-112">Отображаемого имени темы.</span><span class="sxs-lookup"><span data-stu-id="25dad-112">The display name of the subject.</span></span>|
|<span data-ttu-id="25dad-113">email</span><span class="sxs-lookup"><span data-stu-id="25dad-113">email</span></span>|<span data-ttu-id="25dad-114">String</span><span class="sxs-lookup"><span data-stu-id="25dad-114">String</span></span>|<span data-ttu-id="25dad-115">Адрес электронной почты темы.</span><span class="sxs-lookup"><span data-stu-id="25dad-115">The email address of the subject.</span></span>|
|<span data-ttu-id="25dad-116">id</span><span class="sxs-lookup"><span data-stu-id="25dad-116">id</span></span>|<span data-ttu-id="25dad-117">String</span><span class="sxs-lookup"><span data-stu-id="25dad-117">String</span></span>| <span data-ttu-id="25dad-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25dad-118">Read-only.</span></span>|
|<span data-ttu-id="25dad-119">objectId</span><span class="sxs-lookup"><span data-stu-id="25dad-119">objectId</span></span>|<span data-ttu-id="25dad-120">String</span><span class="sxs-lookup"><span data-stu-id="25dad-120">String</span></span>|<span data-ttu-id="25dad-121">ИД объекта темы.</span><span class="sxs-lookup"><span data-stu-id="25dad-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="25dad-122">principalName</span><span class="sxs-lookup"><span data-stu-id="25dad-122">principalName</span></span>|<span data-ttu-id="25dad-123">String</span><span class="sxs-lookup"><span data-stu-id="25dad-123">String</span></span>|<span data-ttu-id="25dad-124">Имя субъекта( если известно) темы.</span><span class="sxs-lookup"><span data-stu-id="25dad-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="25dad-125">type</span><span class="sxs-lookup"><span data-stu-id="25dad-125">type</span></span>|<span data-ttu-id="25dad-126">String</span><span class="sxs-lookup"><span data-stu-id="25dad-126">String</span></span>|<span data-ttu-id="25dad-127">Тип ресурса темы.</span><span class="sxs-lookup"><span data-stu-id="25dad-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25dad-128">Связи</span><span class="sxs-lookup"><span data-stu-id="25dad-128">Relationships</span></span>

<span data-ttu-id="25dad-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25dad-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25dad-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25dad-130">JSON representation</span></span>

<span data-ttu-id="25dad-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25dad-131">The following is a JSON representation of the resource.</span></span>

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


