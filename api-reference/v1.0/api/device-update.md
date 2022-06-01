---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 183155c31a69c0f669d4bafcaa19cb0a6fa78ee4
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821136"
---
# <a name="update-device"></a>Обновление устройства

Пространство имен: microsoft.graph

Обновление свойств зарегистрированного устройства.

Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).

> [!IMPORTANT]
> У этого API есть [известная проблема](/graph/known-issues#linux-based-devices-cant-be-updated-by-an-app-with-application-permissions). Приложение с разрешениями приложения может обновлять свойство **extensionAttributes** только для устройств под управлением Linux, то есть там, где находится **свойство** `linux`operationSystem.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Device.ReadWrite.All, Directory.ReadWrite.All |

Вызывающему пользователю также должна быть одна из следующих [ролей](/azure/active-directory/roles/permissions-reference) *Azure AD:* глобальный администратор, *Intune администратор.* Вызывающий пользователь с ролью администратора облачных устройств может только включить или отключить устройства с помощью этого API, а пользователь  с ролью администратора Windows 365 может обновлять только основные свойства устройства.

## <a name="http-request"></a>HTTP-запрос

В `{id}` запросе содержится значение свойства **идентификатора** устройства, а не **свойства deviceId** .
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md). Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический| Если учетная запись обеспечена — `true`, в противном случае — `false`. Обновить это *свойство могут только* вызывающие *объекты* с ролями глобального администратора и администратора облачных устройств.|
|operatingSystem|String|Тип операционной системы на устройстве.|
|operatingSystemVersion|String|Версия операционной системы на устройстве.|
|displayName|Строка|Отображаемое имя устройства.|
|isCompliant|Boolean|`true` if the device complies with Mobile Device Management (MDM) policies; otherwise, `false`. Его можно обновить только Intune для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows ОС. |
|isManaged|Boolean|`true`Значение , если устройство управляется мобильным приложением Управление устройствами (MDM); в противном случае — значение `false`. Его можно обновить только Intune для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows ОС. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-the-accountenabled-property-of-a-device"></a>Пример 1. Обновление свойства accountEnabled устройства

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
Content-type: application/json

{
  "accountEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-device-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-device-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2--write-extensionattributes-on-a-device"></a>Пример 2. Запись extensionAttributes на устройстве

#### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device_extensionAttributes"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
Content-type: application/json

{
    "extensionAttributes": {
        "extensionAttribute1": "BYOD-Device"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-extensionattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-extensionattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-device-extensionattributes-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-device-extensionattributes-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
