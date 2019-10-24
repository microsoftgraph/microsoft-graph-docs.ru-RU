---
title: Выполнение вызовов API с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию HTTP-запросов Microsoft Graph с помощью пакетов SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653519"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Выполнение вызовов API с помощью пакетов SDK Microsoft Graph

Библиотеки службы SDK Microsoft Graph предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API. Существует два стиля клиентского класса: один использует интерфейс Fluent для создания запроса (например, `client.Me.Manager`), а другой принимает строку пути (например, `api("/me/manager")`). Когда у вас есть объект Request, вы можете указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.

## <a name="read-information-from-microsoft-graph"></a>Чтение информации из Microsoft Graph

Чтобы прочитать данные из Microsoft Graph, сначала необходимо создать объект Request, а затем выполнить `GET` метод для запроса.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a>Использование $select для управления возвращаемыми свойствами

При получении объекта автоматически извлекаются не все свойства; Иногда они должны быть явно выбраны. Кроме того, в некоторых случаях не требуется возвращать набор свойств по умолчанию. Выбор только обязательных свойств может увеличить производительность запроса. Вы можете настроить объект *request* так, чтобы он `$select` выдать параметр запроса с помощью списка свойств.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a>Получение списка объектов

Получение списка сущностей аналогично получению одного объекта, за исключением ряда других вариантов настройки запроса. Параметр `$filter` Query можно использовать, чтобы уменьшить набор результатов до тех строк, которые соответствуют заданному условию.  Параметр `$orderBy` запроса будет запрашивать, чтобы сервер предоставил список сущностей, отсортированных по указанным свойствам.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

Объект, возвращаемый при получении списка сущностей, скорее всего, является страничной коллекцией. Сведения о том, как получить полный список сущностей, можно найти в разделе [paging a Collection](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Доступ к элементу коллекции

Для пакетов SDK, поддерживающих стиль Fluent, доступ к коллекциям сущностей можно получить с помощью индекса массива. Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути, следующий за коллекцией.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a>Использование $expand для доступа к связанным сущностям

С помощью `$expand` фильтра можно запрашивать связанную сущность или коллекцию сущностей, которые запрашивают основной объект.  `Expand()` Функция в объекте *request* добавляет необходимый параметр запроса.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a>Удаление объекта

Чтобы удалить сущность, создайте *запрос* так же, как и для получения объекта. Метод *Delete* объекта *request* указывает на необходимость удаления объекта.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Создание запроса POST для создания нового объекта

Чтобы создать новый объект в коллекции, вызовите метод `add` или `post` и передайте объект, содержащий сведения, которые будут использоваться для создания нового объекта. Обновленная версия созданной сущности обычно возвращается при вызове.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a>Обновление существующей сущности с помощью исправления

Большинство обновлений в Microsoft Graph выполняются с помощью `PATCH` метода, поэтому необходимо включить в передаваемый объект только те свойства, которые нужно изменить.  

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a>Использование заголовков HTTP для управления поведением запроса

Вы можете использовать `header()` функцию для присоединения пользовательских заголовков к запросу. В некоторых сценариях Microsoft Graph для настройки поведения запроса используются настраиваемые заголовки.
 
# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a>Предоставление настраиваемых параметров запроса

В ситуациях, когда вызов API позволяет использовать пользовательские параметры запроса, можно предоставить эти значения параметров с помощью списка `QueryOptions` объектов.

# <a name="ctabcs"></a>[C#](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescripttabtypescript"></a>[TypeScript](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
