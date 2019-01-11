---
title: Создание программы
description: В Azure AD доступа к функции проверки, создайте новый объект.
localization_priority: Normal
ms.openlocfilehash: b982242bbdddb9769d64c9757d9041fddc215d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844018"
---
# <a name="create-program"></a>Создание программы

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте [новый объект](../resources/program.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `ProgramControl.ReadWrite.All`.  Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .

Ниже приведены свойства, которые необходимы для создания программы.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  Имя программы.                   |
| `description`               |`String`                              |  Описание программы.           |


## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201, Created` объект [программы](../resources/program.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса укажите представление объекта [программы](../resources/program.md) с JSON.

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

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
|[Список программ](program-list.md) | [программа](../resources/program.md) семейства сайтов|  Получите коллекцию всех программ.|
|[Список programControls программы](program-listcontrols.md) |     [programControl](../resources/programcontrol.md) коллекции|    Получите коллекцию элементов управления из программы.|
|[Обновите программу](program-update.md) |  [Программа](../resources/program.md)| Обновите программу.|
|[Создание programControl](programcontrol-create.md) |        [programControl](../resources/programcontrol.md)    |   Добавьте programControl программы.|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
