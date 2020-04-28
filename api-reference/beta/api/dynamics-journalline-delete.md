---
title: Удаление Жаурналлинес
description: Удаляет строку журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 64de86b424bed9a1592ceb7ae5194c42d9233352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428931"
---
# <a name="delete-journallines"></a>Удаление Жаурналлинес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление объекта строки журнала из Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
```
DELETE /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок          |Значение                     |
|----------------|--------------------------|
|Авторизация   |Bearer {токен}. Обязательный. |
|If-Match        |Обязательный. Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **жаурналлинес**, **жаурналлинес** не будет обновлен. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
```

**Отклик** 

Ниже приведен пример отклика. 

```json
HTTP/1.1 204 No Content
```
