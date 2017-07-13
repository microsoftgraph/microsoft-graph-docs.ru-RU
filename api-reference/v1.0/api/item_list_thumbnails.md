<span data-ttu-id="d9b8e-p105">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.

| <span data-ttu-id="d9b8e-162">Имя</span><span class="sxs-lookup"><span data-stu-id="d9b8e-162">Name</span></span>           | <span data-ttu-id="d9b8e-163">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d9b8e-163">Resolution</span></span>  | <span data-ttu-id="d9b8e-164">Пропорции</span><span class="sxs-lookup"><span data-stu-id="d9b8e-164">Aspect Ratio</span></span> | <span data-ttu-id="d9b8e-165">Описание</span><span class="sxs-lookup"><span data-stu-id="d9b8e-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="d9b8e-166">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="d9b8e-166">96 longest</span></span>  | <span data-ttu-id="d9b8e-167">Исходные</span><span class="sxs-lookup"><span data-stu-id="d9b8e-167">Original</span></span>     | <span data-ttu-id="d9b8e-168">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="d9b8e-169">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="d9b8e-169">176 longest</span></span> | <span data-ttu-id="d9b8e-170">Исходные</span><span class="sxs-lookup"><span data-stu-id="d9b8e-170">Original</span></span>     | <span data-ttu-id="d9b8e-171">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="d9b8e-172">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="d9b8e-172">800 longest</span></span> | <span data-ttu-id="d9b8e-173">Исходные</span><span class="sxs-lookup"><span data-stu-id="d9b8e-173">Original</span></span>     | <span data-ttu-id="d9b8e-174">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <span data-ttu-id="d9b8e-175">Заметки</span><span class="sxs-lookup"><span data-stu-id="d9b8e-175">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="d9b8e-176">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="d9b8e-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="d9b8e-177">С помощью таких вызовов невозможно дополнить коллекцию эскизов: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
