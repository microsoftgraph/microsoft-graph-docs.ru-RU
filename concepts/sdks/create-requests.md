---
title: Выполнение вызовов API с помощью пакетов SDK Graph Майкрософт
description: Содержит инструкции по созданию запросов Microsoft Graph HTTP с помощью пакетов SDK.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: 49be5a3fdb2ead7e8e3a4d39b459b7ef068a9a74
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848694"
---
<!-- markdownlint-disable MD025 -->

# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Выполнение вызовов API с помощью пакетов SDK Graph Майкрософт

Библиотеки служб microsoft Graph SDK предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API. Существует два стиля клиентского класса: один использует текучий интерфейс для создания запроса (например, `client.Users["user-id"].Manager`) и другой принимает строку пути (например, `api("/users/user-id/manager")`). При наличии объекта запроса можно указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.

Также существует пакет [SDK Microsoft Graph PowerShell](/powershell/microsoftgraph/get-started.md), который не имеет клиентского класса. Вместо этого все запросы представлены в виде команд PowerShell. Например, чтобы получить руководителя пользователя, выполните следующую команду `Get-MgUserManager`: Дополнительные сведения о поиске команд для вызовов API см. в статье "Навигация по [пакету SDK Microsoft Graph PowerShell"](/powershell/microsoftgraph/navigating.md).

## <a name="read-information-from-microsoft-graph"></a>Чтение сведений из microsoft Graph

Чтобы прочитать сведения из microsoft Graph, сначала необходимо создать объект `GET` запроса, а затем запустить метод в запросе.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>Использование $select для управления возвращаемых свойствами

При извлечении сущности не все свойства извлекаются автоматически; Иногда их необходимо выбрать явным образом. Кроме того, в некоторых сценариях нет необходимости возвращать набор свойств по умолчанию. Выбор только необходимых свойств может повысить производительность запроса. Вы можете настроить запрос, чтобы включить параметр `$select` запроса в список свойств.

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>Получение списка сущностей

Получение списка сущностей аналогично получению одной сущности, за исключением ряда других вариантов настройки запроса. Параметр `$filter` запроса можно использовать для уменьшения результирующего набора до тех строк, которые соответствуют указанному условию.  Параметр `$orderBy` запроса запрашивает у сервера список сущностей, отсортированных по указанным свойствам.

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-list.md)]

---

Объект, возвращаемый при получении списка сущностей, скорее всего, является коллекцией страниц. Дополнительные сведения о том, как получить полный список сущностей, см. в подкачки [по коллекции](../paging.md).

## <a name="access-an-item-of-a-collection"></a>Доступ к элементу коллекции

Для пакетов SDK, поддерживающих текучий стиль, доступ к коллекциям сущностей можно получить с помощью индекса массива. Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути после коллекции. Для PowerShell идентификаторы передаются в качестве параметров.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>Использование $expand для доступа к связанным сущностям

Фильтр можно использовать `$expand` для запроса связанной сущности или коллекции сущностей одновременно с запросом основной сущности.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>Удаление сущности

Запросы на удаление создаются так же, как запросы на получение сущности, `DELETE` `GET`но используют запрос вместо .

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Выполнение запроса POST для создания новой сущности

Для пакетов SDK, поддерживающих текучий стиль, новые элементы можно добавлять в коллекции с помощью `Add` метода. Для пакетов SDK на основе шаблонов объект запроса предоставляет `post` метод. Для PowerShell доступна команда `New-*` , которая принимает параметры, которые сопоставляются с добавляемой сущностью. Созданная сущность обычно возвращается из вызова.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>Обновление существующей сущности с помощью PATCH

Большинство обновлений в Microsoft Graph `PATCH` выполняются с помощью метода, поэтому необходимо включать только свойства, которые необходимо изменить в передаваемом объекте.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>Использование заголовков HTTP для управления поведением запросов

Функцию можно использовать `Header()` для прикрепления пользовательских заголовков к запросу. Для PowerShell добавление заголовков возможно только с помощью `Invoke-GraphRequest` метода. В некоторых сценариях microsoft Graph настраиваемые заголовки используются для настройки поведения запроса.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>Предоставление пользовательских параметров запроса

Для пакетов SDK, поддерживающих текучий стиль, можно указать пользовательские значения параметров запроса с помощью списка `QueryOptions` объектов. Для пакетов SDK на основе шаблонов параметры кодируются в URL-адресе и добавляются в URI запроса. Для PowerShell и Go определенные параметры запроса для заданного API предоставляются в качестве параметров для соответствующей команды.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

[!INCLUDE [sample-code](includes/snippets/go/create-requests-queryparams.md)]

---
