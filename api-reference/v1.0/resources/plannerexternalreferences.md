# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="e473f-101">Тип ресурса plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="e473f-101">plannerExternalReferences resource type</span></span>

<span data-ttu-id="e473f-p101">Ресурс **plannerExternalReferences** представляет коллекцию справочных материалов для задачи. Это открытый тип. Он является частью объекта [сведений о задаче](plannertaskdetails.md). Значение в паре "свойство-значение" представляет собой объект [externalReference](plannerexternalreference.md).</span><span class="sxs-lookup"><span data-stu-id="e473f-p101">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="e473f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e473f-106">Properties</span></span>
<span data-ttu-id="e473f-p102">Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить **допустимые URL-адреса** на базе протоколов **HTTP/HTTPS** в качестве свойств с объектами [externalReference](plannerexternalreference.md) в качестве значений. Согласно OData имена свойств в открытых типах не могут содержать символы `.`, `:` и `%`, поэтому их нужно зашифровать. Ниже показан пример. Чтобы удалить определенные справочные материалы, задайте свойству значение `null`.</span><span class="sxs-lookup"><span data-stu-id="e473f-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e473f-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e473f-112">JSON representation</span></span>

<span data-ttu-id="e473f-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e473f-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

<span data-ttu-id="e473f-114">Пример:</span><span class="sxs-lookup"><span data-stu-id="e473f-114">// Example</span></span>

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->