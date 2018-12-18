---
title: Использование подсказок порядка в Планировщике
description: '`)'
author: TarkanSevilmis
ms.openlocfilehash: a89568a7b5204aef199a948e63a092219186aba8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328786"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="fd024-103">Использование подсказок порядка в Планировщике</span><span class="sxs-lookup"><span data-stu-id="fd024-103">Using order hints in Planner</span></span>

> <span data-ttu-id="fd024-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd024-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd024-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd024-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd024-p102">Порядок сортировки объектов в Планировщике определяется подсказками порядка. Значения подсказок порядка — строки. Чтобы определить порядок следования элементов, клиенты могут сортировать эти строки по порядковому значению символов в них. Сравниваются символы с начала строки и до тех пор, пока не будет обнаружена разница в порядковом значении символов, либо пока одна из строк не закончится — в таком случае короткая строка будет расположена выше длинной. Значения могут содержать любой символ с порядковым номером от 32 (пробел) до 126 (`~`).</span><span class="sxs-lookup"><span data-stu-id="fd024-p102">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="fd024-p103">Например, элемент с подсказкой порядка `a` (порядковый номер 97) будет размещен выше элемента с подсказкой порядка `z` (порядковый номер 122). Элемент с подсказкой порядка `abc` (порядковые номера 97, 98, 99) будет размещен выше элемента с подсказкой порядка `abd` (порядковые номера 97, 98, 100). Элемент с подсказкой порядка `a` будет размещен выше элемента с подсказкой порядка `ab`, так как все существующие знаки совпадают, а `a` короче.</span><span class="sxs-lookup"><span data-stu-id="fd024-p103">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="fd024-p104">Значения для всех подсказок порядка вычисляет служба. Клиент может изменить расположение элементов, указав для определенного элемента подсказку порядка, которая переместит его между двумя указанными элементами. Для этого необходимо задать такое значение подсказки порядка: `<previous order hint> <next order hint>!` (где `<previous order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного перед целевым местом, а `<next order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного после целевого места). Между этими значениями ставится пробел, а в конце значения указывается суффикс `!`. Если предыдущий или предшествующий элемент не существует, вместо него следует указать пустую строку. Значение также можно составить на основе проведенных ранее расчетов. Кроме того, клиент может использовать это значение для сортировки элементов в порядке возвращения подсказок порядка. После того как клиент отправит эти значения в обновлении, служба вычислит короткое значение, которое поможет выполнить сортировку.</span><span class="sxs-lookup"><span data-stu-id="fd024-p104">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="fd024-120">**Примечание:** В следующих примерах значения подсказку фактический порядке заключенной в одинарные кавычки символов (`'`) для ясности, тем не менее эти не являющихся частью данных и не должны будут отправляться в службу.</span><span class="sxs-lookup"><span data-stu-id="fd024-120">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="fd024-121">Рассмотрим следующий список подсказок порядка сортировки.</span><span class="sxs-lookup"><span data-stu-id="fd024-121">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="fd024-122">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-122">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="fd024-123">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-123">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="fd024-124">Расположите элемент 3 перед элементом 1, а затем поместите элемент 4 между элементами 1 и 2. Затем поместите элемент 5 после элемента 2. В клиенте будут созданы следующие подсказки порядка.</span><span class="sxs-lookup"><span data-stu-id="fd024-124">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="fd024-125">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-125">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="fd024-126">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-126">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="fd024-127">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-127">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="fd024-128">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-128">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="fd024-129">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-129">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="fd024-130">Затем переместите элемент 1 в конец списка. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="fd024-130">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="fd024-131">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-131">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="fd024-132">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-132">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="fd024-133">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-133">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="fd024-134">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-134">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="fd024-135">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-135">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="fd024-136">Поместите элемент 5 между элементами 3 и 4. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="fd024-136">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="fd024-137">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-137">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="fd024-138">Элемент 5 (подсказка порядка: `' 5637! 5637 adhg!!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-138">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="fd024-139">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-139">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="fd024-140">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-140">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="fd024-141">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-141">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="fd024-142">При отправке эти изменения значений подсказку порядке службы запросов исправлений в службе будет рассчитываться соответствующие значения, которые сохранить порядок, предназначен клиентом.</span><span class="sxs-lookup"><span data-stu-id="fd024-142">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="fd024-143">Клиент мог получать значения непосредственно в том случае, если `Prefer: return=representation` предпочтения заголовок, заданный в `PATCH` запросов.</span><span class="sxs-lookup"><span data-stu-id="fd024-143">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="fd024-144">Значения для указанного выше случая могут выглядеть следующим образом (фактические значения могут отличаться).</span><span class="sxs-lookup"><span data-stu-id="fd024-144">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="fd024-145">Элемент 3 (подсказка порядка: `'432b'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-145">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="fd024-146">Элемент 5 (подсказка порядка: `'6F"#'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-146">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="fd024-147">Элемент 4 (подсказка порядка: `'7A$6'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-147">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="fd024-148">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-148">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="fd024-149">Элемент 1 (подсказка порядка: `'de5%'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-149">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="fd024-p106">Для создания первого элемента в списке можно использовать значение подсказки порядка ` !`, так как ни предыдущий, ни следующий элемент в таком случае не существуют. Но это не обязательно, так как служба автоматически создаст значения для всех подсказок порядка, если они не указаны во время создания элемента. В следующем примере показаны подсказки порядка, которые следует использовать для добавления элементов в пустой список. Добавьте первый элемент:</span><span class="sxs-lookup"><span data-stu-id="fd024-p106">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="fd024-153">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-153">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="fd024-154">Добавьте второй элемент вверху:</span><span class="sxs-lookup"><span data-stu-id="fd024-154">Add the second item to top:</span></span>

1. <span data-ttu-id="fd024-155">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-155">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="fd024-156">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-156">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="fd024-157">Добавьте третий элемент внизу.</span><span class="sxs-lookup"><span data-stu-id="fd024-157">Add the third item to bottom:</span></span>

1. <span data-ttu-id="fd024-158">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-158">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="fd024-159">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-159">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="fd024-160">Элемент 3 (подсказка порядка: `' ! !'`).</span><span class="sxs-lookup"><span data-stu-id="fd024-160">Item 3 (Order Hint: `' ! !'`)</span></span>







