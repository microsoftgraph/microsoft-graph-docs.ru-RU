---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20b7d1f9813873bb7233a8e3c8c35fe88e1c460c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364315"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="c7faa-103">Тип ресурса Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="c7faa-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="c7faa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7faa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7faa-105">Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c7faa-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="c7faa-106">Это одноэлементный экземпляр, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7faa-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="c7faa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c7faa-107">Methods</span></span>

| <span data-ttu-id="c7faa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c7faa-108">Method</span></span>       | <span data-ttu-id="c7faa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7faa-109">Return Type</span></span> | <span data-ttu-id="c7faa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7faa-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c7faa-111">Получение Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="c7faa-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="c7faa-112">аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="c7faa-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="c7faa-113">Чтение объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="c7faa-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="c7faa-114">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="c7faa-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="c7faa-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c7faa-115">None</span></span> | <span data-ttu-id="c7faa-116">Обновление объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="c7faa-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c7faa-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7faa-117">Properties</span></span>  
| <span data-ttu-id="c7faa-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7faa-118">Property</span></span> | <span data-ttu-id="c7faa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c7faa-119">Type</span></span> | <span data-ttu-id="c7faa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7faa-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="c7faa-121">id</span><span class="sxs-lookup"><span data-stu-id="c7faa-121">id</span></span>|<span data-ttu-id="c7faa-122">String</span><span class="sxs-lookup"><span data-stu-id="c7faa-122">String</span></span>| <span data-ttu-id="c7faa-123">Идентификатор политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="c7faa-123">ID of the authorization policy.</span></span> <span data-ttu-id="c7faa-124">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c7faa-124">Required.</span></span> <span data-ttu-id="c7faa-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7faa-125">Read-only.</span></span>| 
|<span data-ttu-id="c7faa-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c7faa-126">displayName</span></span>|<span data-ttu-id="c7faa-127">String</span><span class="sxs-lookup"><span data-stu-id="c7faa-127">String</span></span>| <span data-ttu-id="c7faa-128">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7faa-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="c7faa-129">description</span><span class="sxs-lookup"><span data-stu-id="c7faa-129">description</span></span>|<span data-ttu-id="c7faa-130">String</span><span class="sxs-lookup"><span data-stu-id="c7faa-130">String</span></span>| <span data-ttu-id="c7faa-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7faa-131">Description of this policy.</span></span>|  
|<span data-ttu-id="c7faa-132">гуестусерролеид</span><span class="sxs-lookup"><span data-stu-id="c7faa-132">guestUserRoleId</span></span>|<span data-ttu-id="c7faa-133">Guid</span><span class="sxs-lookup"><span data-stu-id="c7faa-133">Guid</span></span>| <span data-ttu-id="c7faa-134">Представляет templateId роли для роли, которая должна быть выделена пользователю "гость".</span><span class="sxs-lookup"><span data-stu-id="c7faa-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="c7faa-135">Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей.</span><span class="sxs-lookup"><span data-stu-id="c7faa-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="c7faa-136">В настоящее время поддерживаются следующие роли: пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и незащищенный гостевой пользователь (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="c7faa-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="c7faa-137">енабледпревиевфеатурес</span><span class="sxs-lookup"><span data-stu-id="c7faa-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="c7faa-138">Коллекция (String)</span><span class="sxs-lookup"><span data-stu-id="c7faa-138">Collection(string)</span></span>| <span data-ttu-id="c7faa-139">Список компонентов, включенных для закрытой предварительной версии в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c7faa-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="c7faa-140">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="c7faa-140">blockMsolPowerShell</span></span>|<span data-ttu-id="c7faa-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7faa-141">Boolean</span></span>| <span data-ttu-id="c7faa-142">Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true.</span><span class="sxs-lookup"><span data-stu-id="c7faa-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="c7faa-143">Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c7faa-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="c7faa-144">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c7faa-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="c7faa-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="c7faa-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="c7faa-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="c7faa-146">defaultUserRolePermissions</span></span>](defaultUserRolePermissions.md)| <span data-ttu-id="c7faa-147">Задает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c7faa-147">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="c7faa-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="c7faa-148">allowedToUseSSPR</span></span>|<span data-ttu-id="c7faa-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7faa-149">Boolean</span></span>| <span data-ttu-id="c7faa-150">Указывает, можно ли использовать функцию самостоятельного сброса пароля для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="c7faa-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="c7faa-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="c7faa-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="c7faa-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7faa-152">Boolean</span></span>| <span data-ttu-id="c7faa-153">Указывает, могут ли пользователи регистрироваться на почтовые подписки.</span><span class="sxs-lookup"><span data-stu-id="c7faa-153">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="c7faa-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="c7faa-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="c7faa-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7faa-155">Boolean</span></span>| <span data-ttu-id="c7faa-156">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c7faa-156">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="c7faa-157">алловинвитесфром</span><span class="sxs-lookup"><span data-stu-id="c7faa-157">allowInvitesFrom</span></span>|<span data-ttu-id="c7faa-158">String</span><span class="sxs-lookup"><span data-stu-id="c7faa-158">String</span></span>|<span data-ttu-id="c7faa-159">Указывает, кто может приглашать внешних пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="c7faa-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="c7faa-160">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="c7faa-160">Possible values are:</span></span><br/><span data-ttu-id="c7faa-161">`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7faa-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="c7faa-162">Настройка по умолчанию для государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="c7faa-162">Default setting for US Government.</span></span><br/><span data-ttu-id="c7faa-163">`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7faa-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span><br/><span data-ttu-id="c7faa-164">`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7faa-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span><br/><span data-ttu-id="c7faa-165">`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7faa-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="c7faa-166">Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="c7faa-166">Default setting for all cloud environments except US Government.</span></span><br/><span data-ttu-id="c7faa-167">`unknownFutureValue` заполнитель для перечислений расширяемые.</span><span class="sxs-lookup"><span data-stu-id="c7faa-167">`unknownFutureValue` - placeholder for evolvable enums.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7faa-168">Связи</span><span class="sxs-lookup"><span data-stu-id="c7faa-168">Relationships</span></span>
<span data-ttu-id="c7faa-169">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c7faa-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7faa-170">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7faa-170">JSON representation</span></span>

<span data-ttu-id="c7faa-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7faa-171">The following is a JSON representation of the resource.</span></span>

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
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```


