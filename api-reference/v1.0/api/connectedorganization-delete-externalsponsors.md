---
title: Удаление externalSponsors
description: Удалите пользователя или группу из внешних спонсоров подключенной организации.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 946aa0807eec75a6301477f35e2fa5aeab701da4
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242967"
---
# <a name="remove-externalsponsors"></a>Удаление externalSponsors

Пространство имен: microsoft.graph

Удалите пользователя или группу из внешних спонсоров подключенной организации. Внешние [спонсоры](../resources/externalsponsors.md) — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой связанной организации.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.


## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

