---
title: Создание журналов
description: Создает объект журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3c90808de4f07e45ded7c215577fff6916a59978
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431433"
---
# <a name="create-journals"></a>Создание журналов

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает журнал в Dynamics 365 Business Central. 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

```
POST /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок        |Значение                     |
|--------------|--------------------------|
|Авторизация |Bearer {токен}. Обязательный. |
|Content-Type  |application/json          |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта **журналов** в формате JSON.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **журналов** в тексте отклика.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals
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

