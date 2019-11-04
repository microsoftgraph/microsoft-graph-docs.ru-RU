---
title: Тип ресурса Акцесспаккажесубжект
description: В службе управления обслуживанием Azure AD тема назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b37d91ad5669a0a87cef91893babf392f2f309b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939406"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="a09f6-103">Тип ресурса Акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="a09f6-103">accessPackageSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09f6-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)субъектом пакета Access является пользователь, участник службы или другой объект, который можно настроить для запроса или назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="a09f6-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="a09f6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a09f6-105">Properties</span></span>

| <span data-ttu-id="a09f6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a09f6-106">Property</span></span>     | <span data-ttu-id="a09f6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a09f6-107">Type</span></span>        | <span data-ttu-id="a09f6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a09f6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a09f6-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a09f6-109">displayName</span></span>|<span data-ttu-id="a09f6-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a09f6-110">String</span></span>|<span data-ttu-id="a09f6-111">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="a09f6-111">The display name of the subject.</span></span>|
|<span data-ttu-id="a09f6-112">email</span><span class="sxs-lookup"><span data-stu-id="a09f6-112">email</span></span>|<span data-ttu-id="a09f6-113">String</span><span class="sxs-lookup"><span data-stu-id="a09f6-113">String</span></span>|<span data-ttu-id="a09f6-114">Адрес электронной почты субъекта.</span><span class="sxs-lookup"><span data-stu-id="a09f6-114">The email address of the subject.</span></span>|
|<span data-ttu-id="a09f6-115">id</span><span class="sxs-lookup"><span data-stu-id="a09f6-115">id</span></span>|<span data-ttu-id="a09f6-116">String</span><span class="sxs-lookup"><span data-stu-id="a09f6-116">String</span></span>| <span data-ttu-id="a09f6-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a09f6-117">Read-only.</span></span>|
|<span data-ttu-id="a09f6-118">objectId</span><span class="sxs-lookup"><span data-stu-id="a09f6-118">objectId</span></span>|<span data-ttu-id="a09f6-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a09f6-119">String</span></span>|<span data-ttu-id="a09f6-120">Идентификатор объекта subject.</span><span class="sxs-lookup"><span data-stu-id="a09f6-120">The object ID of the subject.</span></span>|
|<span data-ttu-id="a09f6-121">principalName</span><span class="sxs-lookup"><span data-stu-id="a09f6-121">principalName</span></span>|<span data-ttu-id="a09f6-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a09f6-122">String</span></span>|<span data-ttu-id="a09f6-123">Имя участника (если оно известно) субъекта.</span><span class="sxs-lookup"><span data-stu-id="a09f6-123">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="a09f6-124">type</span><span class="sxs-lookup"><span data-stu-id="a09f6-124">type</span></span>|<span data-ttu-id="a09f6-125">String</span><span class="sxs-lookup"><span data-stu-id="a09f6-125">String</span></span>|<span data-ttu-id="a09f6-126">Тип ресурса субъекта.</span><span class="sxs-lookup"><span data-stu-id="a09f6-126">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a09f6-127">Связи</span><span class="sxs-lookup"><span data-stu-id="a09f6-127">Relationships</span></span>

<span data-ttu-id="a09f6-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a09f6-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a09f6-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a09f6-129">JSON representation</span></span>

<span data-ttu-id="a09f6-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a09f6-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "",
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
