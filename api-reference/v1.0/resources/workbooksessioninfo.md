# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="eef8e-101">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="eef8e-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="eef8e-102">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="eef8e-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="eef8e-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eef8e-103">JSON representation</span></span>

<span data-ttu-id="eef8e-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="eef8e-104">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="eef8e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="eef8e-105">Properties</span></span>

| <span data-ttu-id="eef8e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef8e-106">Property</span></span> | <span data-ttu-id="eef8e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="eef8e-107">Type</span></span>  | <span data-ttu-id="eef8e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eef8e-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="eef8e-109">id</span><span class="sxs-lookup"><span data-stu-id="eef8e-109">id</span></span>  | <span data-ttu-id="eef8e-110">строка</span><span class="sxs-lookup"><span data-stu-id="eef8e-110">string</span></span> | <span data-ttu-id="eef8e-111">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="eef8e-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="eef8e-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="eef8e-112">persistChanges</span></span> | <span data-ttu-id="eef8e-113">строка</span><span class="sxs-lookup"><span data-stu-id="eef8e-113">string</span></span> |  <span data-ttu-id="eef8e-114">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="eef8e-114">`true` for persistent session.</span></span> <span data-ttu-id="eef8e-115">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="eef8e-115">`false` for non-persistent session (view mode)</span></span> |

