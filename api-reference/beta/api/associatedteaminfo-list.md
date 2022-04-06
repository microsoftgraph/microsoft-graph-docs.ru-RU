---
title: Перечисление associatedTeamInfo
description: Получение списка команд в Microsoft Teams, с чем связан пользователь.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16842866ca4c2b03268e80eb838bbf953844c605
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685266"
---
# <a name="list-associatedteaminfo"></a>Перечисление associatedTeamInfo
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка команд [в Microsoft Teams](../resources/associatedteaminfo.md), с помощью [которых связан](../resources/user.md) пользователь.
В настоящее [время пользователь](../resources/user.md) может быть связан с [командой двумя](../resources/team.md) разными способами:
* Пользователь [может](../resources/user.md) быть непосредственным участником [команды](../resources/team.md).
* Пользователь [может](../resources/user.md) быть членом общего [канала,](../resources/channel.md) размещенного в [команде](../resources/team.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All|

> **Примечание.** В настоящее время при использовании делегированных пользователем разрешений эта операция поддерживается только для пользователя `me`. При использовании разрешений для приложений она поддерживается для всех пользователей путем указания определенного идентификатора пользователя (псевдоним `me` не поддерживается при использовании разрешений для приложений).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{user-id}/teamwork/associatedTeams
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию связанных [объектовTeamInfo](../resources/associatedteaminfo.md) в теле отклика.

> **Примечание**. Этот API также возвращает группу узлов общего канала, непосредственным участником которого является пользователь.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_associatedteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/teamwork/associatedTeams
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-c5a5-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-e65d-7hd4-9a49-91d9f2e8493a",
      "displayName": "Contoso Team"
    },
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-8934-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-8961-7hd4-9a49-91d9f2e8493a",
      "displayName": "Fabrikam Team"
    }
  ]
}
```


## <a name="see-also"></a>См. также

- [Перечисление объектов joinedTeams](../api/user-list-joinedteams.md)
- [Перечисление всех команд в организации](../api/teams-list.md)
- [Получение команды](../api/team-get.md)

