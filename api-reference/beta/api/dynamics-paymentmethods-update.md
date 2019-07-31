---
title: Обновление Пайментмесодс
description: Обновляет объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 95e9fc2e0de68f737bc68c51e16d55caaa573208
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956081"
---
# <a name="update-paymentmethods"></a>Обновление Пайментмесодс
Обновление свойств объекта метода оплаты для Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
```
PATCH /financials/companies('{id}')/paymentMethods('{id}')
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок        |Значение                     |
|--------------|--------------------------|
|Авторизация |Bearer {токен}. Обязательный. |
|Content-Type  |application/json          |
|If-Match      |Обязательно. Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **пайментмесодс**, **пайментмесодс** не будет обновлен. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **пайментмесодс** в тексте отклика.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods('{id}')
Content-type: application/json

{
  "displayName": "Personal Check Payment",
}
```

**Отклик**

Ниже приведен пример отклика. 

> **Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "CHECK",
  "displayName": "Personal Check Payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}
```


