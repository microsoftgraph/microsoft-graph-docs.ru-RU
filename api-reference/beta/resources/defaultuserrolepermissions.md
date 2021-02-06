---
title: Тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6ee2e8deccf73929b68079379efb0f6d93a3369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135676"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="f608a-103">Тип ресурса defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="f608a-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f608a-104">Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f608a-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="f608a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f608a-105">Properties</span></span>

| <span data-ttu-id="f608a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f608a-106">Property</span></span> | <span data-ttu-id="f608a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f608a-107">Type</span></span> | <span data-ttu-id="f608a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f608a-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="f608a-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="f608a-109">allowedToCreateApps</span></span> | <span data-ttu-id="f608a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="f608a-110">Boolean</span></span> | <span data-ttu-id="f608a-111">Указывает, может ли роль пользователя по умолчанию создавать приложения.</span><span class="sxs-lookup"><span data-stu-id="f608a-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="f608a-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="f608a-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="f608a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="f608a-113">Boolean</span></span> | <span data-ttu-id="f608a-114">Указывает, может ли роль пользователя по умолчанию создавать группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="f608a-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="f608a-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="f608a-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="f608a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="f608a-116">Boolean</span></span> | <span data-ttu-id="f608a-117">Указывает, может ли роль пользователя по умолчанию читать других пользователей.</span><span class="sxs-lookup"><span data-stu-id="f608a-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="f608a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f608a-118">Relationships</span></span>

<span data-ttu-id="f608a-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f608a-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f608a-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f608a-120">JSON representation</span></span>

<span data-ttu-id="f608a-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f608a-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


