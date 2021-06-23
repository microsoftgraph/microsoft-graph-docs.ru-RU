---
title: Создание командной работы
description: Создание нового объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b379037f01b5d28c867de0083ec6f7a581f0ea80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060716"
---
# <a name="create-teamworktag"></a>Создание командной работы
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте [стандартный тег](../resources/teamworktag.md) для участников группы. 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Не поддерживается.|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamworkTag.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [teamworkTag.](../resources/teamworktag.md)

В следующей таблице показаны свойства, необходимые при создании [teamworkTag.](../resources/teamworktag.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя тега. Значение не может быть больше 40 символов.|
|members| [коллекция teamworkTagMember](../resources/teamworktagmember.md) |Члены группы, добавленные в тег. Установите свойство идентификатора пользователя каждого участника. Количество участников не должно быть больше 25.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и объект `201 Created` [teamworkTag](../resources/teamworktag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_teamworktag_from"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
Content-Type: application/json

{
  "displayName": "Finance",
  "members":[
    {
        "userId":"92f6952f-61ca-4a94-8910-508a240bc167"
    },
    {
        "userId":"085d800c-b86b-4bfc-a857-9371ad1caf29"
    }
  ]
}
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Financee",
  "memberCount": 2,
  "tagType": "standard"
}
```

