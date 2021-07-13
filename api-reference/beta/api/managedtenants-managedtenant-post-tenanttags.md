---
title: Создание tenantTag
description: Создание нового объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9de058914e2262debcbe87d449b5ffc7fc15db7b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403056"
---
# <a name="create-tenanttag"></a>Создание tenantTag
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта tenantTag.](../resources/managedtenants-tenanttag.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.WriteRead.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [tenantTag.](../resources/managedtenants-tenanttag.md)

В следующей таблице показаны свойства, необходимые при создании [tenantTag.](../resources/managedtenants-tenanttag.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения тега клиента.|
|description|String|Описание тега клиента.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_tenanttag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
Content-Type: application/json
Content-length: 382

{
  "displayName": "Support",
  "description": "Tenants that have purchased extended support"
}
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "11103b2b-0e28-456b-901d-45f98890ab1d",
  "displayName": "Support",
  "description": "Tenants that have purchased extended support",
  "tenantIds": [],
  "isDeleted": null,
  "createdDateTime": "2021-07-11T19:31:49.807267Z",
  "createdByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0",
  "lastActionDateTime": "2021-07-11T19:31:49.8072716Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
