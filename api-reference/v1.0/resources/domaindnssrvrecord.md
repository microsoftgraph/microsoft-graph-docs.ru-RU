<span data-ttu-id="ed053-p105">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="ed053-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span>| Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null. |
|<span data-ttu-id="ed053-149">weight</span><span class="sxs-lookup"><span data-stu-id="ed053-149">weight</span></span>|<span data-ttu-id="ed053-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ed053-150">Int32</span></span>| <span data-ttu-id="ed053-151">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ed053-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <span data-ttu-id="ed053-152">Связи</span><span class="sxs-lookup"><span data-stu-id="ed053-152">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="ed053-153">Нет</span><span class="sxs-lookup"><span data-stu-id="ed053-153">None</span></span>


## <span data-ttu-id="ed053-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed053-154">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="ed053-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed053-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->