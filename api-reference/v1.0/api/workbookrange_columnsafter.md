# <a name="workbookrange-columnsafter"></a>workbookRange: columnsAfter

Возвращает определенное количество столбцов справа от заданного диапазона.

### <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются такие **области**: _Files.Read, Files.ReadWrite_.
### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
### <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {code}|
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

### <a name="parameters"></a>Параметры

| Параметр       | Тип    |Описание|
|:---------------|:--------|:----------|
|count|Int32|Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.|


### <a name="request-body"></a>Тело запроса

### <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200, OK` и объект [workbookRange](../resources/range.md) в теле отклика.

### <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
