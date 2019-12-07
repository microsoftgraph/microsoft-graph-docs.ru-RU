---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52fb72380ce74acad429aa3da6f9ad4e60102e06
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895840"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="9e4fc-103">Тип ресурса Воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="9e4fc-103">workforceIntegrationEncryption resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e4fc-104">Объект шифрования, определяющий протокол и секрет для [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="9e4fc-104">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e4fc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e4fc-105">Properties</span></span>

| <span data-ttu-id="9e4fc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e4fc-106">Property</span></span>     | <span data-ttu-id="9e4fc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9e4fc-107">Type</span></span>        | <span data-ttu-id="9e4fc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9e4fc-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e4fc-109">Protocol</span><span class="sxs-lookup"><span data-stu-id="9e4fc-109">protocol</span></span>|<span data-ttu-id="9e4fc-110">String</span><span class="sxs-lookup"><span data-stu-id="9e4fc-110">String</span></span>| <span data-ttu-id="9e4fc-111">Возможные значения: `sharedSecret`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e4fc-111">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9e4fc-112">гадк</span><span class="sxs-lookup"><span data-stu-id="9e4fc-112">secret</span></span>|<span data-ttu-id="9e4fc-113">String</span><span class="sxs-lookup"><span data-stu-id="9e4fc-113">String</span></span>|<span data-ttu-id="9e4fc-114">Шифрование общего секрета.</span><span class="sxs-lookup"><span data-stu-id="9e4fc-114">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e4fc-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e4fc-115">JSON representation</span></span>

<span data-ttu-id="9e4fc-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e4fc-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
