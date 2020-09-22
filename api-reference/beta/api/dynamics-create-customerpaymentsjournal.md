---
title: Создание Кустомерпайментжаурналс
description: Создает объект журнала платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a95e0db2d53e3d6e3d172e875cac23119c4592f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008346"
---
# <a name="create-customerpaymentjournals"></a>Создание Кустомерпайментжаурналс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает объект журнала клиентских платежей в Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

```
POST /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок        |Значение                    |
|--------------|-------------------------|
|Авторизация |Bearer {токен}. Обязательный.|
|Content-Type  |application/json         |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта **кустомерпайментжаурналс** в формате JSON.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает ```201 Created``` код отклика и объект **кустомерпайментжаурналс** в тексте отклика.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

**Отклик**

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```




