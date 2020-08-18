---
title: Удаление teamsApp
description: 'Удаление приложения Teams из каталога приложений организации (Каталог приложений клиента). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 432af0167562d34ca006b05901ad5fcb7529a51c
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790499"
---
# <a name="delete-teamsapp"></a>Удаление teamsApp

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (Каталог приложений клиента). Чтобы удалить приложение, свойство **distributionMethod** для приложения должно иметь значение `organization` .

Вы также можете использовать этот API для удаления отправленного приложения из процесса проверки.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Примечание:** Только глобальные администраторы могут вызывать этот API. 

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL |
| Делегированные (рабочая или учебная учетная запись) | CamlQuery. оправить |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

Удаление приложения из каталога приложений:

```http
DELETE /appCatalogs/teamsApps/{id}
```

Чтобы удалить приложение, которое было отправлено, но еще не утверждено:

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

>**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите удалить. Не используйте идентификатор из манифеста пакета приложения ZIP.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
