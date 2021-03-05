---
title: Создание taxAreas
description: Создает объект налоговой области в Dynamics for Financials.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e30275efd4205b776593b5d515b2032654506a90
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473247"
---
# <a name="create-taxareas"></a>Создание taxAreas

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает объект области налогообложения в Центре бизнеса Dynamics 365.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

```http
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|------|-----|
|Авторизация  |Bearer {токен}. Обязательный.    |
|Content-Type  |application/json    |

## <a name="request-body"></a>Текст запроса
В теле запроса укажи представление JSON объекта **taxAreas.**

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` **taxAreas** в тексте ответа.

## <a name="example"></a>Пример

**Запрос**

Вот пример запроса.

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

{
  "code": "44442001T"
}
```

**Отклик**

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


