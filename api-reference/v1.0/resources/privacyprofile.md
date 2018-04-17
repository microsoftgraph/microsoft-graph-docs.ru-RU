# <a name="privacyprofile-resource-type"></a><span data-ttu-id="69a36-101">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="69a36-101">privacyProfile resource type</span></span>

<span data-ttu-id="69a36-102">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="69a36-102">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="69a36-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="69a36-103">Properties</span></span>
| <span data-ttu-id="69a36-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="69a36-104">Property</span></span>   | <span data-ttu-id="69a36-105">Тип</span><span class="sxs-lookup"><span data-stu-id="69a36-105">Type</span></span>|<span data-ttu-id="69a36-106">Описание</span><span class="sxs-lookup"><span data-stu-id="69a36-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69a36-107">contactEmail</span><span class="sxs-lookup"><span data-stu-id="69a36-107">contactEmail</span></span>|<span data-ttu-id="69a36-108">String</span><span class="sxs-lookup"><span data-stu-id="69a36-108">String</span></span>| <span data-ttu-id="69a36-109">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="69a36-109">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="69a36-110">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="69a36-110">Not required</span></span>|
|<span data-ttu-id="69a36-111">statementUrl</span><span class="sxs-lookup"><span data-stu-id="69a36-111">statementUrl</span></span>|<span data-ttu-id="69a36-112">String</span><span class="sxs-lookup"><span data-stu-id="69a36-112">String</span></span>| <span data-ttu-id="69a36-113">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="69a36-113">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="69a36-114">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="69a36-114">The maximum length is 255 characters.</span></span> <span data-ttu-id="69a36-115">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="69a36-115">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="69a36-116">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="69a36-116">Not required</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69a36-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69a36-117">JSON representation</span></span>

<span data-ttu-id="69a36-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69a36-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```