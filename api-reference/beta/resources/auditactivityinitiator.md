---
title: Тип ресурса Аудитактивитинитиатор
description: Identity объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 49c60dc42cb84d047f36904b2af11fe5c8d3bd8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812550"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="c70f0-104">Тип ресурса Аудитактивитинитиатор</span><span class="sxs-lookup"><span data-stu-id="c70f0-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="c70f0-105">Пространство имен: Microsoft. Graph Identity объект ресурса, инициирующий действие.</span><span class="sxs-lookup"><span data-stu-id="c70f0-105">Namespace: microsoft.graph Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="c70f0-106">Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).</span><span class="sxs-lookup"><span data-stu-id="c70f0-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="c70f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c70f0-107">Properties</span></span>
| <span data-ttu-id="c70f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c70f0-108">Property</span></span>     | <span data-ttu-id="c70f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c70f0-109">Type</span></span>   |<span data-ttu-id="c70f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c70f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c70f0-111">программы</span><span class="sxs-lookup"><span data-stu-id="c70f0-111">app</span></span>|[<span data-ttu-id="c70f0-112">аппидентити</span><span class="sxs-lookup"><span data-stu-id="c70f0-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="c70f0-113">Если ресурс, инициирующий действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, СервицепринЦипалид и Name.</span><span class="sxs-lookup"><span data-stu-id="c70f0-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="c70f0-114">user</span><span class="sxs-lookup"><span data-stu-id="c70f0-114">user</span></span>|[<span data-ttu-id="c70f0-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c70f0-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="c70f0-116">Если ресурс, инициирующий действие, является пользователем, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, Усерприникпалнаме.</span><span class="sxs-lookup"><span data-stu-id="c70f0-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c70f0-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c70f0-117">JSON representation</span></span>

<span data-ttu-id="c70f0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c70f0-118">Here is a JSON representation of the resource.</span></span>

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
