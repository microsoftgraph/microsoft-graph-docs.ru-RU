---
title: Тип ресурса Воркфорцеинтегратионенкриптион
description: Объект шифрования, определяющий протокол и секрет для интеграции сотрудников.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb974b80b03edc36a0f974633c8f95ca384182e6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154152"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="dfa7c-103">Тип ресурса Воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="dfa7c-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="dfa7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa7c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfa7c-105">Объект шифрования, определяющий протокол и секрет для [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="dfa7c-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dfa7c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfa7c-106">Properties</span></span>

| <span data-ttu-id="dfa7c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfa7c-107">Property</span></span>     | <span data-ttu-id="dfa7c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dfa7c-108">Type</span></span>        | <span data-ttu-id="dfa7c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa7c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfa7c-110">Protocol</span><span class="sxs-lookup"><span data-stu-id="dfa7c-110">protocol</span></span>|<span data-ttu-id="dfa7c-111">String</span><span class="sxs-lookup"><span data-stu-id="dfa7c-111">String</span></span>| <span data-ttu-id="dfa7c-112">Возможные значения: `sharedSecret`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dfa7c-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dfa7c-113">гадк</span><span class="sxs-lookup"><span data-stu-id="dfa7c-113">secret</span></span>|<span data-ttu-id="dfa7c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="dfa7c-114">String</span></span>|<span data-ttu-id="dfa7c-115">Шифрование общего секрета.</span><span class="sxs-lookup"><span data-stu-id="dfa7c-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfa7c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfa7c-116">JSON representation</span></span>

<span data-ttu-id="dfa7c-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfa7c-117">The following is a JSON representation of the resource.</span></span>

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
