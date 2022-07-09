---
title: 'accessPackageAssignment: повторная обработка'
description: Повторно обработает объекты accesspackageassignment.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 75d221efa4c740eadb132ef429ac5d193512f3c6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698538"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment: повторная обработка

Пространство имен: microsoft.graph

В [Azure AD](../resources/entitlementmanagement-overview.md) управления правами вызывающие объекты могут автоматически переоценить и принудительно применить объект [accessPackageAssignment](../resources/accesspackageassignment.md) назначений пользователя для определенного пакета доступа. Значение **assignmentState** пакета `Delivered` доступа должно быть для повторной обработки назначения пользователя администратором. Это действие могут выполнять только администраторы с ролью диспетчера назначения пакетов доступа или более поздней Azure AD управления правами.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{id}/reprocess 
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный элемент. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

`202 Accepted` В случае успешного выполнения этот метод возвращает код отклика, повторно оценивает и применяет назначения пользователя объекта [accessPackageAssignment](../resources/accesspackageassignment.md), то есть состояние пакета доступа будет изменено на "Доставлено". Если назначение не существует, `404 Not Found` этот метод вернет или, если идентификатор не является  допустимым, этот метод возвращает код `400 Bad Request` отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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