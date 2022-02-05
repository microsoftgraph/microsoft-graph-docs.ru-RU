---
title: Обновление accessPackageCatalog
description: Обновление свойств объекта accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
---
# <a name="update-accesspackagecatalog"></a>Обновление accessPackageCatalog

Пространство имен: microsoft.graph


Обнови [существующий объект accessPackageCatalog](../resources/accesspackagecatalog.md) , чтобы изменить одно или несколько его свойств, например имя или описание отображения.

## <a name="permissions"></a>Разрешения:
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
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя каталога пакетов доступа.|
|description|String|Описание каталога пакетов доступа.|
|catalogType|accessPackageCatalogType|Создается ли каталог пользователем или управлением правами. Допустимые значения: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|state|accessPackageCatalogState|Имеет значение, `published` если пакеты доступа доступны для управления. Допустимые значения: `unpublished`, `published`, `unknownFutureValue`.|
|isExternallyVisible|Логический|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|



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
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
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

