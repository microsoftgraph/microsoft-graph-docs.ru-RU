---
title: Список политик, назначенных для приложения или участника службы
description: Получение объектов политики, назначенных приложению или участнику службы.
localization_priority: Normal
ms.openlocfilehash: 24833a42a8b3df2dfde6894cbcdae89a20c6e1cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332228"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a>Список политик, назначенных для приложения или участника службы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [политики](../resources/policy.md) , назначенных приложению или участнику службы.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объекты [политики](../resources/policy.md) в тексте отклика. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="example"></a>Пример
В следующем примере извлекаются политики, назначенные приложению.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
