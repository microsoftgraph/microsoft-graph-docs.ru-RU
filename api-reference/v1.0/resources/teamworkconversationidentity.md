---
title: тип ресурса teamworkConversationIdentity
description: Представляет беседу в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1bf17f9954459a1e476106315db60f65dc536b02
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211137"
---
# <a name="teamworkconversationidentity-resource-type"></a><span data-ttu-id="e650b-103">тип ресурса teamworkConversationIdentity</span><span class="sxs-lookup"><span data-stu-id="e650b-103">teamworkConversationIdentity resource type</span></span>

<span data-ttu-id="e650b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e650b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e650b-105">Представляет **беседу (чат,** команду или канал) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e650b-105">Represents a **conversation** (chat, team, or channel) in Microsoft Teams.</span></span>

<span data-ttu-id="e650b-106">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="e650b-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e650b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e650b-107">Properties</span></span>
|<span data-ttu-id="e650b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e650b-108">Property</span></span>|<span data-ttu-id="e650b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e650b-109">Type</span></span>|<span data-ttu-id="e650b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e650b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e650b-111">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="e650b-111">conversationIdentityType</span></span>|<span data-ttu-id="e650b-112">teamworkConversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="e650b-112">teamworkConversationIdentityType</span></span>|<span data-ttu-id="e650b-113">Тип беседы.</span><span class="sxs-lookup"><span data-stu-id="e650b-113">Type of conversation.</span></span> <span data-ttu-id="e650b-114">Возможные значения: `team`, `channel`, `chat` и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e650b-114">Possible values are: `team`, `channel`, `chat`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e650b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e650b-115">displayName</span></span>|<span data-ttu-id="e650b-116">String</span><span class="sxs-lookup"><span data-stu-id="e650b-116">String</span></span>|<span data-ttu-id="e650b-117">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="e650b-117">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="e650b-118">Отображение имени беседы.</span><span class="sxs-lookup"><span data-stu-id="e650b-118">Display name of the conversation.</span></span> <span data-ttu-id="e650b-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e650b-119">Optional.</span></span>|
|<span data-ttu-id="e650b-120">id</span><span class="sxs-lookup"><span data-stu-id="e650b-120">id</span></span>|<span data-ttu-id="e650b-121">String</span><span class="sxs-lookup"><span data-stu-id="e650b-121">String</span></span>|<span data-ttu-id="e650b-122">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="e650b-122">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="e650b-123">ID беседы.</span><span class="sxs-lookup"><span data-stu-id="e650b-123">ID of the conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e650b-124">Связи</span><span class="sxs-lookup"><span data-stu-id="e650b-124">Relationships</span></span>
<span data-ttu-id="e650b-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e650b-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e650b-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e650b-126">JSON representation</span></span>
<span data-ttu-id="e650b-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e650b-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

