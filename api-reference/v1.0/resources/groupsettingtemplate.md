<span data-ttu-id="5d26e-p102">Уникальный идентификатор шаблона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d26e-p102">Unique identifier for the subscription. Read-only.</span></span>| Уникальный идентификатор шаблона. Только для чтения.|
|<span data-ttu-id="5d26e-131">values</span><span class="sxs-lookup"><span data-stu-id="5d26e-131">values</span></span>|<span data-ttu-id="5d26e-132">Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="5d26e-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="5d26e-133">Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.</span><span class="sxs-lookup"><span data-stu-id="5d26e-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5d26e-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d26e-134">Relationships</span></span>

<span data-ttu-id="5d26e-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5d26e-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5d26e-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d26e-136">JSON representation</span></span>

<span data-ttu-id="5d26e-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d26e-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->