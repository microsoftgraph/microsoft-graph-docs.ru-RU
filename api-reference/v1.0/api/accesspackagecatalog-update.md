---
title: Обновление accessPackageCatalog
description: Обновление свойств объекта accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9e98ef1781168a502d5db95de9c87680fb5fc40d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242721"
---
# <a name="update-accesspackagecatalog"></a>Обновление accessPackageCatalog

Пространство имен: microsoft.graph


Обнови [существующий объект accessPackageCatalog,](../resources/accesspackagecatalog.md) чтобы изменить одно или несколько его свойств, например имя или описание отображения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя каталога пакетов доступа.|
|description|Строка|Описание каталога пакетов доступа.|
|catalogType|accessPackageCatalogType|Создается ли каталог пользователем или управлением правами. Допустимые значения: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|state|accessPackageCatalogState|Имеет `published` значение, если пакеты доступа доступны для управления. Допустимые значения: `unpublished`, `published`, `unknownFutureValue`.|
|isExternallyVisible|Boolean|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.



## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json

{
  "displayName":"Catalog One"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
}
-->
```http
HTTP/1.1 204 No Content
Content-Type: application/json

```

