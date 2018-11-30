---
title: Тип ресурса internetMessageHeader
description: 'Пары "ключ значение" представляет заголовок сообщения Интернета, в соответствии с RFC5322, который предоставляет '
ms.openlocfilehash: 420d39b6a139563e3f5f277f032f0f7a29252337
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077912"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="d6413-103">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="d6413-103">internetMessageHeader resource type</span></span>

> <span data-ttu-id="d6413-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6413-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6413-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6413-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6413-106">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="d6413-106">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="d6413-107">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="d6413-107">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="d6413-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6413-108">Properties</span></span>
| <span data-ttu-id="d6413-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6413-109">Property</span></span>     | <span data-ttu-id="d6413-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6413-110">Type</span></span>   |<span data-ttu-id="d6413-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6413-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6413-112">name</span><span class="sxs-lookup"><span data-stu-id="d6413-112">name</span></span>|<span data-ttu-id="d6413-113">строка</span><span class="sxs-lookup"><span data-stu-id="d6413-113">string</span></span>|<span data-ttu-id="d6413-114">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d6413-114">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="d6413-115">value</span><span class="sxs-lookup"><span data-stu-id="d6413-115">value</span></span>|<span data-ttu-id="d6413-116">строка</span><span class="sxs-lookup"><span data-stu-id="d6413-116">string</span></span>|<span data-ttu-id="d6413-117">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d6413-117">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6413-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6413-118">JSON representation</span></span>

<span data-ttu-id="d6413-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6413-119">Here is a JSON representation of the resource.</span></span>

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