# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="6722c-101">Тип ресурса internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="6722c-101">internetMessageHeader resource type</span></span>


<span data-ttu-id="6722c-102">Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.</span><span class="sxs-lookup"><span data-stu-id="6722c-102">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="6722c-103">С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/ru-RU/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="6722c-103">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/ru-RU/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="6722c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6722c-104">Properties</span></span>
| <span data-ttu-id="6722c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6722c-105">Property</span></span>     | <span data-ttu-id="6722c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6722c-106">Type</span></span>   |<span data-ttu-id="6722c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="6722c-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6722c-108">name</span><span class="sxs-lookup"><span data-stu-id="6722c-108">name</span></span>|<span data-ttu-id="6722c-109">string</span><span class="sxs-lookup"><span data-stu-id="6722c-109">string</span></span>|<span data-ttu-id="6722c-110">Представляет ключ в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="6722c-110">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="6722c-111">value</span><span class="sxs-lookup"><span data-stu-id="6722c-111">value</span></span>|<span data-ttu-id="6722c-112">string</span><span class="sxs-lookup"><span data-stu-id="6722c-112">string</span></span>|<span data-ttu-id="6722c-113">Представляет значение в паре "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="6722c-113">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6722c-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6722c-114">JSON representation</span></span>

<span data-ttu-id="6722c-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6722c-115">Here is a JSON representation of the resource.</span></span>

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