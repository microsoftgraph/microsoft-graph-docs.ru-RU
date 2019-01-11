---
title: assignLicense
description: Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака. К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя. Также можно включить и отключить определенные планы, связанных с подпиской. Для получения дополнительных сведений о подписках и лицензий, см в этой статье Technet.
localization_priority: Normal
ms.openlocfilehash: 71287b47a0a42ce4f89635fe6a1769c78874ae36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876204"
---
# <a name="assignlicense"></a>assignLicense

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Добавление или удаление лицензии пользователя для включения или отключения их использования Microsoft облака. К примеру организация может иметь подписки на Office 365 для предприятий E3 со 100 лицензий и этого запроса назначает один из этих лицензий для определенного пользователя. Также можно включить и отключить определенные планы, связанных с подпиской. Для получения дополнительных сведений о подписках и лицензий, см в этой [статье Technet](https://technet.microsoft.com/en-us/library/mt765146.aspx).

Чтобы получить подписок, доступных в каталоге, выполните [получить запрос subscribedSkus](subscribedsku-list.md). 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|addLicenses|Коллекция [assignedLicense](../resources/assignedlicense.md)|Коллекция объектов [assignedLicense](../resources/assignedlicense.md) , которые задают лицензий для добавления. Можно отключить servicePlans, связанный с лицензией путем установки свойства **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md) .|
|removeLicenses|Guid|Коллекция skuIds, определение лицензий для удаления.|

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и объект обновленный [пользователя](../resources/user.md) в теле ответа.

## <a name="example"></a>Пример
Добавьте лицензии для пользователя.
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a>Пример
Удалите лицензии у пользователя.

#####<a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a>Ответ
В обоих примерах ответа — это объект обновленный пользовательский. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
