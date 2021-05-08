---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b08284d99d88ffbfa38c950062986ba72da900d5
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231929"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="69205-103">тип ресурса authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="69205-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="69205-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69205-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69205-105">Представляет политику, которая может управлять Azure Active Directory параметров авторизации.</span><span class="sxs-lookup"><span data-stu-id="69205-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="69205-106">Это однотон, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="69205-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="69205-107">Методы</span><span class="sxs-lookup"><span data-stu-id="69205-107">Methods</span></span>

| <span data-ttu-id="69205-108">Метод</span><span class="sxs-lookup"><span data-stu-id="69205-108">Method</span></span>       | <span data-ttu-id="69205-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69205-109">Return Type</span></span> | <span data-ttu-id="69205-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69205-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="69205-111">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="69205-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="69205-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="69205-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="69205-113">Ознакомьтесь с объектом authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="69205-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="69205-114">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="69205-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="69205-115">Нет</span><span class="sxs-lookup"><span data-stu-id="69205-115">None</span></span> | <span data-ttu-id="69205-116">Обновление объекта authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="69205-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="69205-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="69205-117">Properties</span></span>  
| <span data-ttu-id="69205-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="69205-118">Property</span></span> | <span data-ttu-id="69205-119">Тип</span><span class="sxs-lookup"><span data-stu-id="69205-119">Type</span></span> | <span data-ttu-id="69205-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69205-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="69205-121">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="69205-121">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="69205-122">Логический</span><span class="sxs-lookup"><span data-stu-id="69205-122">Boolean</span></span>| <span data-ttu-id="69205-123">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="69205-123">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="69205-124">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="69205-124">allowedToUseSSPR</span></span>|<span data-ttu-id="69205-125">Логический</span><span class="sxs-lookup"><span data-stu-id="69205-125">Boolean</span></span>| <span data-ttu-id="69205-126">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="69205-126">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="69205-127">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="69205-127">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="69205-128">Логический</span><span class="sxs-lookup"><span data-stu-id="69205-128">Boolean</span></span>| <span data-ttu-id="69205-129">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="69205-129">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="69205-130">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="69205-130">allowInvitesFrom</span></span>|<span data-ttu-id="69205-131">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="69205-131">allowInvitesFrom</span></span>|<span data-ttu-id="69205-132">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="69205-132">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="69205-133">Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="69205-133">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="69205-134">`everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США.</span><span class="sxs-lookup"><span data-stu-id="69205-134">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="69205-135">Дополнительные сведения см. в [таблице ниже](#allowinvitesfrom-values).</span><span class="sxs-lookup"><span data-stu-id="69205-135">See more in the [table below](#allowinvitesfrom-values).</span></span> |
|<span data-ttu-id="69205-136">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="69205-136">blockMsolPowerShell</span></span>|<span data-ttu-id="69205-137">Логический</span><span class="sxs-lookup"><span data-stu-id="69205-137">Boolean</span></span>| <span data-ttu-id="69205-138">Чтобы отключить использование MSOL PowerShell, установите это свойство `true` .</span><span class="sxs-lookup"><span data-stu-id="69205-138">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="69205-139">Это также отключит доступ пользователей к конечной точке устаревшей службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="69205-139">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="69205-140">Это не влияет на azure AD Подключение Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69205-140">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="69205-141">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="69205-141">defaultUserRolePermissions</span></span>|[<span data-ttu-id="69205-142">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="69205-142">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="69205-143">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="69205-143">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="69205-144">description</span><span class="sxs-lookup"><span data-stu-id="69205-144">description</span></span>|<span data-ttu-id="69205-145">Строка</span><span class="sxs-lookup"><span data-stu-id="69205-145">String</span></span>| <span data-ttu-id="69205-146">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="69205-146">Description of this policy.</span></span>|
|<span data-ttu-id="69205-147">displayName</span><span class="sxs-lookup"><span data-stu-id="69205-147">displayName</span></span>|<span data-ttu-id="69205-148">Строка</span><span class="sxs-lookup"><span data-stu-id="69205-148">String</span></span>| <span data-ttu-id="69205-149">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="69205-149">Display name for this policy.</span></span> |    
|<span data-ttu-id="69205-150">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="69205-150">guestUserRoleId</span></span>|<span data-ttu-id="69205-151">Guid</span><span class="sxs-lookup"><span data-stu-id="69205-151">Guid</span></span>| <span data-ttu-id="69205-152">Представляет шаблон roleId для роли, которая должна быть предоставлена гостевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="69205-152">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="69205-153">В настоящее время поддерживаются следующие роли: User `a0b1b346-4d3e-4e8b-98f8-753987be4970` (), Guest User `10dae51f-b6af-4016-8d66-8c2a99b929b3` () и Restricted Guest User `2af84b1e-32c8-42b7-82bc-daa82404023b` ().</span><span class="sxs-lookup"><span data-stu-id="69205-153">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> |
|<span data-ttu-id="69205-154">id</span><span class="sxs-lookup"><span data-stu-id="69205-154">id</span></span>|<span data-ttu-id="69205-155">Строка</span><span class="sxs-lookup"><span data-stu-id="69205-155">String</span></span>| <span data-ttu-id="69205-156">ID политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="69205-156">ID of the authorization policy.</span></span> <span data-ttu-id="69205-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="69205-157">Required.</span></span> <span data-ttu-id="69205-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69205-158">Read-only.</span></span>| 

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="69205-159">allowInvitesFrom values</span><span class="sxs-lookup"><span data-stu-id="69205-159">allowInvitesFrom values</span></span>

|<span data-ttu-id="69205-160">Member</span><span class="sxs-lookup"><span data-stu-id="69205-160">Member</span></span>|<span data-ttu-id="69205-161">Описание</span><span class="sxs-lookup"><span data-stu-id="69205-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69205-162">нет</span><span class="sxs-lookup"><span data-stu-id="69205-162">none</span></span>|<span data-ttu-id="69205-163">Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="69205-163">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="69205-164">Параметр по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="69205-164">Default setting for US Government.</span></span>|
|<span data-ttu-id="69205-165">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="69205-165">adminsAndGuestInviters</span></span>|<span data-ttu-id="69205-166">Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="69205-166">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="69205-167">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="69205-167">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="69205-168">Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="69205-168">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="69205-169">все</span><span class="sxs-lookup"><span data-stu-id="69205-169">everyone</span></span>|<span data-ttu-id="69205-170">Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="69205-170">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="69205-171">Параметр по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="69205-171">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69205-172">Связи</span><span class="sxs-lookup"><span data-stu-id="69205-172">Relationships</span></span>

<span data-ttu-id="69205-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69205-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69205-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69205-174">JSON representation</span></span>

<span data-ttu-id="69205-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69205-175">The following is a JSON representation of the resource.</span></span>

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
  "allowInvitesFrom": "String",
  "guestUserRoleId": "Guid"
}
```
