---
title: Удаление Каунтринамедлокатион
description: Удаление объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f56ed6245102cfe01744f22ca0a36fa22d5c4df
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653701"
---
# <a name="delete-countrynamedlocation"></a>Удаление Каунтринамедлокатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

>[!NOTE]
>Этот API требует нескольких разрешений. Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
