---
title: 'educationSynchronizationProfile: uploadUrl'
description: Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для синхронизации профиля данных конкретного school в клиентов. Маркер SAS имеет допустимость часа.
ms.openlocfilehash: cf685b56718664ca68e0fde697872fe624c7e7b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080593"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>educationSynchronizationProfile: uploadUrl

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для конкретных школа данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов. Маркер SAS имеет допустимость часа.

Передача URL-адрес предоставляется только для [поставщика данных CSV](../resources/educationcsvdataprovider.md).

> **Примечание:** Для доступа к хранилища больших двоичных объектов с маркером SAS, с помощью [хранилища Azure SDK](https://github.com/search?q=org%3AAzure+azure-storage) или [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Permissions |
|:-----------|:----------|
| Делегированные (рабочая или учебная учетная запись) | EduAdministration.ReadWrite |
|Делегированные (личная учетная запись Майкрософт|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и URL-адрес SAS [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.

Если по-прежнему обрабатывается предыдущего запроса, этот метод возвращает `409 Conflict` , указывающее, что загрузка в настоящее время заблокирован по [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a>Ответ
Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
