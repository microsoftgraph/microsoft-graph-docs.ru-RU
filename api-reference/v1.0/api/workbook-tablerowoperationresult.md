---
title: 'книга: tableRowOperationResult'
description: Часть асинхронного запроса на создание tableRow.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6f71b07dafba46cf99ee89c19e445dd315aa92f9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860924"
---
# <a name="workbook-tablerowoperationresult"></a>книга: tableRowOperationResult
Пространство имен: microsoft.graph

Эта функция является последней из серии действий по асинхронному созданию ресурса [workbookTableRow.](../resources/workbooktablerow.md)

Лучше всего создать несколько строк таблицы, чтобы пакетизировать их в одну операцию [tableRow](./table-post-rows.md) и выполнять операцию асинхронно.

Асинхронный запрос на создание строк таблиц включает в себя следующие действия:
1. Выдайте запрос async [Create tableRow](./table-post-rows.md) и получите URL-адрес запроса, возвращенный в `Location` заглавной таблице ответа.
2. Используйте URL-адрес запроса, возвращенный на шаге 1, чтобы выступить с запросом [Get workbookOperation](./workbookoperation-get.md) и получить ID операции для шага 3. 
    Кроме того, для удобства после получения результата operationStatus можно получить URL-адрес запроса из свойства resourceLocation возвращаемой в ответе `succeeded`  [книгиOperation](../resources/workbookoperation.md) и применить URL-адрес запроса к шагу  3. 
3. Используйте URL-адрес запроса, возвращенный из шага 2 в качестве URL-адреса запроса GET для этой таблицы **ФункцииRowOperationResult.** Успешный вызов функции возвращает новые строки таблицы в [ресурсе workbookTableRow.](../resources/workbooktablerow.md)

Эта функция не делает ничего, если называется независимо.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Files.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/drive/items/{id}/workbook/tableRowOperationResult(key={operation-id})
GET /me/drive/root:/{item-path}:/workbook/tableRowOperationResult(key={operation-id})
```

## <a name="function-parameters"></a>Параметры функции
URL-адрес запроса требует следующего параметра запроса. 

|Параметр|Тип|Описание|
|:---|:---|:---|
|key|String|**OperationId,** представленная в **ответе workbookOperation,** возвращаемом в предыдущем запросе [Get workbookOperation.](./workbookoperation-get.md)|


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
| Workbook-Session-Id  | ID сеанса книги, определяя, сохраняются ли изменения. Необязательный параметр.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и объект `200 OK` [workbookTableRow](../resources/workbooktablerow.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже показан пример запроса.
<!-- {
  "blockType": "request",
  "sampleKeys": ["0195cfac-bd22-4f91-b276-dece0aa2378b"],
  "name": "workbook_tablerowoperationresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tableRowOperationResult(key='0195cfac-bd22-4f91-b276-dece0aa2378b')
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```
