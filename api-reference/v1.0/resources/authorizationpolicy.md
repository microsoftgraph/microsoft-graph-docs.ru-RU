---
title: тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 85af4636f52e49717e864f2ccb9d710fea313eb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962520"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="0271b-103">тип ресурса authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0271b-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="0271b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0271b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0271b-105">Представляет политику, которая может управлять настройками авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0271b-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="0271b-106">Это однотон, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="0271b-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="0271b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0271b-107">Methods</span></span>

| <span data-ttu-id="0271b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0271b-108">Method</span></span>       | <span data-ttu-id="0271b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0271b-109">Return Type</span></span> | <span data-ttu-id="0271b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0271b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0271b-111">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0271b-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="0271b-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0271b-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="0271b-113">Ознакомьтесь с объектом authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="0271b-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="0271b-114">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="0271b-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="0271b-115">Нет</span><span class="sxs-lookup"><span data-stu-id="0271b-115">None</span></span> | <span data-ttu-id="0271b-116">Обновление объекта authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="0271b-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0271b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0271b-117">Properties</span></span>  
| <span data-ttu-id="0271b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0271b-118">Property</span></span> | <span data-ttu-id="0271b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0271b-119">Type</span></span> | <span data-ttu-id="0271b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0271b-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="0271b-121">id</span><span class="sxs-lookup"><span data-stu-id="0271b-121">id</span></span>|<span data-ttu-id="0271b-122">String</span><span class="sxs-lookup"><span data-stu-id="0271b-122">String</span></span>| <span data-ttu-id="0271b-123">ID политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="0271b-123">ID of the authorization policy.</span></span> <span data-ttu-id="0271b-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0271b-124">Required.</span></span> <span data-ttu-id="0271b-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0271b-125">Read-only.</span></span>| 
|<span data-ttu-id="0271b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="0271b-126">displayName</span></span>|<span data-ttu-id="0271b-127">String</span><span class="sxs-lookup"><span data-stu-id="0271b-127">String</span></span>| <span data-ttu-id="0271b-128">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0271b-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="0271b-129">description</span><span class="sxs-lookup"><span data-stu-id="0271b-129">description</span></span>|<span data-ttu-id="0271b-130">String</span><span class="sxs-lookup"><span data-stu-id="0271b-130">String</span></span>| <span data-ttu-id="0271b-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="0271b-131">Description of this policy.</span></span>|  
|<span data-ttu-id="0271b-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="0271b-132">blockMsolPowerShell</span></span>|<span data-ttu-id="0271b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271b-133">Boolean</span></span>| <span data-ttu-id="0271b-134">Чтобы отключить использование MSOL PowerShell, установите это свойство true.</span><span class="sxs-lookup"><span data-stu-id="0271b-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="0271b-135">Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0271b-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="0271b-136">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0271b-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="0271b-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="0271b-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="0271b-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="0271b-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="0271b-139">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0271b-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="0271b-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="0271b-140">allowedToUseSSPR</span></span>|<span data-ttu-id="0271b-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271b-141">Boolean</span></span>| <span data-ttu-id="0271b-142">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="0271b-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="0271b-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="0271b-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="0271b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271b-144">Boolean</span></span>| <span data-ttu-id="0271b-145">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0271b-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="0271b-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="0271b-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="0271b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0271b-147">Boolean</span></span>| <span data-ttu-id="0271b-148">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0271b-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="0271b-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="0271b-149">allowInvitesFrom</span></span>|<span data-ttu-id="0271b-150">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="0271b-150">allowInvitesFrom</span></span>|<span data-ttu-id="0271b-151">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="0271b-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="0271b-152">Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="0271b-152">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="0271b-153">`everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США.</span><span class="sxs-lookup"><span data-stu-id="0271b-153">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="0271b-154">Подробнее в таблице [ниже](#allowinvitesfrom-values).</span><span class="sxs-lookup"><span data-stu-id="0271b-154">See more in the [table below](#allowinvitesfrom-values).</span></span> |

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="0271b-155">allowInvitesFrom values</span><span class="sxs-lookup"><span data-stu-id="0271b-155">allowInvitesFrom values</span></span>

|<span data-ttu-id="0271b-156">Member</span><span class="sxs-lookup"><span data-stu-id="0271b-156">Member</span></span>|<span data-ttu-id="0271b-157">Описание</span><span class="sxs-lookup"><span data-stu-id="0271b-157">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0271b-158">Нет</span><span class="sxs-lookup"><span data-stu-id="0271b-158">none</span></span>|<span data-ttu-id="0271b-159">Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0271b-159">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="0271b-160">Параметр по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="0271b-160">Default setting for US Government.</span></span>|
|<span data-ttu-id="0271b-161">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="0271b-161">adminsAndGuestInviters</span></span>|<span data-ttu-id="0271b-162">Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0271b-162">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="0271b-163">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="0271b-163">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="0271b-164">Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0271b-164">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="0271b-165">все</span><span class="sxs-lookup"><span data-stu-id="0271b-165">everyone</span></span>|<span data-ttu-id="0271b-166">Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0271b-166">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="0271b-167">Параметр по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="0271b-167">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0271b-168">Связи</span><span class="sxs-lookup"><span data-stu-id="0271b-168">Relationships</span></span>

<span data-ttu-id="0271b-169">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0271b-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0271b-170">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0271b-170">JSON representation</span></span>

<span data-ttu-id="0271b-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0271b-171">The following is a JSON representation of the resource.</span></span>

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
