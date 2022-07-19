---
title: Получение adminReportSettings
description: Получение параметров уровня клиента для отчетов Microsoft 365.
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b9edf2396cd3409e794386f08eb4a124ce65d892
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856819"
---
# <a name="get-adminreportsettings"></a>Получение adminReportSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение параметров уровня клиента для отчетов Microsoft 365.

> **Примечание:** Дополнительные сведения о различных представлениях и именах отчетов см. в разделе "[Отчеты Microsoft 365](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)" в Центре администрирования Приложения Microsoft 365 использования.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)           |
|:---------------------------------------|:------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | ReportSettings.Read.All, ReportSettings.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                        |
| Приложение                            | ReportSettings.Read.All, ReportSettings.ReadWrite.All |

> **Примечание:** Чтобы делегированные разрешения разрешать приложениям получать параметры отчета от имени пользователя, администратор клиента должен назначить пользователю соответствующую ограниченную роль администратора Azure Active Directory. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /admin/reportSettings
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [adminReportSettings](../resources/adminreportsettings.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_adminreportsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/reportSettings
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminReportSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.adminReportSettings",
    "displayConcealedNames": true
  }
}
```
