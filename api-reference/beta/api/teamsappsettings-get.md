---
title: Получение teamsAppSettings
description: Чтение свойств и связей объекта teamsAppSettings.
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd04f3dcdb72775ec372763cb12e94ccbead9a0d
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645716"
---
# <a name="get-teamsappsettings"></a>Получение teamsAppSettings
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чтение свойств и связей объекта [teamsAppSettings](../resources/teamsappsettings.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamworkAppSettings.Read.All, TeamworkAppSettings.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

> [!NOTE]
> Разрешения TeamworkAppSettings.* могут не отображаться в портал Azure. Дополнительные сведения и способы их устранения см [. в статье об известных проблемах](/graph/known-issues#teamworkappsettings-permissions-are-not-visible-in-the-azure-portal).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamsAppSettings
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [teamsAppSettings](../resources/teamsappsettings.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-tenant-wide-settings-for-all-teams-apps-in-the-tenant"></a>Пример 1. Получение параметров на уровне клиента для всех приложений Teams в клиенте.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_teamsappsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/teamsAppSettings
```


#### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamsAppSettings",
    "id": "65bdf003-0c4c-4bca-b102-0821ab0d1364",
    "isChatResourceSpecificConsentEnabled": "true"
  }
}
```

## <a name="see-also"></a>См. также

- [Согласие для определенных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)