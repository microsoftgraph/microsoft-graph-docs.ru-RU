# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="ae798-101">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="ae798-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="ae798-102">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="ae798-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae798-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ae798-103">JSON representation</span></span>

<span data-ttu-id="ae798-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ae798-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="ae798-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae798-105">Properties</span></span>

| <span data-ttu-id="ae798-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae798-106">Property</span></span> | <span data-ttu-id="ae798-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ae798-107">Type</span></span>  | <span data-ttu-id="ae798-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ae798-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="ae798-109">id</span><span class="sxs-lookup"><span data-stu-id="ae798-109">id</span></span>  | <span data-ttu-id="ae798-110">строка</span><span class="sxs-lookup"><span data-stu-id="ae798-110">string</span></span> | <span data-ttu-id="ae798-111">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="ae798-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="ae798-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="ae798-112">persistChanges</span></span> | <span data-ttu-id="ae798-113">boolean</span><span class="sxs-lookup"><span data-stu-id="ae798-113">boolean</span></span> |  <span data-ttu-id="ae798-114">`true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="ae798-114">`true` for persistent session.</span></span> <span data-ttu-id="ae798-115">`false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="ae798-115">`false` for non-persistent session (view mode)</span></span> |

