---
title: Тип ресурса Акцесспаккажесубжект
description: В службе управления обслуживанием Azure AD тема назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8b967e2ba2d678d9648b09eae4aeb3dca760c52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994346"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="4b178-103">Тип ресурса Акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="4b178-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="4b178-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b178-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b178-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)субъектом пакета Access является пользователь, участник службы или другой объект, который можно настроить для запроса или назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="4b178-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="4b178-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b178-106">Properties</span></span>

| <span data-ttu-id="4b178-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b178-107">Property</span></span>     | <span data-ttu-id="4b178-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4b178-108">Type</span></span>        | <span data-ttu-id="4b178-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b178-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b178-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4b178-110">displayName</span></span>|<span data-ttu-id="4b178-111">String</span><span class="sxs-lookup"><span data-stu-id="4b178-111">String</span></span>|<span data-ttu-id="4b178-112">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-112">The display name of the subject.</span></span>|
|<span data-ttu-id="4b178-113">email</span><span class="sxs-lookup"><span data-stu-id="4b178-113">email</span></span>|<span data-ttu-id="4b178-114">String</span><span class="sxs-lookup"><span data-stu-id="4b178-114">String</span></span>|<span data-ttu-id="4b178-115">Адрес электронной почты субъекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-115">The email address of the subject.</span></span>|
|<span data-ttu-id="4b178-116">id</span><span class="sxs-lookup"><span data-stu-id="4b178-116">id</span></span>|<span data-ttu-id="4b178-117">String</span><span class="sxs-lookup"><span data-stu-id="4b178-117">String</span></span>| <span data-ttu-id="4b178-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b178-118">Read-only.</span></span>|
|<span data-ttu-id="4b178-119">objectId</span><span class="sxs-lookup"><span data-stu-id="4b178-119">objectId</span></span>|<span data-ttu-id="4b178-120">String</span><span class="sxs-lookup"><span data-stu-id="4b178-120">String</span></span>|<span data-ttu-id="4b178-121">Идентификатор объекта subject.</span><span class="sxs-lookup"><span data-stu-id="4b178-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="4b178-122">principalName</span><span class="sxs-lookup"><span data-stu-id="4b178-122">principalName</span></span>|<span data-ttu-id="4b178-123">String</span><span class="sxs-lookup"><span data-stu-id="4b178-123">String</span></span>|<span data-ttu-id="4b178-124">Имя участника (если оно известно) субъекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="4b178-125">type</span><span class="sxs-lookup"><span data-stu-id="4b178-125">type</span></span>|<span data-ttu-id="4b178-126">String</span><span class="sxs-lookup"><span data-stu-id="4b178-126">String</span></span>|<span data-ttu-id="4b178-127">Тип ресурса субъекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b178-128">Связи</span><span class="sxs-lookup"><span data-stu-id="4b178-128">Relationships</span></span>

<span data-ttu-id="4b178-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4b178-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b178-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b178-130">JSON representation</span></span>

<span data-ttu-id="4b178-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b178-131">The following is a JSON representation of the resource.</span></span>

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


