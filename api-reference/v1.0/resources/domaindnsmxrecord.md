<span data-ttu-id="2417d-p105">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="2417d-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span>| Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null. |

## <span data-ttu-id="2417d-140">Связи</span><span class="sxs-lookup"><span data-stu-id="2417d-140">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="2417d-141">Нет</span><span class="sxs-lookup"><span data-stu-id="2417d-141">None</span></span>

## <span data-ttu-id="2417d-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2417d-142">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="2417d-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2417d-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->