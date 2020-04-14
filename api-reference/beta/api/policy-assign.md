---
title: Назначение политики
description: Назначает политику для приложения или участника службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 694b070b0186e8e76a0bb7180e538c0ac42188d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450895"
---
# <a name="assign-policy"></a>Назначение политики

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Назначает [политику](../resources/policy.md) для приложения или участника службы.

>Примечание. в настоящее время назначение политики применяется только к политике времени жизни маркеров. Этот тип политики описан в разделе [Политика](../resources/policy.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> Note: "ID" в запросе — это свойство "ID" приложения или субъекта-службы, а не свойство AppID.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | application/json  | Характер данных в теле объекта. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте представление объекта политики, который необходимо добавить, в формате JSON.

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="example"></a>Пример
В следующем примере для приложения назначается политика.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 204 No Content
```
