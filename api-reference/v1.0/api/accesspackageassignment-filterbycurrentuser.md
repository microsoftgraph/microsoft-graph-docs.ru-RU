---
title: 'accessPackageAssignment: filterByCurrentUser'
description: Извлечение списка объектов accesspackageassignment, фильтруемых на входе пользователя.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9ed084f91e84d288ad8ea3d7d07ebaa4b32ffa9e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242697"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a>accessPackageAssignment: filterByCurrentUser
Пространство имен: microsoft.graph


В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)вы можете получить список объектов [accessPackageAssignment,](../resources/accesspackageassignment.md) фильтруемых для пользователя, входив в него.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Параметры функции
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Параметр|Тип|Описание|
|:---|:---|:---|
|on|accessPackageAssignmentFilterByCurrentUserOptions|Список пользовательских параметров, которые можно использовать для фильтрации в списке назначений пакета доступа.|

- `target` используется для получения объектов, в которых целевым объектом является пользователь, заявив `accessPackageAssignment` о подписании. В итоговом списке содержатся все назначения, текущие и просроченные, для вызываемого во всех каталогах и пакетах доступа.

- `createdBy` используется для получения `accessPackageAssignment` объектов, созданных подписанным пользователем. В итоговом списке содержатся все назначения, созданные вызываемой для себя или от имени других лиц, например в случае прямого назначения администратора, во всех каталогах и пакетах доступа.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [коллекцию accessPackageAssignment](../resources/accesspackageassignment.md) в тексте ответа.

Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством в ответе, содержам URL-адрес на `@odata.nextLink` следующую страницу результатов. Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом в каждом ответе, пока не будут возвращены `@odata.nextLink` все результаты. Дополнительные сведения см. [в Graph microsoft Graph в приложении.](/graph/paging)

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='target')
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "null",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```

