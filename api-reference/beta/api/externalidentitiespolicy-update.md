---
title: Обновление externalIdentitiesPolicy
description: Обновите параметры объекта externalIdentitiesPolicy на уровне клиента, который определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания.
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 918bc089306c51d28a4afb61fc4a4038bb8eb049
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768380"
---
# <a name="update-externalidentitiespolicy"></a>Обновление externalIdentitiesPolicy
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите параметры объекта [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) на уровне клиента, который определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.ExternalIdentities|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Policy.ReadWrite.ExternalIdentities|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/externalIdentitiesPolicy
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowDeletedIdentitiesDataRemoval|Логический|Уведомляет Azure AD о том, следует ли удалять сведения о внешнем удостоверении из гостевого клиента при удалении пользователя в домашнем клиенте. Обязательный.|
|allowExternalIdentitiesToLeave|Логическое|Уведомляет Azure AD о том, следует ли удалять сведения о внешнем удостоверении из гостевого клиента при удалении пользователя в домашнем клиенте. Обязательный.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_externalidentitiespolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/externalIdentitiesPolicy

{
  "allowExternalIdentitiesToLeave":false
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

