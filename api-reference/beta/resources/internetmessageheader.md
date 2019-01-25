---
title: Тип ресурса internetMessageHeader
description: 'Пары "ключ значение" представляет заголовок сообщения Интернета, в соответствии с RFC5322, который предоставляет '
localization_priority: Normal
ms.openlocfilehash: e748e6badd3e6bad6adb02a9df46a40a7241d636
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511669"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="15d41-103">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="15d41-103">internetMessageHeader resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15d41-104">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="15d41-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="15d41-105">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="15d41-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="15d41-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="15d41-106">Properties</span></span>
| <span data-ttu-id="15d41-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="15d41-107">Property</span></span>     | <span data-ttu-id="15d41-108">Тип</span><span class="sxs-lookup"><span data-stu-id="15d41-108">Type</span></span>   |<span data-ttu-id="15d41-109">Описание</span><span class="sxs-lookup"><span data-stu-id="15d41-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15d41-110">name</span><span class="sxs-lookup"><span data-stu-id="15d41-110">name</span></span>|<span data-ttu-id="15d41-111">string</span><span class="sxs-lookup"><span data-stu-id="15d41-111">string</span></span>|<span data-ttu-id="15d41-112">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="15d41-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="15d41-113">value</span><span class="sxs-lookup"><span data-stu-id="15d41-113">value</span></span>|<span data-ttu-id="15d41-114">строка</span><span class="sxs-lookup"><span data-stu-id="15d41-114">string</span></span>|<span data-ttu-id="15d41-115">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="15d41-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15d41-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15d41-116">JSON representation</span></span>

<span data-ttu-id="15d41-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15d41-117">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/internetmessageheader.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
