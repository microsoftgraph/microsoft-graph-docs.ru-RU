---
title: Обновление entitlementManagementSettings
description: Обновление объекта entitlementManagementSettings, чтобы изменить одно или несколько его свойств.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 90542c2ee86fb0680feec65b92f0996a7852c364
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242764"
---
# <a name="update-entitlementmanagementsettings"></a>Обновление entitlementManagementSettings

Пространство имен: microsoft.graph


Обновим [существующий объект entitlementManagementSettings,](../resources/entitlementmanagementsettings.md) чтобы изменить одно или несколько его свойств.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/settings
```

## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON параметров объекта [entitlementManagementSettings.](../resources/entitlementmanagementsettings.md)

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

