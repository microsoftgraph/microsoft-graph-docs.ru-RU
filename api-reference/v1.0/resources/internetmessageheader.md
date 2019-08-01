---
title: Тип ресурса internetMessageHeader
description: 'Ключ типа "ключ — значение", представляющий заголовок сообщения в Интернете, как определено в RFC5322, который предоставляет '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 14d4cb88c79651bbba381206df7d5ff9b26db0bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030200"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="d5e09-103">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="d5e09-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="d5e09-104">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="d5e09-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="d5e09-105">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="d5e09-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="d5e09-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5e09-106">Properties</span></span>
| <span data-ttu-id="d5e09-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5e09-107">Property</span></span>     | <span data-ttu-id="d5e09-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d5e09-108">Type</span></span>   |<span data-ttu-id="d5e09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e09-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e09-110">name</span><span class="sxs-lookup"><span data-stu-id="d5e09-110">name</span></span>|<span data-ttu-id="d5e09-111">string</span><span class="sxs-lookup"><span data-stu-id="d5e09-111">string</span></span>|<span data-ttu-id="d5e09-112">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d5e09-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="d5e09-113">value</span><span class="sxs-lookup"><span data-stu-id="d5e09-113">value</span></span>|<span data-ttu-id="d5e09-114">string</span><span class="sxs-lookup"><span data-stu-id="d5e09-114">string</span></span>|<span data-ttu-id="d5e09-115">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d5e09-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5e09-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5e09-116">JSON representation</span></span>

<span data-ttu-id="d5e09-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5e09-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
