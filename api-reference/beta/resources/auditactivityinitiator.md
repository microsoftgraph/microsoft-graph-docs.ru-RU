---
title: Тип ресурса auditActivityInitiator
description: Идентификатор объекта ресурса, запускает действие. Инициатор может быть пользователем, приложения или системы (который считается, что приложение)
ms.openlocfilehash: 834b39f67a9a3a251c61f15d3b1fa8aa964870e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079535"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="40280-104">Тип ресурса auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="40280-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="40280-105">Идентификатор объекта ресурса, запускает действие.</span><span class="sxs-lookup"><span data-stu-id="40280-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="40280-106">Инициатор может быть пользователем, приложения или системы (который считается, что приложение)</span><span class="sxs-lookup"><span data-stu-id="40280-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="40280-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40280-107">Properties</span></span>
| <span data-ttu-id="40280-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40280-108">Property</span></span>     | <span data-ttu-id="40280-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40280-109">Type</span></span>   |<span data-ttu-id="40280-110">Description</span><span class="sxs-lookup"><span data-stu-id="40280-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40280-111">приложение</span><span class="sxs-lookup"><span data-stu-id="40280-111">app</span></span>|[<span data-ttu-id="40280-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="40280-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="40280-113">Если ресурсов, инициализация действие представляет собой приложение, это свойство показывает все приложения связанные сведения, например, appId, имя, servicePrincipalId, имя.</span><span class="sxs-lookup"><span data-stu-id="40280-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="40280-114">user</span><span class="sxs-lookup"><span data-stu-id="40280-114">user</span></span>|[<span data-ttu-id="40280-115">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="40280-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="40280-116">Если ресурсов, инициализация действия пользователя, это свойство показывает все пользовательские связанные сведения, например, идентификатор пользователя, имя, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="40280-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40280-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40280-117">JSON representation</span></span>

<span data-ttu-id="40280-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40280-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->