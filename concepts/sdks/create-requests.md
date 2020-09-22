---
title: Выполнение вызовов API с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию HTTP-запросов Microsoft Graph с помощью пакетов SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: f317b52393378231fb57f2c39c9b9701a9215cf4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193025"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Выполнение вызовов API с помощью пакетов SDK Microsoft Graph

Библиотеки службы SDK Microsoft Graph предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API. Существует два стиля клиентского класса: один использует интерфейс Fluent для создания запроса (например, `client.Users["user-id"].Manager` ), а другой принимает строку пути (например, `api("/users/user-id/manager")` ). Когда у вас есть объект Request, вы можете указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.

Кроме того, существует [пакет SDK Microsoft Graph PowerShell](../powershell/get-started.md), в котором нет клиентского класса. Вместо этого все запросы представлены в виде команд PowerShell. Например, для получения сведений о руководителе пользователя используется команда `Get-MgUserManager` . Дополнительные сведения о поиске команд для вызовов API приведены [в статье Навигация по пакету SDK для Microsoft Graph PowerShell](../powershell/navigating.md).

## <a name="read-information-from-microsoft-graph"></a>Чтение информации из Microsoft Graph

Чтобы прочитать данные из Microsoft Graph, сначала необходимо создать объект Request, а затем выполнить `GET` метод для запроса.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>Использование $select для управления возвращаемыми свойствами

При получении объекта автоматически извлекаются не все свойства; Иногда они должны быть явно выбраны. Кроме того, в некоторых случаях не требуется возвращать набор свойств по умолчанию. Выбор только обязательных свойств может увеличить производительность запроса. Вы можете настроить запрос на включение `$select` параметра запроса в список свойств.

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>Получение списка объектов

Получение списка сущностей аналогично получению одного объекта, за исключением ряда других вариантов настройки запроса. `$filter`Параметр Query можно использовать, чтобы уменьшить набор результатов до тех строк, которые соответствуют заданному условию.  `$orderBy`Параметр запроса будет запрашивать, чтобы сервер предоставил список сущностей, отсортированных по указанным свойствам.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

Объект, возвращаемый при получении списка сущностей, скорее всего, является страничной коллекцией. Сведения о том, как получить полный список сущностей, можно найти в разделе [paging a Collection](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Доступ к элементу коллекции

Для пакетов SDK, поддерживающих стиль Fluent, доступ к коллекциям сущностей можно получить с помощью индекса массива. Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути, следующий за коллекцией. Для PowerShell идентификаторы передаются в качестве параметров.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>Использование $expand для доступа к связанным сущностям

С помощью фильтра можно `$expand` запрашивать связанную сущность или коллекцию сущностей, которые запрашивают основной объект.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>Удаление объекта

Запросы DELETE создаются так же, как запросы на получение объекта, но `DELETE` вместо него используется запрос `GET` .

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Создание запроса POST для создания нового объекта

Для пакетов SDK, поддерживающих стиль Fluent, новые элементы можно добавлять в коллекции с помощью `Add` метода. В пакетах SDK на основе шаблонов объект Request предоставляет `post` метод. Для PowerShell `New-*` доступна команда, принимающая параметры, сопоставленные с добавляемой сущностью. Созданная сущность обычно возвращается из вызова.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>Обновление существующей сущности с помощью исправления

Большинство обновлений в Microsoft Graph выполняются с помощью `PATCH` метода, поэтому необходимо включить в передаваемый объект только те свойства, которые нужно изменить.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>Использование заголовков HTTP для управления поведением запроса

Вы можете использовать `Header()` функцию для присоединения пользовательских заголовков к запросу. Для PowerShell Добавление заголовков возможно только в `Invoke-GraphRequest` методе. В некоторых сценариях Microsoft Graph для настройки поведения запроса используются настраиваемые заголовки.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>Предоставление настраиваемых параметров запроса

Для пакетов SDK, поддерживающих стиль Fluent, можно указать настраиваемые значения параметров запроса с помощью списка `QueryOptions` объектов. Для пакетов SDK на основе шаблонов параметры кодируются в URL-адресе и добавляются в URI запроса. Для PowerShell определенные параметры запроса для данного API предоставляются в виде параметров для соответствующей команды.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
