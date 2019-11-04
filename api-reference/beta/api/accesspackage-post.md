---
title: Создание Акцесспаккаже
description: Создание нового Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06d6c92ed227b03d1adf069e1fc8dd76e9658622
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936071"
---
# <a name="create-accesspackage"></a>Создание Акцесспаккаже

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [акцесспаккаже](../resources/accesspackage.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Ентитлементманажемент. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Authorization | Носитель \{токен\}. Обязательный элемент. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [акцесспаккаже](../resources/accesspackage.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика 201, созданный в теле отклика, и новый объект [акцесспаккаже](../resources/accesspackage.md) .

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
