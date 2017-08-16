# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="ffb57-101">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ffb57-101">scoredEmailAddress resource type</span></span>

<span data-ttu-id="ffb57-102">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ffb57-102">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="ffb57-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffb57-103">Properties</span></span>
| <span data-ttu-id="ffb57-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffb57-104">Property</span></span>     | <span data-ttu-id="ffb57-105">Тип</span><span class="sxs-lookup"><span data-stu-id="ffb57-105">Type</span></span>   |<span data-ttu-id="ffb57-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ffb57-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffb57-107">address</span><span class="sxs-lookup"><span data-stu-id="ffb57-107">address</span></span>|<span data-ttu-id="ffb57-108">string</span><span class="sxs-lookup"><span data-stu-id="ffb57-108">string</span></span>|<span data-ttu-id="ffb57-109">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ffb57-109">The user's email address.</span></span>|
|<span data-ttu-id="ffb57-110">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="ffb57-110">relevanceScore</span></span>|<span data-ttu-id="ffb57-111">double</span><span class="sxs-lookup"><span data-stu-id="ffb57-111">double</span></span>|<span data-ttu-id="ffb57-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="ffb57-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ffb57-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ffb57-116">JSON representation</span></span>

<span data-ttu-id="ffb57-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffb57-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
