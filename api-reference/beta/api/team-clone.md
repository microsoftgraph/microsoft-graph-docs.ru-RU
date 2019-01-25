---
title: Клонирование группы
description: Создайте копию группы. Эта операция также создает копию соответствующей группе.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5ef317d004e3355f9b40fc44232b7c594a3e45a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526167"
---
# <a name="clone-a-team"></a>Клонирование группы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте копию [группы](../resources/team.md). Эта операция также создает копию в соответствующие [группы](../resources/group.md).
Можно определить какие части группы следует скопировать.

- **приложения** - группами Майкрософт копий приложений, установленных в группе. 
- **каналы** — копирует структуру канала (но не сообщения в канале).
- **члены** — копирует участников и владельцев группы.
- **Параметры** — копирует все параметры в рамках рабочей группы, а также параметры ключа группы.
- **вкладки** — копирует вкладок между каналами.

При клонировании вкладок они помещаются в исходное состояние — они отображаются в панели вкладок в группах Microsoft и при первом открытии, вы перейдете через экрана конфигурации. (Если пользователь на вкладке не имеет разрешения для настройки приложения, они появится сообщение о том, что вкладке еще не были настроены.)

Клонирование — это длительная операция.
После возвращает клонированной POST, необходимо получить [операция](../resources/teamsasyncoperation.md) , является ли он «запуск» или «успешно» и «failed». Следует продолжить GET, пока состояние не «выполняется». Рекомендуемые задержки между получает — 5 секунд.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений                            | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classification|String (необязательно)|Описание классификации для группы (например, низкий, средний или высокий для бизнеса). Допустимые значения для этого свойства определены, создав значение [параметра](../resources/directorysetting.md) ClassificationList на основе [определения шаблона](../resources/directorysettingtemplate.md). Если классификация не указан, классификации копируются из исходной группы или группы.|
|description|String (необязательно)|Необязательное описание для группы. Если это свойство не указан, он остается пустым.|
|displayName|Строка|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|mailNickname|String|Почтовый псевдоним для группы (уникальный в организации). Это свойство должно быть указано при создании группы. Поддерживает параметр $filter. Если это свойство не задано, его повторное вычисление из displayName. Известные проблемы: это свойство учитывается.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Список разделенных запятой частей следует скопировать. Юридические части, «приложений, вкладок, параметры, каналы, участники».|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательно)| Определяет видимость группы. Возможные значения: **частный**, **открытым**. Если видимости не указан, видимости копируются из исходной группы или группы. Если группа клонировании — это группа **educationClass** , параметр видимости игнорируется и видимости новой группы будут иметь значение HiddenMembership.|

## <a name="response"></a>Ответ

Если успешно завершена, этот метод возвращает `202 Accepted` код ответа с расположением: заголовок, с указанием ресурсов [операции](../resources/teamsasyncoperation.md) .
После завершения операции ресурсов операции сообщит вам, идентификатор созданного группы.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a>Ответ
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-clone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
