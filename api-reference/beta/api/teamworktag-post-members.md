---
title: Создание командной работыTagMember
description: Создайте новый объект teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28ae8ae4749e1ecca4f5e370858e88de45d2faf4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060719"
---
# <a name="create-teamworktagmember"></a>Создание командной работыTagMember
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект teamworkTagMember](../resources/teamworktagmember.md) в команде.

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
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [teamworkTagMember.](../resources/teamworktagmember.md)

В следующей таблице показаны свойства, необходимые при создании [командной работыTagMember.](../resources/teamworktagmember.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя члена группы.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект teamworkTagMember](../resources/teamworktagmember.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_teamworktagmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
Content-Type: application/json
Content-length: 144

{
    "userId":"97f62344-57dc-409c-88ad-c4af14158ff5"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Megan Bowen",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
}
```

