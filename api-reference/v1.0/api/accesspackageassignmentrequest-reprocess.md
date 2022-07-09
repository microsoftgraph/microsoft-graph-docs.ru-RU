---
title: 'accessPackageAssignmentRequest: повторная обработка'
description: Повторно обработает объекты accessPackageAssignmentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0ec27bd2dc451f95b3c001188924fa8c0077211b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698532"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest: повторная обработка

Пространство имен: microsoft.graph

В [Azure AD управления правами](../resources/entitlementmanagement-overview.md) вызывающие объекты могут автоматически повторить запрос пользователя на доступ к пакету доступа. Он выполняется для объекта [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) , **состояние requestState** которого находится в состоянии `DeliveryFailed` или состоянии `PartiallyDelivered` . 

Вы можете повторно обработать запрос только в течение 14 дней с даты завершения исходного запроса. Для запросов, выполненных более 14 дней, необходимо попросить пользователей отменить запросы и создать новый запрос на [портале MyAccess](https://myaccess.microsoft.com/) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/reprocess
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный элемент. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код  `202 Accepted` ответа и повторяет запрос. Если объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) не существует, `404 Not Found` этот метод вернет или, если идентификатор не является  допустимым, `400 Bad Request` этот метод возвращает код отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted  
```
