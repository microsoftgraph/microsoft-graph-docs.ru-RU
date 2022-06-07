---
title: 'домен: повышение уровня'
description: Повышение уровня проверенного поддомена до корневого домена.
author: franqq
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c2dc412e4efd6ae2fc8466f134085f85bfd8e78a
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924196"
---
# <a name="domain-promote"></a>домен: повышение уровня

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Повышение уровня проверенного поддомена до корневого домена. Для проверенного домена **свойству isVerified** задано значение `true`.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения  |
|:--------------------|:-------------|
|Делегированное (рабочая или учебная учетная запись) | Domain.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
|Application | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/promote
```

> В качестве параметра {id} укажите домен, используя его полное доменное имя.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {token}. Обязательный.|
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик

В случае успешного выполнения этот вызов возвращает ответ `200 OK` и логическое значение, указывающее состояние публикации типа контента.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "domain_promote"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/promote
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.Boolean",
    "value": true
}
```
