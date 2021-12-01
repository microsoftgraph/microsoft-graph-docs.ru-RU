---
title: Создание accessPackage
description: Создание нового accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9c62d3444f65f0d17dadc26070ffe8afe18eb7d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242673"
---
# <a name="create-accesspackage"></a>Создание accessPackage

Пространство имен: microsoft.graph

Создайте новый [объект accessPackage.](../resources/accesspackage.md)

Пакет доступа будет добавлен в существующий [accessPackageCatalog.](../resources/accesspackagecatalog.md)

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
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем JSON-представление [объекта accessPackage.](../resources/accesspackage.md)

При создании **accessPackage** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени пакета доступа.|
|description|Строка|Описание пакета доступа.|
|isHidden|Логический|Скрыт ли пакет доступа от запросителя.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект accessPackage](../resources/accesspackage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_accesspackage"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages
Content-Type: application/json

{
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "catalog": {
    "id": "66584aae-98bb-48cc-9458-7bee5d2a6577"
  }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "642181f0-bc17-4fc6-9ebb-ff53dbf18c2f",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "createdDateTime": "2021-11-10T01:10:09.5220119Z",
  "modifiedDateTime": "2021-11-10T01:10:09.5220119Z"
}
```

