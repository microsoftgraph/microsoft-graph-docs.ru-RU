---
title: Создание customerPaymentJournals
description: Создает объект журнала платежей клиентов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8041463e58ff9d81d04f771d21bea313f6829620
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473338"
---
# <a name="create-customerpaymentjournals"></a>Создание customerPaymentJournals

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает объект журнала платежей клиентов в Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

```http
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
В теле запроса поставляем представление JSON объекта **customerPaymentJournals.**

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и объект ```201 Created``` **customerPaymentJournals** в тексте ответа.

## <a name="example"></a>Пример

**Запрос**

Вот пример запроса.

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals
Content-type: application/json

{
  "code": "DEFAULT"
}
```

**Отклик**

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```




