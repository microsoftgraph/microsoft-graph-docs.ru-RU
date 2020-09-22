---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15feb2097a3a7bf36092070cc2af4841d2aa3839
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019399"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="52e92-103">Тип ресурса Воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="52e92-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="52e92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52e92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52e92-105">Объект шифрования, определяющий протокол и секрет для [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="52e92-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="52e92-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="52e92-106">Properties</span></span>

| <span data-ttu-id="52e92-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="52e92-107">Property</span></span>     | <span data-ttu-id="52e92-108">Тип</span><span class="sxs-lookup"><span data-stu-id="52e92-108">Type</span></span>        | <span data-ttu-id="52e92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="52e92-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52e92-110">Protocol</span><span class="sxs-lookup"><span data-stu-id="52e92-110">protocol</span></span>|<span data-ttu-id="52e92-111">String</span><span class="sxs-lookup"><span data-stu-id="52e92-111">String</span></span>| <span data-ttu-id="52e92-112">Возможные значения: `sharedSecret`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="52e92-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="52e92-113">гадк</span><span class="sxs-lookup"><span data-stu-id="52e92-113">secret</span></span>|<span data-ttu-id="52e92-114">String</span><span class="sxs-lookup"><span data-stu-id="52e92-114">String</span></span>|<span data-ttu-id="52e92-115">Шифрование общего секрета.</span><span class="sxs-lookup"><span data-stu-id="52e92-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52e92-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52e92-116">JSON representation</span></span>

<span data-ttu-id="52e92-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52e92-117">The following is a JSON representation of the resource.</span></span>

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


