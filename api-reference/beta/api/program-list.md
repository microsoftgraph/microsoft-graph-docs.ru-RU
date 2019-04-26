---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
ms.openlocfilehash: 6200cfe9a2f9879b5589c52cd9f48b4cfa2253ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337265"
---
# <a name="list-programs"></a>Список программ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL  |

 Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не следует предоставлять текст запроса.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Програмконтролс программы](program-listcontrols.md) |     Коллекция [програмконтрол](../resources/programcontrol.md)|    Получение коллекции элементов управления программы.|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
