---
title: Permissions
description: 'Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.  '
ms.openlocfilehash: affdd67d48056c4459e651fd5c64168d8356abe8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024966"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**Список удаленных элементов, принадлежащие пользователю**

Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.  

На данный момент удаленных элементов со списками поддерживается только для [группы](../resources/group.md) ресурсов владеет пользователь.

Это действие службы, которое означает, что он не поддерживает разбиение на страницы.  API возвращает до 1 000 удаленных объектов, принадлежащие пользователю, отсортированные по идентификатору.

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

| Имя          | Описание               |
| ------------- | ------------------------- |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

Текст запроса необходимо задать следующие параметры:

| Параметр    | Тип |Description|
|:---------------|:--------|:----------|
|userId|String|Идентификатор владельца.|
|type|String|Тип собственные объекты для возвращения; `Group` в данный момент поддерживается только значение.|


## <a name="response"></a>Ответ

Успешные запросы `200 OK` коды ответа; объект ответа включает в себя свойств [каталога (удаленных элементов)](../resources/directory.md) .

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
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
              "deletedDateTime": 2018-04-01T12:39:16Z,
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


