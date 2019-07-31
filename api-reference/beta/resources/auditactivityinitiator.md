---
title: Тип ресурса Аудитактивитинитиатор
description: Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f76c071efd10d2d43887bdd5dd04df0d2aa86d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974229"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="40d2a-104">Тип ресурса Аудитактивитинитиатор</span><span class="sxs-lookup"><span data-stu-id="40d2a-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="40d2a-105">Identity объект ресурса, инициирующий действие.</span><span class="sxs-lookup"><span data-stu-id="40d2a-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="40d2a-106">Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).</span><span class="sxs-lookup"><span data-stu-id="40d2a-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="40d2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40d2a-107">Properties</span></span>
| <span data-ttu-id="40d2a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40d2a-108">Property</span></span>     | <span data-ttu-id="40d2a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40d2a-109">Type</span></span>   |<span data-ttu-id="40d2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40d2a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40d2a-111">программы</span><span class="sxs-lookup"><span data-stu-id="40d2a-111">app</span></span>|[<span data-ttu-id="40d2a-112">Аппидентити</span><span class="sxs-lookup"><span data-stu-id="40d2a-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="40d2a-113">Если ресурс, инициирующий действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, СервицепринЦипалид и Name.</span><span class="sxs-lookup"><span data-stu-id="40d2a-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="40d2a-114">user</span><span class="sxs-lookup"><span data-stu-id="40d2a-114">user</span></span>|[<span data-ttu-id="40d2a-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="40d2a-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="40d2a-116">Если ресурс, инициирующий действие, является пользователем, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, Усерприникпалнаме.</span><span class="sxs-lookup"><span data-stu-id="40d2a-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40d2a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40d2a-117">JSON representation</span></span>

<span data-ttu-id="40d2a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40d2a-118">Here is a JSON representation of the resource.</span></span>

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
