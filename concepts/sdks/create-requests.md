---
title: Вызовы API с помощью SDKs Graph Microsoft
description: Содержит инструкции по созданию Graph http-запросов с помощью SDKs.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: d8b7233fb360b3dd5bba088c6d193a6bac18f304
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695386"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a>Вызовы API с помощью SDKs Graph Microsoft

Библиотеки служб майкрософт Graph SDK предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API. Существует два стиля клиентского класса: один использует беглое интерфейс для создания запроса (например, ) и другой принимает строку пути `client.Users["user-id"].Manager` (например, `api("/users/user-id/manager")` ). Если у вас есть объект запроса, можно указать различные параметры, такие как фильтрация и сортировка, и, наконец, вы выберите тип операции, который необходимо выполнить.

Существует также microsoft [Graph PowerShell SDK,](../powershell/get-started.md)который не имеет клиентского класса вообще. Вместо этого все запросы представлены в качестве команд PowerShell. Например, чтобы получить менеджера пользователя, команда `Get-MgUserManager` . Дополнительные сведения о поиске команд для вызовов API см. в обзоре [Navigating the Microsoft Graph PowerShell SDK.](../powershell/navigating.md)

## <a name="read-information-from-microsoft-graph"></a>Ознакомьтесь с информацией из Microsoft Graph

Чтобы прочитать сведения из microsoft Graph, сначала необходимо создать объект запроса, а затем запустить `GET` метод по запросу.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a>Использование $select для управления возвращенными свойствами

При извлечении объекта не все свойства автоматически извлекаются; иногда они должны быть явно выбраны. Кроме того, в некоторых сценариях нет необходимости возвращать набор свойств по умолчанию. Выбор только необходимых свойств может повысить производительность запроса. Вы можете настроить запрос, чтобы включить параметр `$select` запроса со списком свойств.

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a>Извлечение списка сущностями

Ирисовка списка сущностей похожа на ирисовку одной сущности, за исключением ряда других вариантов настройки запроса. Параметр запроса можно использовать для уменьшения заданного результата только до тех строк, которые соответствуют `$filter` условию.  Параметр запроса запрашивает, чтобы сервер предоставил список объектов, `$orderBy` сортироваться по указанным свойствам.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

Объект, возвращающийся при сборе списка сущностями, скорее всего, будет страницей коллекции. Сведения о том, как получить полный список сущностях, см. в материале [paging through a collection.](../paging.md)

## <a name="access-an-item-of-a-collection"></a>Доступ к элементу коллекции

Для SDKs, поддерживаюющих беглое использование стиля, можно получить доступ к коллекциям сущностям с помощью индекса массива. Для SDKs на основе шаблонов достаточно встраить идентификатор элемента в сегмент пути, следующий за коллекцией. Для PowerShell идентификаторы передаются в качестве параметров.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a>Использование $expand для доступа к связанным сущностям

Фильтр можно использовать для запроса связанной сущности или коллекции сущностей одновременно с запросом `$expand` основного объекта.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a>Удаление объекта

Удаление запросов строится так же, как и запросы на извлечение объекта, но вместо `DELETE` запроса используется `GET` .

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a>Создание запроса POST для создания нового объекта

Для SDKs, которые поддерживают беглое стиле, новые элементы могут быть добавлены в коллекции с помощью `Add` метода. Для SDKs на основе шаблонов объект запроса предоставляет `post` метод. Для PowerShell доступна команда, которая принимает параметры, которые необходимо добавить в `New-*` объект. Созданная сущность обычно возвращается из вызова.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a>Обновление существующей сущности с помощью PATCH

Большинство обновлений в Microsoft Graph выполняются с помощью метода, поэтому необходимо включать только свойства, которые необходимо изменить в `PATCH` переданном объекте.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a>Использование http-заглавок для управления поведением запросов

Вы можете использовать `Header()` функцию для прикрепления настраиваемой заготки к запросу. Для PowerShell добавление загона возможно только с помощью `Invoke-GraphRequest` метода. В ряде Graph Майкрософт для настройки поведения запроса используются настраиваемые заготки.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a>Предоставление настраиваемой параметров запроса

Для SDKs, которые поддерживают беглое стиле, можно предоставить настраиваемые значения параметров запроса с помощью списка `QueryOptions` объектов. Для SDKs на основе шаблонов параметры кодируются URL-адресами и добавляются в URI запроса. Для PowerShell определенные параметры запроса для данного API выставляются в качестве параметров соответствующей команды.

# <a name="c"></a>[C#](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[TypeScript](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
