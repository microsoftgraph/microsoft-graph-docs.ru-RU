---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71e4d01ba54c9043ff827b3749be63442d06ac
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581250"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="696a0-103">Тип ресурса Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="696a0-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="696a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="696a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="696a0-105">Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="696a0-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="696a0-106">Это одноэлементный экземпляр, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="696a0-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="696a0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="696a0-107">Methods</span></span>

| <span data-ttu-id="696a0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="696a0-108">Method</span></span>       | <span data-ttu-id="696a0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="696a0-109">Return Type</span></span> | <span data-ttu-id="696a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="696a0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="696a0-111">Получение Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="696a0-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="696a0-112">аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="696a0-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="696a0-113">Чтение объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="696a0-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="696a0-114">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="696a0-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="696a0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="696a0-115">None</span></span> | <span data-ttu-id="696a0-116">Обновление объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="696a0-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="696a0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="696a0-117">Properties</span></span>  
| <span data-ttu-id="696a0-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="696a0-118">Property</span></span> | <span data-ttu-id="696a0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="696a0-119">Type</span></span> | <span data-ttu-id="696a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="696a0-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="696a0-121">id</span><span class="sxs-lookup"><span data-stu-id="696a0-121">id</span></span>|<span data-ttu-id="696a0-122">String</span><span class="sxs-lookup"><span data-stu-id="696a0-122">String</span></span>| <span data-ttu-id="696a0-123">Идентификатор политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="696a0-123">ID of the authorization policy.</span></span> <span data-ttu-id="696a0-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="696a0-124">Required.</span></span> <span data-ttu-id="696a0-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696a0-125">Read-only.</span></span>| 
|<span data-ttu-id="696a0-126">displayName</span><span class="sxs-lookup"><span data-stu-id="696a0-126">displayName</span></span>|<span data-ttu-id="696a0-127">String</span><span class="sxs-lookup"><span data-stu-id="696a0-127">String</span></span>| <span data-ttu-id="696a0-128">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="696a0-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="696a0-129">description</span><span class="sxs-lookup"><span data-stu-id="696a0-129">description</span></span>|<span data-ttu-id="696a0-130">String</span><span class="sxs-lookup"><span data-stu-id="696a0-130">String</span></span>| <span data-ttu-id="696a0-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="696a0-131">Description of this policy.</span></span>|  
|<span data-ttu-id="696a0-132">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="696a0-132">blockMsolPowerShell</span></span>|<span data-ttu-id="696a0-133">Логический</span><span class="sxs-lookup"><span data-stu-id="696a0-133">Boolean</span></span>| <span data-ttu-id="696a0-134">Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true.</span><span class="sxs-lookup"><span data-stu-id="696a0-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="696a0-135">Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="696a0-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="696a0-136">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="696a0-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="696a0-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="696a0-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="696a0-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="696a0-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="696a0-139">Задает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="696a0-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="696a0-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="696a0-140">allowedToUseSSPR</span></span>|<span data-ttu-id="696a0-141">Логический</span><span class="sxs-lookup"><span data-stu-id="696a0-141">Boolean</span></span>| <span data-ttu-id="696a0-142">Указывает, может ли функция сброса пароля Self-Serve использоваться пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="696a0-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="696a0-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="696a0-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="696a0-144">Логический</span><span class="sxs-lookup"><span data-stu-id="696a0-144">Boolean</span></span>| <span data-ttu-id="696a0-145">Указывает, могут ли пользователи регистрироваться на почтовые подписки.</span><span class="sxs-lookup"><span data-stu-id="696a0-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="696a0-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="696a0-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="696a0-147">Логический</span><span class="sxs-lookup"><span data-stu-id="696a0-147">Boolean</span></span>| <span data-ttu-id="696a0-148">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="696a0-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="696a0-149">алловинвитесфром</span><span class="sxs-lookup"><span data-stu-id="696a0-149">allowInvitesFrom</span></span>|<span data-ttu-id="696a0-150">String</span><span class="sxs-lookup"><span data-stu-id="696a0-150">String</span></span>|<span data-ttu-id="696a0-151">Указывает, кто может приглашать внешних пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="696a0-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="696a0-152">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="696a0-152">Possible values are:</span></span><ul><li><span data-ttu-id="696a0-153">`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="696a0-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="696a0-154">Настройка по умолчанию для государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="696a0-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="696a0-155">`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="696a0-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="696a0-156">`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="696a0-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="696a0-157">`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="696a0-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="696a0-158">Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="696a0-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="696a0-159">Связи</span><span class="sxs-lookup"><span data-stu-id="696a0-159">Relationships</span></span>

<span data-ttu-id="696a0-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="696a0-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="696a0-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="696a0-161">JSON representation</span></span>

<span data-ttu-id="696a0-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="696a0-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
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
