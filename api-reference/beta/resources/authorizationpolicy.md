---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c20f4dad0263e9d4c931e43da99870ed022f1e58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492232"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="cd4f3-103">Тип ресурса Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="cd4f3-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="cd4f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd4f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd4f3-105">Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="cd4f3-106">Это одноэлементный экземпляр, который наследуется от базового типа политики и всегда существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="cd4f3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cd4f3-107">Methods</span></span>

| <span data-ttu-id="cd4f3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cd4f3-108">Method</span></span>       | <span data-ttu-id="cd4f3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd4f3-109">Return Type</span></span> | <span data-ttu-id="cd4f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4f3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cd4f3-111">Получение Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="cd4f3-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="cd4f3-112">аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="cd4f3-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="cd4f3-113">Чтение объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="cd4f3-114">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="cd4f3-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="cd4f3-115">Нет</span><span class="sxs-lookup"><span data-stu-id="cd4f3-115">None</span></span> | <span data-ttu-id="cd4f3-116">Обновление объекта Аусоризатионполици.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cd4f3-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd4f3-117">Properties</span></span>  
| <span data-ttu-id="cd4f3-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd4f3-118">Property</span></span> | <span data-ttu-id="cd4f3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cd4f3-119">Type</span></span> | <span data-ttu-id="cd4f3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4f3-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="cd4f3-121">id</span><span class="sxs-lookup"><span data-stu-id="cd4f3-121">id</span></span>|<span data-ttu-id="cd4f3-122">String</span><span class="sxs-lookup"><span data-stu-id="cd4f3-122">String</span></span>| <span data-ttu-id="cd4f3-123">Идентификатор политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-123">ID of the authorization policy.</span></span> <span data-ttu-id="cd4f3-124">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-124">Required.</span></span> <span data-ttu-id="cd4f3-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-125">Read-only.</span></span>| 
|<span data-ttu-id="cd4f3-126">displayName</span><span class="sxs-lookup"><span data-stu-id="cd4f3-126">displayName</span></span>|<span data-ttu-id="cd4f3-127">Строка</span><span class="sxs-lookup"><span data-stu-id="cd4f3-127">String</span></span>| <span data-ttu-id="cd4f3-128">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="cd4f3-129">description</span><span class="sxs-lookup"><span data-stu-id="cd4f3-129">description</span></span>|<span data-ttu-id="cd4f3-130">String</span><span class="sxs-lookup"><span data-stu-id="cd4f3-130">String</span></span>| <span data-ttu-id="cd4f3-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-131">Description of this policy.</span></span>|  
|<span data-ttu-id="cd4f3-132">гуестусерролеид</span><span class="sxs-lookup"><span data-stu-id="cd4f3-132">guestUserRoleId</span></span>|<span data-ttu-id="cd4f3-133">Guid</span><span class="sxs-lookup"><span data-stu-id="cd4f3-133">Guid</span></span>| <span data-ttu-id="cd4f3-134">Представляет templateId роли для роли, которая должна быть выделена пользователю "гость".</span><span class="sxs-lookup"><span data-stu-id="cd4f3-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="cd4f3-135">Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="cd4f3-136">В настоящее время поддерживаются следующие роли: пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и незащищенный гостевой пользователь (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="cd4f3-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="cd4f3-137">енабледпревиевфеатурес</span><span class="sxs-lookup"><span data-stu-id="cd4f3-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="cd4f3-138">Коллекция (String)</span><span class="sxs-lookup"><span data-stu-id="cd4f3-138">Collection(string)</span></span>| <span data-ttu-id="cd4f3-139">Список компонентов, включенных для закрытой предварительной версии в клиенте.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="cd4f3-140">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="cd4f3-140">blockMsolPowerShell</span></span>|<span data-ttu-id="cd4f3-141">Логический</span><span class="sxs-lookup"><span data-stu-id="cd4f3-141">Boolean</span></span>| <span data-ttu-id="cd4f3-142">Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="cd4f3-143">Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="cd4f3-144">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 


## <a name="relationships"></a><span data-ttu-id="cd4f3-145">Связи</span><span class="sxs-lookup"><span data-stu-id="cd4f3-145">Relationships</span></span>
<span data-ttu-id="cd4f3-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd4f3-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cd4f3-147">JSON representation</span></span>

<span data-ttu-id="cd4f3-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-148">The following is a JSON representation of the resource.</span></span>

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
  "blockMsolPowerShell": true 
}
```
