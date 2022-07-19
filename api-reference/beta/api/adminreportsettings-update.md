---
title: Обновление adminReportSettings
description: Обновление параметров уровня клиента для отчетов Microsoft 365.
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 0fb9ed8d8e80bf195e3d63f5139ca6498246fc48
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856818"
---
# <a name="update-adminreportsettings"></a>Обновление adminReportSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров уровня клиента для отчетов Microsoft 365.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|----------------------------------------|---------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | ReportSettings.ReadWrite.All                |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | ReportSettings.ReadWrite.All                |

> **Примечание:** Для делегированных разрешений, позволяющих приложениям обновлять параметры отчета от имени пользователя, администратор клиента должен назначить пользователю соответствующую ограниченную роль администратора Azure Active Directory. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } --> 
```http
PATCH /admin/reportSettings
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                |
| :------------ | :--------------------------|
| Авторизация | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство       | Тип           | Описание                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Логический | Если задано значение , `true`все отчеты будут скрывать сведения о пользователе, такие как имена пользователей, группы и сайты. Если `false`это так, все отчеты будут отображать идентифицируемые сведения. Это свойство представляет параметр в Центр администрирования Microsoft 365. Обязательный. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

Ниже приведен пример запроса, который обновляет параметр на уровне клиента для отчетов Microsoft 365.

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_adminreportsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/reportSettings
Content-Type: application/json
Content-length: 37

{
  "displayConcealedNames": true
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
