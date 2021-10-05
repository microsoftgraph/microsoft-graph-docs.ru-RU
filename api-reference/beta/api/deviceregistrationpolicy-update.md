---
title: Обновление deviceRegistrationPolicy
description: Обновление свойств объекта deviceRegistrationPolicy.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e55beac9f1ada8a3a6d2fe9d2ae8a81eff6e3085
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127929"
---
# <a name="update-deviceregistrationpolicy"></a>Обновление deviceRegistrationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md) Представляет ограничения квоты deviceRegistrationPolicy, дополнительные политики проверки подлинности и авторизации для регистрации удостоверений устройств в организации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Policy.ReadWrite.DeviceConfiguration|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

При вызове от имени пользователя пользователю необходимо принадлежать к следующим ролям [Azure AD:](/azure/active-directory/roles/permissions-reference)
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
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить.


|Свойство|Тип|Описание|
|:---|:---|:---|
|userDeviceQuota|Int32|Указывает максимальное количество устройств, которые пользователь может иметь в организации, перед блокировкой регистрации новых устройств. |
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Указывает политику проверки подлинности, чтобы пользователь завершил регистрацию с помощью Azure AD Join или Azure AD, зарегистрированных в организации. Возможные значения: `notRequired` или `required`. |
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Указывает политику авторизации для контроля регистрации новых устройств с помощью регистрации Azure AD в организации. Обязательно. Дополнительные сведения см. [в том, что такое удостоверение устройства?](/azure/active-directory/devices/overview). Если включен Intune, это свойство не может быть изменено.|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Указывает политику авторизации для контроля регистрации новых устройств с помощью Azure AD Join в организации. Обязательно. Дополнительные сведения см. [в том, что такое удостоверение устройства?](/azure/active-directory/devices/overview).|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

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
