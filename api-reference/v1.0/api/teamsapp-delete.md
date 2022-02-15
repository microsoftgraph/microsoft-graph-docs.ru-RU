---
title: Удаление teamsApp
description: 'Удаление Teams приложения из каталога приложений организации (каталог приложений клиента). '
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0be663b84f624d0b3650c5baf6859e580fafc380
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62803956"
---
# <a name="delete-teamsapp"></a>Удаление teamsApp

Пространство имен: microsoft.graph

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a>Удаление приложения из каталога приложений организации

Удаление [приложения из](../resources/teamsapp.md) каталога приложений организации (каталога приложений клиента). Чтобы удалить приложение, необходимо задать свойство **distributionMethod** для приложения `organization`.

Этот API также можно использовать для удаления отправленного приложения из процесса проверки.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Только глобальные администраторы могут вызывать этот API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись) | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All** |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается. |

> **Примечание**. Разрешения, отмеченные **, поддерживаются только для обратной совместимости. Мы рекомендуем обновить решения, чтобы использовать альтернативное разрешение, перечисленное в предыдущей таблице, и избегать использования этих разрешений в будущем.

## <a name="http-request"></a>HTTP-запрос

Удаление приложения из каталога приложений:

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

Удаление приложения, которое было отправлено, но не утверждено:

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

>**Примечание:** Используйте ID, возвращенный из вызова [опубликованных приложений Списка](./appcatalogs-list-teamsapps.md) , для ссылки на приложение, которое вы хотите удалить. Не используйте ID из манифеста пакета почтовых приложений.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-teamsapp-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-teamsapp-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

