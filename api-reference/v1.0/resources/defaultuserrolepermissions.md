---
title: Тип ресурса Дефаултусерролепермиссионс
description: Содержит определенные настраиваемые разрешения роли пользователя по умолчанию.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581245"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="7f6a1-103">Тип ресурса Дефаултусерролепермиссионс</span><span class="sxs-lookup"><span data-stu-id="7f6a1-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="7f6a1-104">Содержит определенные настраиваемые разрешения роли пользователя по умолчанию в Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="7f6a1-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="7f6a1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f6a1-105">Properties</span></span>

| <span data-ttu-id="7f6a1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f6a1-106">Property</span></span> | <span data-ttu-id="7f6a1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7f6a1-107">Type</span></span> | <span data-ttu-id="7f6a1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7f6a1-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="7f6a1-109">алловедтокреатеаппс</span><span class="sxs-lookup"><span data-stu-id="7f6a1-109">allowedToCreateApps</span></span> | <span data-ttu-id="7f6a1-110">Логический</span><span class="sxs-lookup"><span data-stu-id="7f6a1-110">Boolean</span></span> | <span data-ttu-id="7f6a1-111">Указывает, может ли роль пользователя по умолчанию создавать приложения.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="7f6a1-112">алловедтокреатесекуритиграупс</span><span class="sxs-lookup"><span data-stu-id="7f6a1-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="7f6a1-113">Логический</span><span class="sxs-lookup"><span data-stu-id="7f6a1-113">Boolean</span></span> | <span data-ttu-id="7f6a1-114">Указывает, может ли роль пользователя по умолчанию создавать группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="7f6a1-115">алловедтореадосерусерс</span><span class="sxs-lookup"><span data-stu-id="7f6a1-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="7f6a1-116">Логический</span><span class="sxs-lookup"><span data-stu-id="7f6a1-116">Boolean</span></span> | <span data-ttu-id="7f6a1-117">Указывает, может ли роль пользователя по умолчанию читать других пользователей.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="7f6a1-118">пермиссионгрантполиЦиесассигнед</span><span class="sxs-lookup"><span data-stu-id="7f6a1-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="7f6a1-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7f6a1-119">String collection</span></span>|<span data-ttu-id="7f6a1-120">Указывает, разрешено ли согласие пользователя на приложения, и, если это так, какое разрешение на предоставление согласия и какая политика согласия приложения (Пермиссионгрантполици) управляет разрешением на предоставление разрешений для пользователей.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="7f6a1-121">Значение должно быть в формате `managePermissionGrantsForSelf.{id}` , где `{id}` — это **идентификатор** встроенной или настраиваемой [политики согласия приложения](/azure/active-directory/manage-apps/manage-app-consent-policies).</span><span class="sxs-lookup"><span data-stu-id="7f6a1-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="7f6a1-122">Пустой список указывает на то, что согласие пользователя на приложения отключено.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7f6a1-123">Связи</span><span class="sxs-lookup"><span data-stu-id="7f6a1-123">Relationships</span></span>

<span data-ttu-id="7f6a1-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f6a1-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7f6a1-125">JSON representation</span></span>

<span data-ttu-id="7f6a1-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f6a1-126">The following is a JSON representation of the resource.</span></span>

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
