---
title: Обновление accessPackage
description: Обновление свойств объекта accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 84d393e276d5551e086e3419270df7cc5e4264dd
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242902"
---
# <a name="update-accesspackage"></a>Обновление accessPackage

Пространство имен: microsoft.graph


Обновим [существующий объект accessPackage,](../resources/accesspackage.md) чтобы изменить одно или несколько его свойств, например имя или описание отображения.

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
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
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
|displayName|Строка|Имя пакета доступа.|
|description|Строка|Описание пакета доступа.|
|isHidden|Логический|Скрыт ли пакет доступа от запросителя.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json

{
  "displayName":"Access Package New Name"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```


