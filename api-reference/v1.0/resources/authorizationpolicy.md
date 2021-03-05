---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ce482195ce7921eb43f2e4d1845a95f750688f1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448872"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="68c0c-103">тип ресурса authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="68c0c-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="68c0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68c0c-105">Представляет политику, которая может управлять настройками авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="68c0c-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="68c0c-106">Это однотон, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="68c0c-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="68c0c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="68c0c-107">Methods</span></span>

| <span data-ttu-id="68c0c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="68c0c-108">Method</span></span>       | <span data-ttu-id="68c0c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="68c0c-109">Return Type</span></span> | <span data-ttu-id="68c0c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="68c0c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="68c0c-111">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="68c0c-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="68c0c-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="68c0c-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="68c0c-113">Ознакомьтесь с объектом authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="68c0c-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="68c0c-114">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="68c0c-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="68c0c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="68c0c-115">None</span></span> | <span data-ttu-id="68c0c-116">Обновление объекта authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="68c0c-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="68c0c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="68c0c-117">Properties</span></span>  
| <span data-ttu-id="68c0c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="68c0c-118">Property</span></span> | <span data-ttu-id="68c0c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="68c0c-119">Type</span></span> | <span data-ttu-id="68c0c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="68c0c-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="68c0c-121">id</span><span class="sxs-lookup"><span data-stu-id="68c0c-121">id</span></span>|<span data-ttu-id="68c0c-122">String</span><span class="sxs-lookup"><span data-stu-id="68c0c-122">String</span></span>| <span data-ttu-id="68c0c-123">ID политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="68c0c-123">ID of the authorization policy.</span></span> <span data-ttu-id="68c0c-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="68c0c-124">Required.</span></span> <span data-ttu-id="68c0c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c0c-125">Read-only.</span></span>| 
|<span data-ttu-id="68c0c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="68c0c-126">displayName</span></span>|<span data-ttu-id="68c0c-127">String</span><span class="sxs-lookup"><span data-stu-id="68c0c-127">String</span></span>| <span data-ttu-id="68c0c-128">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="68c0c-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="68c0c-129">description</span><span class="sxs-lookup"><span data-stu-id="68c0c-129">description</span></span>|<span data-ttu-id="68c0c-130">String</span><span class="sxs-lookup"><span data-stu-id="68c0c-130">String</span></span>| <span data-ttu-id="68c0c-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="68c0c-131">Description of this policy.</span></span>|  
|<span data-ttu-id="68c0c-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="68c0c-132">blockMsolPowerShell</span></span>|<span data-ttu-id="68c0c-133">Логический</span><span class="sxs-lookup"><span data-stu-id="68c0c-133">Boolean</span></span>| <span data-ttu-id="68c0c-134">Чтобы отключить использование MSOL PowerShell, установите это свойство true.</span><span class="sxs-lookup"><span data-stu-id="68c0c-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="68c0c-135">Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="68c0c-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="68c0c-136">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="68c0c-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="68c0c-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="68c0c-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="68c0c-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="68c0c-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="68c0c-139">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="68c0c-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="68c0c-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="68c0c-140">allowedToUseSSPR</span></span>|<span data-ttu-id="68c0c-141">Логический</span><span class="sxs-lookup"><span data-stu-id="68c0c-141">Boolean</span></span>| <span data-ttu-id="68c0c-142">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="68c0c-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="68c0c-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="68c0c-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="68c0c-144">Логический</span><span class="sxs-lookup"><span data-stu-id="68c0c-144">Boolean</span></span>| <span data-ttu-id="68c0c-145">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="68c0c-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="68c0c-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="68c0c-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="68c0c-147">Логический</span><span class="sxs-lookup"><span data-stu-id="68c0c-147">Boolean</span></span>| <span data-ttu-id="68c0c-148">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="68c0c-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="68c0c-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="68c0c-149">allowInvitesFrom</span></span>|<span data-ttu-id="68c0c-150">String</span><span class="sxs-lookup"><span data-stu-id="68c0c-150">String</span></span>|<span data-ttu-id="68c0c-151">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="68c0c-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="68c0c-152">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="68c0c-152">Possible values are:</span></span><ul><li><span data-ttu-id="68c0c-153">`none` - Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="68c0c-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="68c0c-154">Параметр по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="68c0c-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="68c0c-155">`adminsAndGuestInviters` - Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="68c0c-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="68c0c-156">`adminsGuestInvitersAndAllMembers` - Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="68c0c-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="68c0c-157">`everyone` - Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="68c0c-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="68c0c-158">Параметр по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="68c0c-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="68c0c-159">Связи</span><span class="sxs-lookup"><span data-stu-id="68c0c-159">Relationships</span></span>

<span data-ttu-id="68c0c-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="68c0c-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68c0c-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="68c0c-161">JSON representation</span></span>

<span data-ttu-id="68c0c-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68c0c-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```
