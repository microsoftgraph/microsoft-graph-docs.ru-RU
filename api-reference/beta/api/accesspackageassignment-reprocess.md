---
title: 'accessPackageAssignment: reprocess'
description: Повторное выполнение объектов accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4ba699950b7c4ab54eca1a75a1a85f1e63c9c774
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257362"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment: reprocess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](../resources/entitlementmanagement-root.md)звонители могут автоматически переоформить и принудить объект [accessPackageAssignment](../resources/accesspackageassignment.md) к назначениям пользователя для определенного пакета доступа. **НазначениеУправление** пакета доступа должно быть для администратора для повторной работы с `Delivered` назначением пользователя. Выполнить это действие могут только администраторы с ролью диспетчера назначения пакетов доступа или более высокой в управлении правами Azure AD.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{id}/reprocess 
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика, а также возвращает и применяет назначения пользователя объекта `202 Accepted` [accessPackageAssignment,](../resources/accesspackageassignment.md) что означает, что состояние пакета доступа будет изменено на Delivered. Если назначения не существует, этот метод возвращается или если код не действителен, этот метод возвращает `404 Not Found` код  `400 Bad Request` ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted 
```
