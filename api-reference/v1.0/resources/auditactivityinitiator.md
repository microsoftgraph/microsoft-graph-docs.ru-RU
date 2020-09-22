---
title: Тип ресурса Аудитактивитинитиатор
description: Определяет объект ресурса, инициирующий действие. Инициатор может быть пользователем, приложением или системой (который рассматривается как приложение).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d6d4d41698e6251c0f33a637dff9e667df7d092
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988515"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="d7322-104">Тип ресурса Аудитактивитинитиатор</span><span class="sxs-lookup"><span data-stu-id="d7322-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="d7322-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7322-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7322-106">Identity объект ресурса, инициирующий действие.</span><span class="sxs-lookup"><span data-stu-id="d7322-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="d7322-107">Инициатор может быть пользователем, приложением или системой (которое считается приложением).</span><span class="sxs-lookup"><span data-stu-id="d7322-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="d7322-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7322-108">Properties</span></span>

| <span data-ttu-id="d7322-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7322-109">Property</span></span>     | <span data-ttu-id="d7322-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7322-110">Type</span></span>   |<span data-ttu-id="d7322-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7322-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7322-112">программы</span><span class="sxs-lookup"><span data-stu-id="d7322-112">app</span></span>|[<span data-ttu-id="d7322-113">аппидентити</span><span class="sxs-lookup"><span data-stu-id="d7322-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="d7322-114">Если ресурс, инициирующий действие, является приложением, это свойство указывает все связанные с приложением сведения, такие как appId, Name, СервицепринЦипалид и Name.</span><span class="sxs-lookup"><span data-stu-id="d7322-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="d7322-115">user</span><span class="sxs-lookup"><span data-stu-id="d7322-115">user</span></span>|[<span data-ttu-id="d7322-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d7322-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="d7322-117">Если ресурс, инициирующий действие, является пользователем, это свойство указывает все связанные с пользователем сведения, такие как userId, Name, Усерприникпалнаме.</span><span class="sxs-lookup"><span data-stu-id="d7322-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7322-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7322-118">JSON representation</span></span>

<span data-ttu-id="d7322-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7322-119">Here is a JSON representation of the resource.</span></span>

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

