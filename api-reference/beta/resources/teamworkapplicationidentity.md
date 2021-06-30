---
title: тип ресурса teamworkApplicationIdentity
description: Представляет приложение в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b7e6c17b70e7f30e102e270d2d98b406e01dcae3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211386"
---
# <a name="teamworkapplicationidentity-resource-type"></a><span data-ttu-id="f29b2-103">тип ресурса teamworkApplicationIdentity</span><span class="sxs-lookup"><span data-stu-id="f29b2-103">teamworkApplicationIdentity resource type</span></span>

<span data-ttu-id="f29b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f29b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f29b2-105">Представляет приложение **в** Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f29b2-105">Represents an **application** in Microsoft Teams.</span></span> <span data-ttu-id="f29b2-106">`teamworkApplicationIdentity` используется для представления ботов и исходяющих веб-@mentioned в сообщениях.</span><span class="sxs-lookup"><span data-stu-id="f29b2-106">`teamworkApplicationIdentity` is used to represent bots and outgoing webhooks @mentioned in messages.</span></span>


<span data-ttu-id="f29b2-107">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="f29b2-107">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f29b2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f29b2-108">Properties</span></span>
|<span data-ttu-id="f29b2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f29b2-109">Property</span></span>|<span data-ttu-id="f29b2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f29b2-110">Type</span></span>|<span data-ttu-id="f29b2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f29b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29b2-112">applicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="f29b2-112">applicationIdentityType</span></span>|<span data-ttu-id="f29b2-113">teamworkApplicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="f29b2-113">teamworkApplicationIdentityType</span></span>| <span data-ttu-id="f29b2-114">Тип ссылаемого приложения.</span><span class="sxs-lookup"><span data-stu-id="f29b2-114">Type of application that is referenced.</span></span> <span data-ttu-id="f29b2-115">Возможные значения: `aadApplication` `bot` , , , , `tenantBot` и `office365Connector` `outgoingWebhook` .</span><span class="sxs-lookup"><span data-stu-id="f29b2-115">Possible values are: `aadApplication`, `bot`, `tenantBot`, `office365Connector`, and `outgoingWebhook`.</span></span>|
|<span data-ttu-id="f29b2-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f29b2-116">displayName</span></span>|<span data-ttu-id="f29b2-117">String</span><span class="sxs-lookup"><span data-stu-id="f29b2-117">String</span></span>|<span data-ttu-id="f29b2-118">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="f29b2-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="f29b2-119">Отображение имени приложения.</span><span class="sxs-lookup"><span data-stu-id="f29b2-119">Display name of the application.</span></span> <span data-ttu-id="f29b2-120">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f29b2-120">Optional.</span></span>|
|<span data-ttu-id="f29b2-121">id</span><span class="sxs-lookup"><span data-stu-id="f29b2-121">id</span></span>|<span data-ttu-id="f29b2-122">String</span><span class="sxs-lookup"><span data-stu-id="f29b2-122">String</span></span>|<span data-ttu-id="f29b2-123">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="f29b2-123">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="f29b2-124">ID приложения.</span><span class="sxs-lookup"><span data-stu-id="f29b2-124">ID of the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f29b2-125">Связи</span><span class="sxs-lookup"><span data-stu-id="f29b2-125">Relationships</span></span>
<span data-ttu-id="f29b2-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f29b2-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f29b2-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f29b2-127">JSON representation</span></span>
<span data-ttu-id="f29b2-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f29b2-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

