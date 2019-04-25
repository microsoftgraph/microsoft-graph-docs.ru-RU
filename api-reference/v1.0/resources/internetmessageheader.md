---
title: Тип ресурса internetMessageHeader
description: 'Ключ типа "ключ — значение", представляющий заголовок сообщения в Интернете, как определено в RFC5322, который предоставляет '
localization_priority: Normal
ms.openlocfilehash: 2a8dd616ffe8417a5064c0a98976d512b1279704
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567517"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="a0f3b-103">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="a0f3b-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="a0f3b-104">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="a0f3b-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="a0f3b-105">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="a0f3b-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="a0f3b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0f3b-106">Properties</span></span>
| <span data-ttu-id="a0f3b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0f3b-107">Property</span></span>     | <span data-ttu-id="a0f3b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a0f3b-108">Type</span></span>   |<span data-ttu-id="a0f3b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0f3b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0f3b-110">name</span><span class="sxs-lookup"><span data-stu-id="a0f3b-110">name</span></span>|<span data-ttu-id="a0f3b-111">string</span><span class="sxs-lookup"><span data-stu-id="a0f3b-111">string</span></span>|<span data-ttu-id="a0f3b-112">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a0f3b-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="a0f3b-113">value</span><span class="sxs-lookup"><span data-stu-id="a0f3b-113">value</span></span>|<span data-ttu-id="a0f3b-114">string</span><span class="sxs-lookup"><span data-stu-id="a0f3b-114">string</span></span>|<span data-ttu-id="a0f3b-115">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a0f3b-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0f3b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0f3b-116">JSON representation</span></span>

<span data-ttu-id="a0f3b-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0f3b-117">Here is a JSON representation of the resource.</span></span>

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
