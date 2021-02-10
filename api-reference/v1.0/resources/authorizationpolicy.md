---
title: Тип ресурса authorizationPolicy
description: Представляет политику, которая может управлять настройками авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 12fe4ad670d2bb5056d05fde533d4b690068f7a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154217"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="a7ead-103">Тип ресурса authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a7ead-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="a7ead-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7ead-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a7ead-105">Представляет политику, которая может управлять настройками авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a7ead-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="a7ead-106">Это однотон, наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7ead-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="a7ead-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a7ead-107">Methods</span></span>

| <span data-ttu-id="a7ead-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a7ead-108">Method</span></span>       | <span data-ttu-id="a7ead-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7ead-109">Return Type</span></span> | <span data-ttu-id="a7ead-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ead-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a7ead-111">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a7ead-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="a7ead-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a7ead-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="a7ead-113">Чтение объекта authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="a7ead-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="a7ead-114">Обновление authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a7ead-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="a7ead-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a7ead-115">None</span></span> | <span data-ttu-id="a7ead-116">Обновление объекта authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="a7ead-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a7ead-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7ead-117">Properties</span></span>  
| <span data-ttu-id="a7ead-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7ead-118">Property</span></span> | <span data-ttu-id="a7ead-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a7ead-119">Type</span></span> | <span data-ttu-id="a7ead-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ead-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="a7ead-121">id</span><span class="sxs-lookup"><span data-stu-id="a7ead-121">id</span></span>|<span data-ttu-id="a7ead-122">String</span><span class="sxs-lookup"><span data-stu-id="a7ead-122">String</span></span>| <span data-ttu-id="a7ead-123">ИД политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="a7ead-123">ID of the authorization policy.</span></span> <span data-ttu-id="a7ead-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a7ead-124">Required.</span></span> <span data-ttu-id="a7ead-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7ead-125">Read-only.</span></span>| 
|<span data-ttu-id="a7ead-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a7ead-126">displayName</span></span>|<span data-ttu-id="a7ead-127">String</span><span class="sxs-lookup"><span data-stu-id="a7ead-127">String</span></span>| <span data-ttu-id="a7ead-128">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a7ead-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="a7ead-129">description</span><span class="sxs-lookup"><span data-stu-id="a7ead-129">description</span></span>|<span data-ttu-id="a7ead-130">String</span><span class="sxs-lookup"><span data-stu-id="a7ead-130">String</span></span>| <span data-ttu-id="a7ead-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="a7ead-131">Description of this policy.</span></span>|  
|<span data-ttu-id="a7ead-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="a7ead-132">blockMsolPowerShell</span></span>|<span data-ttu-id="a7ead-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="a7ead-133">Boolean</span></span>| <span data-ttu-id="a7ead-134">Чтобы отключить использование MSOL PowerShell, установите для этого свойства true.</span><span class="sxs-lookup"><span data-stu-id="a7ead-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="a7ead-135">При установке true также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a7ead-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="a7ead-136">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a7ead-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="a7ead-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a7ead-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="a7ead-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a7ead-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="a7ead-139">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a7ead-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="a7ead-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="a7ead-140">allowedToUseSSPR</span></span>|<span data-ttu-id="a7ead-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="a7ead-141">Boolean</span></span>| <span data-ttu-id="a7ead-142">Указывает, может ли функция Self-Serve сброса пароля может использоваться пользователями в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a7ead-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="a7ead-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="a7ead-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="a7ead-144">Логическое</span><span class="sxs-lookup"><span data-stu-id="a7ead-144">Boolean</span></span>| <span data-ttu-id="a7ead-145">Указывает, могут ли пользователи зарегистрироваться для подписок на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a7ead-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="a7ead-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="a7ead-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="a7ead-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="a7ead-147">Boolean</span></span>| <span data-ttu-id="a7ead-148">Указывает, может ли пользователь присоединиться к клиенту по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="a7ead-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="a7ead-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="a7ead-149">allowInvitesFrom</span></span>|<span data-ttu-id="a7ead-150">String</span><span class="sxs-lookup"><span data-stu-id="a7ead-150">String</span></span>|<span data-ttu-id="a7ead-151">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="a7ead-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="a7ead-152">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="a7ead-152">Possible values are:</span></span><ul><li><span data-ttu-id="a7ead-153">`none` – Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7ead-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="a7ead-154">Настройка по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="a7ead-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="a7ead-155">`adminsAndGuestInviters` - Разрешить участникам ролей глобальных администраторов, администраторов пользователей и приглашений гостей приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7ead-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="a7ead-156">`adminsGuestInvitersAndAllMembers` - Разрешить вышеуказанным ролям администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7ead-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="a7ead-157">`everyone` - Разрешить всем пользователям в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7ead-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="a7ead-158">Значение по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="a7ead-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="a7ead-159">Связи</span><span class="sxs-lookup"><span data-stu-id="a7ead-159">Relationships</span></span>

<span data-ttu-id="a7ead-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a7ead-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7ead-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a7ead-161">JSON representation</span></span>

<span data-ttu-id="a7ead-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7ead-162">The following is a JSON representation of the resource.</span></span>

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
