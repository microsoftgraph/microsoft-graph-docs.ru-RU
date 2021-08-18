---
title: Список удаленных элементов, которые принадлежат пользователю
description: 'Извлекает список недавно удаленных элементов, которые принадлежат указанному пользователю.  '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0820b4187524f29b488852241944528712fc4f5e90a951605f75c51a520601f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165464"
---
# <a name="list-deleted-items-owned-by-a-user"></a>Список удаленных элементов, которые принадлежат пользователю

Пространство имен: microsoft.graph

Извлекает список недавно удаленных элементов, которые принадлежат указанному пользователю.  

В настоящее время функции удаленных элементов списка поддерживаются только для [приложений](../resources/application.md) и групповых ресурсов, которые принадлежат пользователю. [](../resources/group.md)

Это действие службы, которое означает, что оно не поддерживает pagination.  API возвращает до 1000 удаленных объектов, которые принадлежат пользователю, отсортировали по ID.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| --- | --- |
| Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) |  Не поддерживается. |
| Приложение | Group.Read.All, Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP-запрос

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| ------------- | ------------------------- |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Орган запроса требует следующих параметров:

| Параметр    | Тип |Описание|
|:---------------|:--------|:----------|
|userId|String|ID владельца.|
|type|Строка|Тип объектов, которые необходимо возвращать; `group` в настоящее время является единственным поддерживаемым значением.|


## <a name="response"></a>Отклик

Успешные запросы возвращают коды ответов; объект ответа включает свойства `200 OK` [каталога (удаленных](../resources/directory.md) элементов).

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Этот объект ответа может быть усечен для краткости. Все поддерживаемые свойства возвращаются из фактических вызовов.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```
