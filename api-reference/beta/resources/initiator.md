---
title: Тип ресурса инициатора
description: Указывает, кто инициировал событие подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 909849775e5bf35c9a29902efbbc3975177956d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496014"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="d6e5b-103">Тип ресурса инициатора</span><span class="sxs-lookup"><span data-stu-id="d6e5b-103">initiator resource type</span></span>

<span data-ttu-id="d6e5b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6e5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e5b-105">Указывает, кто инициировал событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="d6e5b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6e5b-106">Properties</span></span>

| <span data-ttu-id="d6e5b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6e5b-107">Property</span></span>     | <span data-ttu-id="d6e5b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d6e5b-108">Type</span></span>        | <span data-ttu-id="d6e5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d6e5b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6e5b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d6e5b-110">displayName</span></span>|<span data-ttu-id="d6e5b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="d6e5b-111">String</span></span>|<span data-ttu-id="d6e5b-112">Имя пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d6e5b-113">id</span><span class="sxs-lookup"><span data-stu-id="d6e5b-113">id</span></span>|<span data-ttu-id="d6e5b-114">String</span><span class="sxs-lookup"><span data-stu-id="d6e5b-114">String</span></span>|<span data-ttu-id="d6e5b-115">Уникальный идентификатор пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d6e5b-116">инитиатортипе</span><span class="sxs-lookup"><span data-stu-id="d6e5b-116">initiatorType</span></span>|<span data-ttu-id="d6e5b-117">String</span><span class="sxs-lookup"><span data-stu-id="d6e5b-117">String</span></span>| <span data-ttu-id="d6e5b-118">Тип инициатора.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-118">Type of initiator.</span></span> <span data-ttu-id="d6e5b-119">Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6e5b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6e5b-120">JSON representation</span></span>

<span data-ttu-id="d6e5b-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6e5b-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
