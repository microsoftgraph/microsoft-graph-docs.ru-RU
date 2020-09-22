---
title: Тип ресурса Дефаултусерролепермиссионс
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ee3df9779d5c69ec35bdc4ac9d373554cb0728e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049949"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="de732-103">Тип ресурса Дефаултусерролепермиссионс</span><span class="sxs-lookup"><span data-stu-id="de732-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de732-104">Содержит некоторые настраиваемые разрешения роли пользователя по умолчанию в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de732-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="de732-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="de732-105">Properties</span></span>

| <span data-ttu-id="de732-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="de732-106">Property</span></span> | <span data-ttu-id="de732-107">Тип</span><span class="sxs-lookup"><span data-stu-id="de732-107">Type</span></span> | <span data-ttu-id="de732-108">Описание</span><span class="sxs-lookup"><span data-stu-id="de732-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="de732-109">алловедтокреатеаппс</span><span class="sxs-lookup"><span data-stu-id="de732-109">allowedToCreateApps</span></span> | <span data-ttu-id="de732-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="de732-110">Boolean</span></span> | <span data-ttu-id="de732-111">Указывает, может ли роль пользователя по умолчанию создавать приложения.</span><span class="sxs-lookup"><span data-stu-id="de732-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="de732-112">алловедтокреатесекуритиграупс</span><span class="sxs-lookup"><span data-stu-id="de732-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="de732-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="de732-113">Boolean</span></span> | <span data-ttu-id="de732-114">Указывает, может ли роль пользователя по умолчанию создавать группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="de732-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="de732-115">алловедтореадосерусерс</span><span class="sxs-lookup"><span data-stu-id="de732-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="de732-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="de732-116">Boolean</span></span> | <span data-ttu-id="de732-117">Указывает, может ли роль пользователя по умолчанию читать других пользователей.</span><span class="sxs-lookup"><span data-stu-id="de732-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="de732-118">Связи</span><span class="sxs-lookup"><span data-stu-id="de732-118">Relationships</span></span>

<span data-ttu-id="de732-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="de732-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de732-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="de732-120">JSON representation</span></span>

<span data-ttu-id="de732-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de732-121">The following is a JSON representation of the resource.</span></span>

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


