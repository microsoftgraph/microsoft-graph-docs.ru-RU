---
title: Получить сведения о состоянии educationSynchronizationProfile
description: Получите сведения о состоянии определенного школа данных синхронизации профиля в клиентов. Ответ будет указывают состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 394bb03760e33b4581f5d29e90a4c8fd875c26d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418136"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a>Получить сведения о состоянии educationSynchronizationProfile

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получите сведения о состоянии данных конкретного школа [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов. Ответ будет указывают состояние синхронизации.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:-----------|:----------|
| Делегированные (рабочая или учебная учетная запись) | EduAdministration.Read EduAdministration.ReadWrite |
|Делегированные (личная учетная запись Майкрософт|Не поддерживается.|
|Для приложений| EduAdministration.Read.All EduAdministration.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
