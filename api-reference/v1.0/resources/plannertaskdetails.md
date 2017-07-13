<span data-ttu-id="70099-p103">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="70099-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.|
|<span data-ttu-id="70099-135">references</span><span class="sxs-lookup"><span data-stu-id="70099-135">references</span></span>|[<span data-ttu-id="70099-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="70099-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="70099-137">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="70099-137">The collection of references on the task.</span></span>|

## <span data-ttu-id="70099-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="70099-138">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="70099-139">Нет</span><span class="sxs-lookup"><span data-stu-id="70099-139">None</span></span>


## <span data-ttu-id="70099-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70099-140">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="70099-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70099-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->