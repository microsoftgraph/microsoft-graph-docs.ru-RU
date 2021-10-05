---
title: Get deviceRegistrationPolicy
description: Ознакомьтесь с свойствами и отношениями объекта deviceRegistrationPolicy.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b02e1c9d6a0de046771e4a437cb1762eea73c6db
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127926"
---
# <a name="get-deviceregistrationpolicy"></a>Get deviceRegistrationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md) Представляет ограничения квоты deviceRegistrationPolicy, дополнительные политики проверки подлинности и авторизации для регистрации удостоверений устройств в организации.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)| Policy.ReadWrite.DeviceConfiguration|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

При вызове от имени пользователя пользователю необходимо принадлежать к следующим ролям [Azure AD:](/azure/active-directory/roles/permissions-reference)
+ Глобальный администратор
+ Администратор облачных устройств
+ Глобальный читатель

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_deviceregistrationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/policies/deviceRegistrationPolicy
```


### <a name="response"></a>Отклик

Ниже приводится пример ответа, который показывает параметры по умолчанию для политики регистрации устройств.

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
