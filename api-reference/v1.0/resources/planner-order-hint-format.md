---
title: Использование подсказок порядка в Планировщике
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 585c8d34a90cf8f567014b763ebeeb9b296c7aae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534045"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="64382-103">Использование подсказок порядка в Планировщике</span><span class="sxs-lookup"><span data-stu-id="64382-103">Using order hints in Planner</span></span>

<span data-ttu-id="64382-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64382-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64382-105">Порядок сортировки объектов в Планировщике определяется подсказками порядка.</span><span class="sxs-lookup"><span data-stu-id="64382-105">Objects in Planner identify their sort order by order hints.</span></span> <span data-ttu-id="64382-106">Значения подсказок порядка — строки.</span><span class="sxs-lookup"><span data-stu-id="64382-106">The order hint values are strings.</span></span> <span data-ttu-id="64382-107">Чтобы определить порядок следования элементов, клиенты могут сортировать эти строки по порядковому значению символов в них.</span><span class="sxs-lookup"><span data-stu-id="64382-107">The clients can sort the strings based on ordinal value of characters in them to identify the order of items.</span></span> <span data-ttu-id="64382-108">Сравниваются символы с начала строки и до тех пор, пока не будет обнаружена разница в порядковом значении символов, либо пока одна из строк не закончится — в таком случае короткая строка будет расположена выше длинной.</span><span class="sxs-lookup"><span data-stu-id="64382-108">The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer.</span></span> <span data-ttu-id="64382-109">Значения могут содержать любой символ с порядковым номером от 32 (пробел) до 126 (`~`).</span><span class="sxs-lookup"><span data-stu-id="64382-109">The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="64382-110">Например, элемент с подсказкой порядка `a` (порядковый номер 97) будет размещен выше элемента с подсказкой порядка `z` (порядковый номер 122).</span><span class="sxs-lookup"><span data-stu-id="64382-110">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122).</span></span> <span data-ttu-id="64382-111">Элемент с подсказкой порядка `abc` (порядковые номера 97, 98, 99) будет размещен выше элемента с подсказкой порядка `abd` (порядковые номера 97, 98, 100).</span><span class="sxs-lookup"><span data-stu-id="64382-111">An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100).</span></span> <span data-ttu-id="64382-112">Элемент с подсказкой порядка `a` будет размещен выше элемента с подсказкой порядка `ab`, так как все существующие знаки совпадают, а `a` короче.</span><span class="sxs-lookup"><span data-stu-id="64382-112">An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="64382-113">Значения для всех подсказок порядка вычисляет служба.</span><span class="sxs-lookup"><span data-stu-id="64382-113">The values for all order hints are calculated by the service.</span></span> <span data-ttu-id="64382-114">Клиент может изменить расположение элементов, указав для определенного элемента подсказку порядка, которая переместит его между двумя указанными элементами. Для этого необходимо задать такое значение подсказки порядка: `<previous order hint> <next order hint>!` (где `<previous order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного перед целевым местом, а `<next order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного после целевого места).</span><span class="sxs-lookup"><span data-stu-id="64382-114">The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location.</span></span> <span data-ttu-id="64382-115">Между этими значениями ставится пробел, а в конце значения указывается суффикс `!`.</span><span class="sxs-lookup"><span data-stu-id="64382-115">There is a space character between these order hint values, and the entire value is suffixed with `!`.</span></span> <span data-ttu-id="64382-116">Если предыдущий или предшествующий элемент не существует, вместо него следует указать пустую строку.</span><span class="sxs-lookup"><span data-stu-id="64382-116">If either item isn't present, empty string should be used instead.</span></span> <span data-ttu-id="64382-117">Значение также можно составить на основе проведенных ранее расчетов. Кроме того, клиент может использовать это значение для сортировки элементов в порядке возвращения подсказок порядка.</span><span class="sxs-lookup"><span data-stu-id="64382-117">This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints.</span></span> <span data-ttu-id="64382-118">После того как клиент отправит эти значения в обновлении, служба вычислит короткое значение, которое поможет выполнить сортировку.</span><span class="sxs-lookup"><span data-stu-id="64382-118">Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

