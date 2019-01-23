---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7279b8da1ffe159dba56f4a5a10345243703da1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393748"
---
# <a name="update-iosvppebook"></a>Обновление объекта iosVppEBook

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|displayName|String|Имя электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|description|String|Описание. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|publisher|String|Издатель. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Обложка книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги. Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|vppTokenId|Guid|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с токеном VPP.|
|vppOrganizationName|String|Название организации для токена VPP.|
|genres|Коллекция String|Жанры.|
|language|String|Язык.|
|seller|String|Продавец.|
|totalLicenseCount|Int32|Общее число лицензий.|
|usedLicenseCount|Int32|Число используемых лицензий.|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 854

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




