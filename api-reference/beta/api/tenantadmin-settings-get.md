---
title: Получение параметров
description: Получение параметров уровня клиента для SharePoint и OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 2111ff6b45149a133de0022d50dd92042c0c3d60
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653651"
---
# <a name="get-settings"></a>Получение параметров
Пространство имен: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите параметры уровня [клиента для](../resources/tenantadmin-settings.md) SharePoint и OneDrive.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SharePointTenantSettings.Read.All, SharePointTenantSettings.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|SharePointTenantSettings.Read.All, SharePointTenantSettings.ReadWrite.All|

При вызове от имени пользователя пользователь должен принадлежать к одной из следующих ролей администратора. Дополнительные сведения о ролях администраторов см. в статье о ролях администраторов [в Центр администрирования Microsoft 365](/microsoft-365/admin/add-users/about-admin-roles).
* Глобальный администратор
* Глобальный читатель
* Администратор SharePoint

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/sharepoint/settings
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика [и объект](../resources/tenantadmin-settings.md) параметров в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/sharepoint/settings
```


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tenantAdmin.settings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": {
        "@odata.type": "#microsoft.graph.tenantAdmin.settings",
        "id": "e79403fa-abdf-af49-56c5-f7119d8b1948",
        "allowedDomainGuidsForSyncApp": [
            "bdd1ab9b-3fd0-4def-a761-ec8d7471732c", 
            "ad31vb6b-5zd0-7tyg-m231-kj8d6578432c"
        ],
        "availableManagedPathsForSiteCreation": [
            "/sites/",
            "/teams/"
        ],
        "deletedUserPersonalSiteRetentionPeriodInDays": 344,
        "excludedFileExtensionsForSyncApp": [
            ".md", 
            ".git"
        ],
        "imageTaggingOption": "basic",
        "isCommentingOnSitePagesEnabled": true,
        "isFileActivityNotificationEnabled": true,
        "isLoopEnabled": true,
        "isMacSyncAppEnabled": false,
        "isResharingByExternalUsersEnabled": true,
        "isSharePointMobileNotificationEnabled": true,
        "isSharePointNewsfeedEnabled": true,
        "isSiteCreationEnabled": true,
        "isSiteCreationUIEnabled": true,
        "isSitePagesCreationEnabled": true,
        "isSitesStorageLimitAutomatic": true,
        "isSyncButtonHiddenOnPersonalSite": true,
        "isUnmanagedSyncAppForTenantRestricted": true,
        "personalSiteDefaultStorageLimitInMB": 113664,
        "sharingAllowedDomainList" : [
            "contoso.com",
            "fabrikam.com"
        ],
        "sharingBlockedDomainList" : [
            "contoso.com",
            "fabrikam.com"
        ],
        "sharingCapability": "externalUserAndGuestSharing",
        "sharingDomainRestrictionMode": "allowList",
        "siteCreationDefaultManagedPath": "/sites/",
        "siteCreationDefaultStorageLimitInMB": 808034,
        "tenantDefaultTimezone": "(UTC-05:00) Eastern Time (US and Canada)"
    }
}
```

