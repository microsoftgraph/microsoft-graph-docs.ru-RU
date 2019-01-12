---
title: Permissions
description: 'Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.  '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f02d6dccd005696c130c6bb4a1f42c603943e5c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960569"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**Список удаленных элементов, принадлежащие пользователю**

Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.  

На данный момент удаленных элементов со списками поддерживается только для [группы](../resources/group.md) ресурсов владеет пользователь.

Это действие службы, которое означает, что он не поддерживает разбиение на страницы.  API возвращает до 1 000 удаленных объектов, принадлежащие пользователю, отсортированные по идентификатору.  1000 или больше удаленных владеет пользователь объектов API возвращает значение nothing.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| --- | --- |
| Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) |  Не поддерживается. |
| Для приложений | Group.Read.All, Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP-запрос

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>Заголовки запросов

| **Имя**      | **Описание**           |
| ------------- | ------------------------- |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

Текст запроса необходимо задать следующие параметры:

| Параметр    | Тип |Описание|
|:---------------|:--------|:----------|
|userId|String|Идентификатор владельца.|
|type|Строка|Тип собственные объекты для возвращения; `Group` в данный момент поддерживается только значение.|

## <a name="response"></a>Ответ

Успешные запросы `200 OK` коды ответа; объект ответа включает в себя свойств [каталога (удаленных элементов)](../resources/directory.md) .

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a>Ответ

Ниже приведен пример отклика. Примечание: Этот объект ответа может усекаться для краткости. Все поддерживаемые свойства возвращаются фактических вызовов.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
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


