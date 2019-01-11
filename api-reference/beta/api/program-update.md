---
title: Обновите программу
description: Доступ к функции проверки в Azure AD "," Обновление существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: a9abe10a2a672984d14f1da821b7ae6244cbdf39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840336"
---
# <a name="update-program"></a>Обновите программу

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `ProgramControl.ReadWrite.All`.  Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать обновления программы. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .

В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении программы.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  Имя программы.                   |
| `description`               |`String`                              |  Описание программы.           |


## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `204, Accepted` объект [программы](../resources/program.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса укажите представление JSON параметров объекта [программа](../resources/program.md) для изменения.

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список programControls программы](program-listcontrols.md) |     [programControl](../resources/programcontrol.md) коллекции|    Получите коллекцию элементов управления из программы.|
|[Создание programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   Добавьте programControl программы.|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
