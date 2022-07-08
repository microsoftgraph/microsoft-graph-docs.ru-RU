---
title: Обновление deviceRegistrationPolicy
description: Обновление свойств объекта deviceRegistrationPolicy.
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: df37115ff775d204a68c2d95f59d644de5d62d6a
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690002"
---
# <a name="update-deviceregistrationpolicy"></a>Обновление deviceRegistrationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) . Представляет ограничения квоты deviceRegistrationPolicy, дополнительную проверку подлинности и политики авторизации для регистрации удостоверений устройств в организации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.DeviceConfiguration|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Не поддерживается|

При вызове от имени пользователя пользователь должен принадлежать к следующим Azure AD [ролей](/azure/active-directory/roles/permissions-reference):
+ Глобальный администратор
+ Администратор облачных устройств

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить.


|Свойство|Тип|Описание|
|:---|:---|:---|
|userDeviceQuota|Int32|Указывает максимальное количество устройств, которые пользователь может иметь в вашей организации перед блокировкой регистрации новых устройств. |
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Указывает политику проверки подлинности для пользователя, чтобы завершить регистрацию с помощью Azure AD присоединения или Azure AD зарегистрированных в организации. Возможные значения: `notRequired` или `required`. |
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Задает политику авторизации для управления регистрацией новых устройств с Azure AD регистрации в организации. Обязательный элемент. Дополнительные сведения см. [в разделе "Что такое удостоверение устройства?"](/azure/active-directory/devices/overview). Если Intune включено, это свойство нельзя изменить.|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Задает политику авторизации для управления регистрацией новых устройств с помощью Azure AD присоединения в организации. Обязательный элемент. Дополнительные сведения см. [в разделе "Что такое удостоверение устройства?"](/azure/active-directory/devices/overview).|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deviceregistrationpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/deviceRegistrationPolicy
Content-Type: application/json

{
    "id": "deviceRegistrationPolicy",
    "displayName": "Device Registration Policy",
    "description": "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    "userDeviceQuota": 50,
    "multiFactorAuthConfiguration": "0",
    "azureADRegistration": {
        "appliesTo": "1",
        "isAdminConfigurable": false,
        "allowedUsers": [],
        "allowedGroups": []
    },
    "azureADJoin": {
        "appliesTo": "1",
        "isAdminConfigurable": true,
        "allowedUsers": [],
        "allowedGroups": []
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deviceregistrationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deviceregistrationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deviceregistrationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-deviceregistrationpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#deviceRegistrationPolicy",
    "id": "deviceRegistrationPolicy",
    "displayName": "Device Registration Policy",
    "description": "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    "userDeviceQuota": 50,
    "multiFactorAuthConfiguration": "0",
    "azureADRegistration": {
        "appliesTo": "1",
        "isAdminConfigurable": false,
        "allowedUsers": [],
        "allowedGroups": []
    },
    "azureADJoin": {
        "appliesTo": "1",
        "isAdminConfigurable": true,
        "allowedUsers": [],
        "allowedGroups": []
    }
}
```
