<span data-ttu-id="0e6e5-p104">Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e6e5-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span>| Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения. |

## <span data-ttu-id="0e6e5-132">Связи</span><span class="sxs-lookup"><span data-stu-id="0e6e5-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="0e6e5-133">Нет</span><span class="sxs-lookup"><span data-stu-id="0e6e5-133">None</span></span>

## <span data-ttu-id="0e6e5-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e6e5-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="0e6e5-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e6e5-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->