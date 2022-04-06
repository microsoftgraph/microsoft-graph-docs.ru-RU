---
title: Создание делегированияAdminRelationship
description: Создание нового объекта делегированияAdminRelationship.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 052790ed1b5356d86316364017dab395e2ecc661
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64590023"
---
# <a name="create-delegatedadminrelationship"></a>Создание делегированияAdminRelationship
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта делегированияAdminRelationship](../resources/delegatedadminrelationship.md) .

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
POST /tenantRelationships/delegatedAdminRelationships
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) .

При создании **делегированияAdminRelationship** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[microsoft.graph.delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Идентификаторы административных ролей, к которые партнер запрашивает или имеет доступ в клиенте-клиенте. Обязательный аргумент.|
|клиент|[microsoft.graph.delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|Имя отображения и уникальный идентификатор клиента отношения. Необязательное свойство.|
|displayName|String|Отображает имя отношения, используемого для простоты идентификации. Должна быть уникальной для *всех* делегированных отношений администратора партнера. Обязательный аргумент.|
|duration|Длительность|Продолжительность отношений в формате ISO 8601. Должно быть значением между инклюзивным `P1D` `P2Y` . Обязательный.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `201 Created` ответа и объект [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) в тексте ответа.

Ответ содержит **заглавную ссылку Location** , которая содержит URL-адрес созданного делегированного отношения администратора. **Каждый объект делегированияAdminRelationship** **содержит свойство @odata.etag** по RFC2616.
## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminrelationship_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships
Content-Type: application/json

{
  "displayName": "Contoso admin relationship",
  "duration": "P730D",
  "customer": {
    "tenantId": "4b827261-d21f-4aa9-b7db-7fa1f56fb163",
    "displayName": "Contoso subsidiary Inc"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationship"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
  "displayName": "Contoso admin relationship",
  "duration": "P730D",
  "customer": {
    "tenantId": "4b827261-d21f-4aa9-b7db-7fa1f56fb163",
    "displayName": "Contoso subsidiary Inc"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  },
  "status": "created",
  "createdDateTime": "2022-02-10T11:24:42.3148266Z",
  "lastModifiedDateTime": "2022-02-10T11:24:42.3148266Z",
  "activatedDateTime": "",
  "endDateTime": "2024-02-10T11:24:42.3148266Z"
}
```

