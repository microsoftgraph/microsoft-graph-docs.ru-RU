---
title: Тип ресурса internetMessageHeader
description: 'Ключ типа "ключ — значение", представляющий заголовок сообщения в Интернете, как определено в RFC5322, который предоставляет '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 5f11f176eaf7d1817f58ed5f1ba25483965a5258
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044230"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="738ed-103">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="738ed-103">internetMessageHeader resource type</span></span>

<span data-ttu-id="738ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="738ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="738ed-105">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="738ed-105">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span>

<span data-ttu-id="738ed-106">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="738ed-106">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="738ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="738ed-107">Properties</span></span>
| <span data-ttu-id="738ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="738ed-108">Property</span></span>     | <span data-ttu-id="738ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="738ed-109">Type</span></span>   |<span data-ttu-id="738ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="738ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="738ed-111">name</span><span class="sxs-lookup"><span data-stu-id="738ed-111">name</span></span>|<span data-ttu-id="738ed-112">string</span><span class="sxs-lookup"><span data-stu-id="738ed-112">string</span></span>|<span data-ttu-id="738ed-113">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="738ed-113">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="738ed-114">value</span><span class="sxs-lookup"><span data-stu-id="738ed-114">value</span></span>|<span data-ttu-id="738ed-115">string</span><span class="sxs-lookup"><span data-stu-id="738ed-115">string</span></span>|<span data-ttu-id="738ed-116">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="738ed-116">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="738ed-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="738ed-117">JSON representation</span></span>

<span data-ttu-id="738ed-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="738ed-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