<span data-ttu-id="64382-119">**Обратите внимание**: в следующих примерах значения подсказки порядка приведены в одинарных кавычках (`'`) для наглядности, однако кавычки не являются частью данных и не должны отправляться в службу.</span><span class="sxs-lookup"><span data-stu-id="64382-119">**Please note** that in the following examples the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="64382-120">Рассмотрим следующий список подсказок порядка сортировки.</span><span class="sxs-lookup"><span data-stu-id="64382-120">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="64382-121">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="64382-121">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="64382-122">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="64382-122">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="64382-123">Расположите элемент 3 перед элементом 1, а затем поместите элемент 4 между элементами 1 и 2. Затем поместите элемент 5 после элемента 2. В клиенте будут созданы следующие подсказки порядка.</span><span class="sxs-lookup"><span data-stu-id="64382-123">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="64382-124">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-124">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="64382-125">Элемент 1 (подсказка порядка: `'5637'`).</span><span class="sxs-lookup"><span data-stu-id="64382-125">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="64382-126">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-126">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="64382-127">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="64382-127">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="64382-128">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-128">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="64382-129">Затем переместите элемент 1 в конец списка. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="64382-129">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="64382-130">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-130">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="64382-131">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-131">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="64382-132">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="64382-132">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="64382-133">Элемент 5 (подсказка порядка: `'adhg !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-133">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="64382-134">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-134">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="64382-135">Поместите элемент 5 между элементами 3 и 4. Будут созданы следующие подсказки.</span><span class="sxs-lookup"><span data-stu-id="64382-135">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="64382-136">Элемент 3 (подсказка порядка: `' 5637!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-136">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="64382-137">Элемент 5 (подсказка порядка: `' 5637! 5637 adhg!!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-137">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="64382-138">Элемент 4 (подсказка порядка: `'5637 adhg!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-138">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="64382-139">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="64382-139">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="64382-140">Элемент 1 (подсказка порядка: `'adhg ! !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-140">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="64382-141">После того как эти изменения значений подсказок порядка будут отправлены в службу с помощью запросов Patch, служба рассчитает правильные значения, соответствующие порядку следования, предусмотренному клиентом.</span><span class="sxs-lookup"><span data-stu-id="64382-141">Once these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="64382-142">Клиент может получить эти значения немедленно, если в запросах `PATCH` указана настройка `return=representation`.</span><span class="sxs-lookup"><span data-stu-id="64382-142">The client can obtain the values immediate if `return=representation` preference is specified in the `PATCH` requests.</span></span> <span data-ttu-id="64382-143">Значения для указанного выше случая могут выглядеть следующим образом (фактические значения могут отличаться).</span><span class="sxs-lookup"><span data-stu-id="64382-143">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="64382-144">Элемент 3 (подсказка порядка: `'432b'`).</span><span class="sxs-lookup"><span data-stu-id="64382-144">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="64382-145">Элемент 5 (подсказка порядка: `'6F"#'`).</span><span class="sxs-lookup"><span data-stu-id="64382-145">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="64382-146">Элемент 4 (подсказка порядка: `'7A$6'`).</span><span class="sxs-lookup"><span data-stu-id="64382-146">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="64382-147">Элемент 2 (подсказка порядка: `'adhg'`).</span><span class="sxs-lookup"><span data-stu-id="64382-147">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="64382-148">Элемент 1 (подсказка порядка: `'de5%'`).</span><span class="sxs-lookup"><span data-stu-id="64382-148">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="64382-149">Для создания первого элемента в списке можно использовать значение подсказки порядка `!`, так как ни предыдущий, ни следующий элемент в таком случае не существуют. Но это не обязательно, так как служба автоматически создаст значения для всех подсказок порядка, если они не указаны во время создания элемента.</span><span class="sxs-lookup"><span data-stu-id="64382-149">Order Hints can be specified for creating the first item in the list as `!`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item.</span></span> <span data-ttu-id="64382-150">В следующем примере показаны подсказки порядка, которые следует использовать для добавления элементов в пустой список.</span><span class="sxs-lookup"><span data-stu-id="64382-150">Following example illustrates the order hints should be used when placing items in a previously empty list.</span></span>
<span data-ttu-id="64382-151">Добавьте первый элемент:</span><span class="sxs-lookup"><span data-stu-id="64382-151">Add the first item:</span></span>

1. <span data-ttu-id="64382-152">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-152">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="64382-153">Добавьте второй элемент вверху:</span><span class="sxs-lookup"><span data-stu-id="64382-153">Add the second item to top:</span></span>

1. <span data-ttu-id="64382-154">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-154">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="64382-155">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-155">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="64382-156">Добавьте третий элемент внизу.</span><span class="sxs-lookup"><span data-stu-id="64382-156">Add the third item to bottom:</span></span>

1. <span data-ttu-id="64382-157">Элемент 2 (подсказка порядка: `'  !!'`).</span><span class="sxs-lookup"><span data-stu-id="64382-157">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="64382-158">Элемент 1 (подсказка порядка: `' !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-158">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="64382-159">Элемент 3 (подсказка порядка: `' ! !'`).</span><span class="sxs-lookup"><span data-stu-id="64382-159">Item 3 (Order Hint: `' ! !'`)</span></span>







