---
title: Удаление paymentMethods
description: Удаляет объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f02b2c82386180609afbf13beeb25b35c6a30467
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474330"
---
# <a name="delete-paymentmethods"></a>Удаление paymentMethods

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление объекта метода оплаты из Центра бизнеса Dynamics 365.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
```
DELETE /financials/companies/{id}/paymentMethods/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

|Заголовок         |Значение                     |
|---------------|--------------------------|
|Авторизация  |Bearer {токен}. Обязательный. |
|If-Match       |Обязательно. Если этот загон запроса включен и предоставленный eTag не соответствует текущему тегу на **paymentMethods,** **платежMethods** не обновляется. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods/{id}
```

**Отклик** 

Ниже приведен пример отклика. 

```http
HTTP/1.1 204 No Content
```



