---
title: Обновление Унитсофмеасуре
description: Обновляет объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 47ec43ae34a4841cbae04ef9c2fc3530becf96df
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791114"
---
# <a name="update-unitsofmeasure"></a>Обновление Унитсофмеасуре
Обновление свойств объекта Units of Measure для Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

```
PATCH /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|------|-----|
|Авторизация |Носителя. Обязательно.|
|Content-Type  |application/json|
|If-Match      |Обязательно. Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **унитсофмеасуре**, **унитсофмеасуре** не будет обновлен. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **унитсофмеасуре** в тексте отклика.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
Content-type: application/json

{
  "displayName": "One Piece"
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
  "code": "PCS",
  "displayName": "One Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```

