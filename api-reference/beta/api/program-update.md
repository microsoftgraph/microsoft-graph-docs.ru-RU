---
title: Программа обновления
description: В функции проверки доступа Azure AD обновите существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538549"
---
# <a name="update-program"></a>Программа обновления

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `ProgramControl.ReadWrite.All`.  Пользователь, вошедшего в систему, также должен находиться в роли каталога, что позволяет им обновлять программу. |
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
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.

В следующей таблице приведены свойства, которые можно указать при обновлении программы.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  Имя программы.                   |
| `description`               |`String`                              |  Описание программы.           |


## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [Program](../resources/program.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [программы](../resources/program.md) , который необходимо изменить, в формате JSON.

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
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
|[Список Програмконтролс программы](program-listcontrols.md) |     Коллекция [програмконтрол](../resources/programcontrol.md)|    Получение коллекции элементов управления программы.|
|[Создание Програмконтрол](programcontrol-create.md) |        [Програмконтрол](../resources/programcontrol.md)    |   Добавление Програмконтрол в программу.|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
