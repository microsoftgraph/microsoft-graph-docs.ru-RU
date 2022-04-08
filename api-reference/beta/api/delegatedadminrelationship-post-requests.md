---
title: Создание запросов
description: Создайте новый объект delegatedAdminRelationshipRequest.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: df8e80f55e51c5b720e791243668fa468c1bcea6
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704401"
---
# <a name="create-requests"></a>Создание запросов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/requests
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) в формате JSON.

При создании **delegatedAdminRelationshipRequest** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|Действие, выполняемые с делегированным отношением администратора. Обязательный. Возможные значения: `lockForApproval`, `terminate`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) в тексте отклика. Ответ содержит заголовок **Location** , который содержит URL-адрес созданного запроса делегированных отношений администратора.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminrelationshiprequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests
Content-Type: application/json

{
  "action": "lockForApproval"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/c45e5ffb-3de2-4938-a214-b7eed802db66-4be56058-bb48-4a8e-8282-6cf0e98e6c9d/requests/5a6666c9-7282-0a41-67aa-25a5a3fbf339

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#requests",
  "id": "5a6666c9-7282-0a41-67aa-25a5a3fbf339",
  "action": "lockForApproval",
  "status": "created",
  "createdDateTime": "2022-02-10T10:55:47.1180588Z",
  "lastModifiedDateTime": "2022-02-10T10:55:47.1180588Z"
}
```

