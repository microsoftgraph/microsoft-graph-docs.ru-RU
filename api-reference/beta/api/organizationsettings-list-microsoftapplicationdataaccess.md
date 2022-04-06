---
title: Список microsoftApplicationDataAccessSettings
description: Получите параметры объекта MicrosoftApplicationDataAccessSettings, которые указывают доступ из приложений Майкрософт к Microsoft 365 пользовательских данных в организации.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 01b0f53b99eaff9abf62b36c8247be44cf5c94e7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589788"
---
# <a name="list-microsoftapplicationdataaccesssettings"></a>Список microsoftApplicationDataAccessSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите _параметры_ объекта [MicrosoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md), которые указывают доступ из приложений Майкрософт к Microsoft 365 пользовательских данных в организации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Organization.Read.All, Organization.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/settings/microsoftApplicationDataAccess
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного `200 OK` решения этот метод возвращает код ответа и коллекцию объектов [MicrosoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_microsoftapplicationdataaccesssettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/microsoftApplicationDataAccess
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "name": "list_microsoftapplicationdataaccesssettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```

## <a name="see-also"></a>См. также

[Настройка конфиденциальности элементов](/graph/insights-customize-item-insights-privacy) для организации.
