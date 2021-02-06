---
title: Тип ресурса auditActivityInitiator
description: Удостоверение объекта ресурса, который инициирует действие. Инициатором может быть пользователь, приложение или система (которая считается приложением)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: 71aa5e2bd09d66a2aea49058ceffea3e017eaf4d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131637"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="36085-104">Тип ресурса auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="36085-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="36085-105">Пространство имен: удостоверение microsoft.graph для объекта ресурса, который инициирует действие.</span><span class="sxs-lookup"><span data-stu-id="36085-105">Namespace: microsoft.graph Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="36085-106">Инициатором может быть пользователь, приложение или система (которая считается приложением)</span><span class="sxs-lookup"><span data-stu-id="36085-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="36085-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="36085-107">Properties</span></span>
| <span data-ttu-id="36085-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="36085-108">Property</span></span>     | <span data-ttu-id="36085-109">Тип</span><span class="sxs-lookup"><span data-stu-id="36085-109">Type</span></span>   |<span data-ttu-id="36085-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36085-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36085-111">приложение</span><span class="sxs-lookup"><span data-stu-id="36085-111">app</span></span>|[<span data-ttu-id="36085-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="36085-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="36085-113">Если ресурс, инициируя действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, servicePrincipalId, Name.</span><span class="sxs-lookup"><span data-stu-id="36085-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="36085-114">user</span><span class="sxs-lookup"><span data-stu-id="36085-114">user</span></span>|[<span data-ttu-id="36085-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="36085-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="36085-116">Если ресурсом, инициирующим действие, является пользователь, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="36085-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36085-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36085-117">JSON representation</span></span>

<span data-ttu-id="36085-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36085-118">Here is a JSON representation of the resource.</span></span>

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


