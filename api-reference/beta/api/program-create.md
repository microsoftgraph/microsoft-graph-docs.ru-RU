---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 33b55ddec6da5351d59c1c5cda32a156e8b0a3e2
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123195"
---
# <a name="create-program"></a>Создание программы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | ProgramControl.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании программы.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  Имя программы.                   |
| `description`               |`String`                              |  Описание программы.           |


## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список программ](program-list.md) | Коллекция [Program](../resources/program.md)|  Получение коллекции всех программ.|
|[Список Програмконтролс программы](program-listcontrols.md) |     Коллекция [програмконтрол](../resources/programcontrol.md)|    Получение коллекции элементов управления программы.|
|[Программа обновления](program-update.md) |  [Программа](../resources/program.md)| Обновление программы.|
|[Создание Програмконтрол](programcontrol-create.md) |        [програмконтрол](../resources/programcontrol.md)    |   Добавление Програмконтрол в программу.|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
