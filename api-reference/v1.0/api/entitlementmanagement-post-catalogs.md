---
title: Создание accessPackageCatalog
description: Создание нового accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 043df8315a4f91953555fb36fbd2458ec363af82
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242770"
---
# <a name="create-accesspackagecatalog"></a>Создание accessPackageCatalog

Пространство имен: microsoft.graph


Создайте новый [объект accessPackageCatalog.](../resources/accesspackagecatalog.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/catalogs
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessPackageCatalog.](../resources/accesspackagecatalog.md)

При создании **accessPackageCatalog** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени каталога пакетов доступа.|
|description|Строка|Описание каталога пакетов доступа.|
|state|accessPackageCatalogState|Имеет `published` значение, если пакеты доступа доступны для управления. Возможные значения: `unpublished` и `published` .|
|isExternallyVisible|Boolean|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект accessPackageCatalog](../resources/accesspackagecatalog.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs
Content-Type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "state": "published",
  "isExternallyVisible": true
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{

  "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "userManaged",
  "state": "published",
  "isExternallyVisible": true,
  "createdDateTime": "2021-11-10T01:08:30.9134953Z",
  "modifiedDateTime": "2021-11-10T01:08:30.9134953Z"
}
```

