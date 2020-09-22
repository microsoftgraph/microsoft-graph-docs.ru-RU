---
title: Тип ресурса инициатора
description: Указывает, кто инициировал событие подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0b6b326925d0ca3f0dbf8c0c25df266834ecce6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021912"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="1da86-103">Тип ресурса инициатора</span><span class="sxs-lookup"><span data-stu-id="1da86-103">initiator resource type</span></span>

<span data-ttu-id="1da86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1da86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1da86-105">Указывает, кто инициировал событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="1da86-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="1da86-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1da86-106">Properties</span></span>

| <span data-ttu-id="1da86-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1da86-107">Property</span></span>     | <span data-ttu-id="1da86-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1da86-108">Type</span></span>        | <span data-ttu-id="1da86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1da86-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1da86-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1da86-110">displayName</span></span>|<span data-ttu-id="1da86-111">String</span><span class="sxs-lookup"><span data-stu-id="1da86-111">String</span></span>|<span data-ttu-id="1da86-112">Имя пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="1da86-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="1da86-113">id</span><span class="sxs-lookup"><span data-stu-id="1da86-113">id</span></span>|<span data-ttu-id="1da86-114">String</span><span class="sxs-lookup"><span data-stu-id="1da86-114">String</span></span>|<span data-ttu-id="1da86-115">Уникальный идентификатор пользователя или службы, которые инициировали событие подготовки.</span><span class="sxs-lookup"><span data-stu-id="1da86-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="1da86-116">инитиатортипе</span><span class="sxs-lookup"><span data-stu-id="1da86-116">initiatorType</span></span>|<span data-ttu-id="1da86-117">String</span><span class="sxs-lookup"><span data-stu-id="1da86-117">String</span></span>| <span data-ttu-id="1da86-118">Тип инициатора.</span><span class="sxs-lookup"><span data-stu-id="1da86-118">Type of initiator.</span></span> <span data-ttu-id="1da86-119">Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1da86-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1da86-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1da86-120">JSON representation</span></span>

<span data-ttu-id="1da86-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1da86-121">The following is a JSON representation of the resource.</span></span>

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


