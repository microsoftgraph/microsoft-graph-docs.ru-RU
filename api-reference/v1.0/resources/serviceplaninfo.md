<span data-ttu-id="c241b-p103">Объект, которому может быть назначен план обслуживания. Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="c241b-p103">The object the service plan can be assigned to. Possible values:</span></span>|Объект, которому может быть назначен план обслуживания. Возможные значения:<br/><span data-ttu-id="c241b-127">"User" — план обслуживания можно назначить отдельным пользователям.</span><span class="sxs-lookup"><span data-stu-id="c241b-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="c241b-128">"Company" — план обслуживания можно назначить всему клиенту.</span><span class="sxs-lookup"><span data-stu-id="c241b-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c241b-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c241b-129">JSON representation</span></span>

<span data-ttu-id="c241b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c241b-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
