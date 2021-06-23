---
title: Обновление командной работы
description: Обновление свойств объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: a17fcca078e66251a6532b2d3862352485f3cb2f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060713"
---
# <a name="update-teamworktag"></a>Обновление командной работы
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [teamworkTag.](../resources/teamworktag.md)

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
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [teamworkTag.](../resources/teamworktag.md)

В следующей таблице показаны свойства, необходимые при обновлении [teamworkTag.](../resources/teamworktag.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя тега. Значение не может быть более 40 символов.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_teamworktag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
Content-Type: application/json
Content-length: 185

{
  "displayName": "Finance"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Finance",
  "memberCount": 2,
  "tagType": "standard"
}
```
