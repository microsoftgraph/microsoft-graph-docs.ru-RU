---
title: Создание запросов
description: Создание нового объекта делегированияAdminRelationshipRequest.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 96760913dc8dc5e4745cd1231f1b69a18a313b6f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589886"
---
# <a name="create-requests"></a>Создание запросов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта делегированияAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

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
В теле запроса поставляем представление JSON объекта [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

При создании **делегированияAdminRelationshipRequest** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|Действие, выполняемые в делегированной связи администратора. Обязательный аргумент. Возможные значения: `lockForApproval`, `terminate`.|

## <a name="response"></a>Отклик

В случае успеха этот метод `201 Created` возвращает код ответа и объект [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) в тексте ответа. Ответ содержит **заглавную ссылку Location** , которая содержит URL-адрес созданного делегированного запроса на отношения администратора.

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

