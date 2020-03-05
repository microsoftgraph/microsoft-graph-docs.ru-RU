---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2d24371a0a999069d80a9ad86afd48ac9e68d38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519080"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="901e0-103">Тип ресурса Воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="901e0-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="901e0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="901e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="901e0-105">Объект шифрования, определяющий протокол и секрет для [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="901e0-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="901e0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="901e0-106">Properties</span></span>

| <span data-ttu-id="901e0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="901e0-107">Property</span></span>     | <span data-ttu-id="901e0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="901e0-108">Type</span></span>        | <span data-ttu-id="901e0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="901e0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="901e0-110">Protocol</span><span class="sxs-lookup"><span data-stu-id="901e0-110">protocol</span></span>|<span data-ttu-id="901e0-111">String</span><span class="sxs-lookup"><span data-stu-id="901e0-111">String</span></span>| <span data-ttu-id="901e0-112">Возможные значения: `sharedSecret`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="901e0-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="901e0-113">гадк</span><span class="sxs-lookup"><span data-stu-id="901e0-113">secret</span></span>|<span data-ttu-id="901e0-114">String</span><span class="sxs-lookup"><span data-stu-id="901e0-114">String</span></span>|<span data-ttu-id="901e0-115">Шифрование общего секрета.</span><span class="sxs-lookup"><span data-stu-id="901e0-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="901e0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="901e0-116">JSON representation</span></span>

<span data-ttu-id="901e0-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="901e0-117">The following is a JSON representation of the resource.</span></span>

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
