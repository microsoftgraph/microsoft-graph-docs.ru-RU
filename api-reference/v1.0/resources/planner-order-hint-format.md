---
title: Использование подсказок порядка в Планировщике
description: '`)'
author: TarkanSevilmis
ms.openlocfilehash: 17aee5f0a867f086ff8171bb3a7f8609526bf1ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304006"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="3bbbd-103">Использование подсказок порядка в Планировщике</span><span class="sxs-lookup"><span data-stu-id="3bbbd-103">Using order hints in Planner</span></span>

<span data-ttu-id="3bbbd-p101">Порядок сортировки объектов в Планировщике определяется подсказками порядка. Значения подсказок порядка — строки. Чтобы определить порядок следования элементов, клиенты могут сортировать эти строки по порядковому значению символов в них. Сравниваются символы с начала строки и до тех пор, пока не будет обнаружена разница в порядковом значении символов, либо пока одна из строк не закончится — в таком случае короткая строка будет расположена выше длинной. Значения могут содержать любой символ с порядковым номером от 32 (пробел) до 126 (`~`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-p101">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="3bbbd-p102">Например, элемент с подсказкой порядка `a` (порядковый номер 97) будет размещен выше элемента с подсказкой порядка `z` (порядковый номер 122). Элемент с подсказкой порядка `abc` (порядковые номера 97, 98, 99) будет размещен выше элемента с подсказкой порядка `abd` (порядковые номера 97, 98, 100). Элемент с подсказкой порядка `a` будет размещен выше элемента с подсказкой порядка `ab`, так как все существующие знаки совпадают, а `a` короче.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-p102">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="3bbbd-p103">Значения для всех подсказок порядка вычисляет служба. Клиент может изменить расположение элементов, указав для определенного элемента подсказку порядка, которая переместит его между двумя указанными элементами. Для этого необходимо задать такое значение подсказки порядка: `<previous order hint> <next order hint>!` (где `<previous order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного перед целевым местом, а `<next order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного после целевого места). Между этими значениями ставится пробел, а в конце значения указывается суффикс `!`. Если предыдущий или предшествующий элемент не существует, вместо него следует указать пустую строку. Значение также можно составить на основе проведенных ранее расчетов. Кроме того, клиент может использовать это значение для сортировки элементов в порядке возвращения подсказок порядка. После того как клиент отправит эти значения в обновлении, служба вычислит короткое значение, которое поможет выполнить сортировку.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-p103">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

<span data-ttu-id="3bbbd-118">**Обратите внимание**: в следующих примерах значения подсказки порядка приведены в одинарных кавычках (`'`) для наглядности, однако кавычки не являются частью данных и не должны отправляться в службу.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-118">**Please note** that in the following examples the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="3bbbd-119">Рассмотрим следующий список подсказок порядка сортировки.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-119">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="3bbbd-120">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-120">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="3bbbd-121">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-121">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="3bbbd-122">Расположите элемент 3 перед элементом 1, а затем поместите элемент 4 между элементами 1 и 2. Затем поместите элемент 5 после элемента 2. В клиенте будут созданы следующие подсказки порядка.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-122">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="3bbbd-123">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-123">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="3bbbd-124">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-124">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="3bbbd-125">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-125">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="3bbbd-126">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-126">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="3bbbd-127">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-127">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="3bbbd-128">Затем переместите элемент 1 в конец списка. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-128">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="3bbbd-129">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-129">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="3bbbd-130">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-130">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="3bbbd-131">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-131">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="3bbbd-132">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-132">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="3bbbd-133">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-133">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="3bbbd-134">Поместите элемент 5 между элементами 3 и 4. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-134">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="3bbbd-135">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-135">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="3bbbd-136">Элемент 5 (подсказка порядка: `' 5637! 5637 adhg!!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-136">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="3bbbd-137">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-137">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="3bbbd-138">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-138">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="3bbbd-139">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-139">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="3bbbd-p104">После того как эти изменения значений подсказок порядка будут отправлены в службу с помощью запросов Patch, служба рассчитает правильные значения, соответствующие порядку следования, предусмотренному клиентом. Клиент может получить эти значения немедленно, если в запросах `PATCH` указана настройка `return=representation`. Значения для указанного выше случая могут выглядеть следующим образом (фактические значения могут отличаться).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-p104">Once these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client. The client can obtain the values immediate if `return=representation` preference is specified in the `PATCH` requests. The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="3bbbd-143">Элемент 3 (подсказка порядка: `'432b'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-143">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="3bbbd-144">Элемент 5 (подсказка порядка: `'6F"#'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-144">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="3bbbd-145">Элемент 4 (подсказка порядка: `'7A$6'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-145">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="3bbbd-146">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-146">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="3bbbd-147">Элемент 1 (подсказка порядка: `'de5%'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-147">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="3bbbd-p105">Для создания первого элемента в списке можно использовать значение подсказки порядка ` !`, так как ни предыдущий, ни следующий элемент в таком случае не существуют. Но это не обязательно, так как служба автоматически создаст значения для всех подсказок порядка, если они не указаны во время создания элемента. В следующем примере показаны подсказки порядка, которые следует использовать для добавления элементов в пустой список. Добавьте первый элемент:</span><span class="sxs-lookup"><span data-stu-id="3bbbd-p105">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="3bbbd-151">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-151">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="3bbbd-152">Добавьте второй элемент вверху:</span><span class="sxs-lookup"><span data-stu-id="3bbbd-152">Add the second item to top:</span></span>

1. <span data-ttu-id="3bbbd-153">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-153">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="3bbbd-154">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-154">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="3bbbd-155">Добавьте третий элемент внизу.</span><span class="sxs-lookup"><span data-stu-id="3bbbd-155">Add the third item to bottom:</span></span>

1. <span data-ttu-id="3bbbd-156">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-156">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="3bbbd-157">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-157">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="3bbbd-158">Элемент 3 (подсказка порядка: `' ! !'`).</span><span class="sxs-lookup"><span data-stu-id="3bbbd-158">Item 3 (Order Hint: `' ! !'`)</span></span>







