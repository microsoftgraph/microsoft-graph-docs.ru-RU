---
title: тип ресурса teamworkApplicationIdentity
description: Представляет приложение в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 67e1ed4365febae44032c09d94656d2e3ac0b504
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211142"
---
# <a name="teamworkapplicationidentity-resource-type"></a><span data-ttu-id="d028f-103">тип ресурса teamworkApplicationIdentity</span><span class="sxs-lookup"><span data-stu-id="d028f-103">teamworkApplicationIdentity resource type</span></span>

<span data-ttu-id="d028f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d028f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d028f-105">Представляет приложение **в** Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d028f-105">Represents an **application** in Microsoft Teams.</span></span> <span data-ttu-id="d028f-106">`teamworkApplicationIdentity` используется для представления ботов и исходяющих веб-@mentioned в сообщениях.</span><span class="sxs-lookup"><span data-stu-id="d028f-106">`teamworkApplicationIdentity` is used to represent bots and outgoing webhooks @mentioned in messages.</span></span>


<span data-ttu-id="d028f-107">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="d028f-107">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d028f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d028f-108">Properties</span></span>
|<span data-ttu-id="d028f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d028f-109">Property</span></span>|<span data-ttu-id="d028f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d028f-110">Type</span></span>|<span data-ttu-id="d028f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d028f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d028f-112">applicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="d028f-112">applicationIdentityType</span></span>|<span data-ttu-id="d028f-113">teamworkApplicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="d028f-113">teamworkApplicationIdentityType</span></span>| <span data-ttu-id="d028f-114">Тип ссылаемого приложения.</span><span class="sxs-lookup"><span data-stu-id="d028f-114">Type of application that is referenced.</span></span> <span data-ttu-id="d028f-115">Возможные значения: `aadApplication` `bot` , , , , , `tenantBot` `office365Connector` и `outgoingWebhook` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d028f-115">Possible values are: `aadApplication`, `bot`, `tenantBot`, `office365Connector`, `outgoingWebhook`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d028f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d028f-116">displayName</span></span>|<span data-ttu-id="d028f-117">String</span><span class="sxs-lookup"><span data-stu-id="d028f-117">String</span></span>|<span data-ttu-id="d028f-118">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="d028f-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="d028f-119">Отображение имени приложения.</span><span class="sxs-lookup"><span data-stu-id="d028f-119">Display name of the application.</span></span> <span data-ttu-id="d028f-120">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d028f-120">Optional.</span></span>|
|<span data-ttu-id="d028f-121">id</span><span class="sxs-lookup"><span data-stu-id="d028f-121">id</span></span>|<span data-ttu-id="d028f-122">String</span><span class="sxs-lookup"><span data-stu-id="d028f-122">String</span></span>|<span data-ttu-id="d028f-123">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="d028f-123">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="d028f-124">ID приложения.</span><span class="sxs-lookup"><span data-stu-id="d028f-124">ID of the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d028f-125">Связи</span><span class="sxs-lookup"><span data-stu-id="d028f-125">Relationships</span></span>
<span data-ttu-id="d028f-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d028f-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d028f-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d028f-127">JSON representation</span></span>
<span data-ttu-id="d028f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d028f-128">The following is a JSON representation of the resource.</span></span>
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

