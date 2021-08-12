---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 65ccc4dcc323914301fb5429a6cb3d0c3e29584fe3773417cfe4ec66bcb7ae65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200189"
---
# <a name="chart-image"></a>Chart: Image

Пространство имен: microsoft.graph

Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "samples" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.|

## <a name="path-parameters"></a>Параметры пути
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|height|Int32|Нужная высота создаваемого изображения. Необязательно.|
|width|Int32|Нужная ширина создаваемого изображения. Необязательно.|
|fittingMode|string|Метод, используемый для масштабирования диаграммы до указанных размеров (если заданы как высота, так и ширина)."  Допустимые значения: `Fit`, `FitAndCenter`, `Fill`.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a>Отклик
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a>Применение

Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`. Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки. А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

