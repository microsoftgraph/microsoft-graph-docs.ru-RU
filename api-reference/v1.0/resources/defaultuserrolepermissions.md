---
title: Тип ресурса defaultUserRolePermissions
description: Содержит определенные настраиваемые разрешения для роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e89f175a62615efe172646613897222a9ae75fa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137559"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="737de-103">Тип ресурса defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="737de-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="737de-104">Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="737de-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="737de-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="737de-105">Properties</span></span>

| <span data-ttu-id="737de-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="737de-106">Property</span></span> | <span data-ttu-id="737de-107">Тип</span><span class="sxs-lookup"><span data-stu-id="737de-107">Type</span></span> | <span data-ttu-id="737de-108">Описание</span><span class="sxs-lookup"><span data-stu-id="737de-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="737de-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="737de-109">allowedToCreateApps</span></span> | <span data-ttu-id="737de-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="737de-110">Boolean</span></span> | <span data-ttu-id="737de-111">Указывает, может ли роль пользователя по умолчанию создавать приложения.</span><span class="sxs-lookup"><span data-stu-id="737de-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="737de-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="737de-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="737de-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="737de-113">Boolean</span></span> | <span data-ttu-id="737de-114">Указывает, может ли роль пользователя по умолчанию создавать группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="737de-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="737de-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="737de-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="737de-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="737de-116">Boolean</span></span> | <span data-ttu-id="737de-117">Указывает, может ли роль пользователя по умолчанию читать других пользователей.</span><span class="sxs-lookup"><span data-stu-id="737de-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="737de-118">permissionGrantPoliciesAssigned</span><span class="sxs-lookup"><span data-stu-id="737de-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="737de-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="737de-119">String collection</span></span>|<span data-ttu-id="737de-120">Указывает, разрешено ли согласие пользователя на доступ к приложениям, и, если да, какое разрешение на предоставление согласия и какая политика согласия приложения (permissionGrantPolicy) управляет разрешением пользователей на предоставление согласия.</span><span class="sxs-lookup"><span data-stu-id="737de-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="737de-121">Значение должно быть в `managePermissionGrantsForSelf.{id}` формате, где находится `{id}` **ид** встроенной или настраиваемой политики согласия [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies)</span><span class="sxs-lookup"><span data-stu-id="737de-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="737de-122">Пустой список указывает, что согласие пользователя на приложения отключено.</span><span class="sxs-lookup"><span data-stu-id="737de-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="737de-123">Связи</span><span class="sxs-lookup"><span data-stu-id="737de-123">Relationships</span></span>

<span data-ttu-id="737de-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="737de-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="737de-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="737de-125">JSON representation</span></span>

<span data-ttu-id="737de-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="737de-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
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
