---
title: Запуск синхронизации после загрузки файлов educationSynchronizationProfile
description: Проверьте файлы, отправленные в конкретных школа профиль синхронизации данных клиента. Если проверка выполнена успешно, в профиле будет запустить синхронизацию. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, не запустится синхронизации. Если ответ содержит только предупреждения, будет запущен процесс синхронизации.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1447178e80d30058b415345aea83dce4390e6bcf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512355"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a>Запуск синхронизации после загрузки файлов educationSynchronizationProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Проверьте файлы, загруженные в конкретных школа данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов. Если проверка выполнена успешно, в профиле будет запустить синхронизацию. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, не запустится синхронизации. Если ответ содержит только предупреждения, будет запущен процесс синхронизации.

> **Примечание:** Этот метод используется только в том случае, если поставщик данных имеет тип [educationcsvdataprovider](../resources/educationcsvdataprovider.md). Кроме того свойство профиля в состоянии необходимо подготовить к работе с прежде чем можно будет начать. Опрос объект профиля, чтобы проверить значение свойства состояний.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения |
|:-----------|:----------|
| Делегированные (рабочая или учебная учетная запись) | EduAdministration.ReadWrite |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика `200 OK`. Если неудачно, возвращается `400 Bad Request`. Ответ содержит коллекцию объектов [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) как часть тела ответа, если найдены ошибки и предупреждения.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a>Ответ
Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
