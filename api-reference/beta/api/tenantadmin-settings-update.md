---
title: Обновление параметров
description: Обновите один или несколько параметров уровня клиента для SharePoint и OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 07abcd226649c175fe6906a3b15e14971d8e9cf7
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653687"
---
# <a name="update-settings"></a>Обновление параметров
Пространство имен: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите один или несколько [параметров уровня клиента](../resources/tenantadmin-settings.md) для SharePoint и OneDrive.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SharePointTenantSettings.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|SharePointTenantSettings.ReadWrite.All|

При вызове от имени пользователя пользователь должен принадлежать к одной из следующих ролей администратора. Дополнительные сведения о ролях администраторов см. в статье о ролях администраторов [в Центр администрирования Microsoft 365](/microsoft-365/admin/add-users/about-admin-roles).
* Глобальный администратор
* Администратор SharePoint

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/sharepoint/settings
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]
В следующей таблице показаны свойства, которые можно изменить [для объекта параметров](../resources/tenantadmin-settings.md) .

|Свойство|Тип|Описание|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | Коллекция идентификаторов GUID              | Коллекция идентификаторов GUID доверенного домена для приложение синхронизации OneDrive приложения.                                                                                                                                                  |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | Количество дней для сохранения удаленного OneDrive.                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | Коллекция String            | Коллекция расширений файлов, не загруженных приложение синхронизации OneDrive приложения.                                                                                                                                           |
| imageTaggingOption                                 | imageTaggingChoice           | Указывает параметр маркировки изображений для клиента. Возможные значения: `disabled`, `basic`, `enhanced`.                                                                                                       |
| isCommentingOnSitePagesEnabled                     | Логический                      | Указывает, разрешены ли комментарии на современных страницах сайта в SharePoint.                                                                                                                                          |
| isFileActivityNotificationEnabled                  | Логический                      | Указывает, включены ли push-уведомления для OneDrive событий.                                                                                                                                               |
| isLoopEnabled                                      | Логический                      | Указывает, разрешено ли Fluid Framework на SharePoint сайтах.                                                                                                                                                   |
| isMacSyncAppEnabled                                | Логический                      | Указывает, можно ли синхронизировать файлы с помощью приложение синхронизации OneDrive для Mac.                                                                                                                                          |
| isResharingByExternalUsersEnabled                  | Логический                      | Указывает, разрешено ли гостям повторно использовать файлы, папки и сайты, которыми они не владеют.                                                                                                                           |
| isSharePointMobileNotificationEnabled              | Логический                      | Указывает, включены ли мобильные push-уведомления для SharePoint.                                                                                                                                             |
| isSharePointShafeedEnabled                        | Логический                      | Указывает, разрешен ли канал новостей на современных страницах сайта в SharePoint.                                                                                                                                   |
| isSiteCreationEnabled                              | Логический                      | Указывает, разрешено ли пользователям создавать сайты.                                                                                                                                                           |
| isSiteCreationUIEnabled                            | Логический                      | Указывает, отображаются ли команды пользовательского интерфейса для создания сайтов.                                                                                                                                                     |
| isSitePagesCreationEnabled                         | Логический                      | Указывает, разрешено ли создавать новые современные страницы на SharePoint сайтах.                                                                                                                                         |
| isSitesStorageLimitAutomatic                       | Логический                      | Указывает, выполняется ли автоматическое управление пространством хранилища сайта или задано ли для каждого сайта определенные ограничения хранилища.                                                                                                       |
| isSyncButtonHiddenOnPersonalSite                   | Логический                      | Указывает, скрыта ли кнопка синхронизации в OneDrive.                                                                                                                                                            |
| isUnmanagedSyncAppForTenantRestricted              | Логический                      | Указывает, разрешено ли пользователям синхронизировать файлы только на компьютерах, присоединенных к определенным доменам.                                                                                                                           |
| personalSiteDefaultStorageLimitInMB                | Int64                        | По умолчанию OneDrive для всех новых и существующих пользователей, которым назначена лицензия. Измеряется в мегабайтах (МБ).                                                                           |
| sharingAllowedDomainList                           | Коллекция строк            | Коллекция доменов электронной почты, которым разрешен общий доступ за пределами организации.                                                                                                                              |
| sharingBlockedDomainList                           | Коллекция строк            | Коллекция доменов электронной почты, которые заблокированы для общего доступа за пределами организации.                                                                                                                              |
| sharingCapability                                  | sharingCapabilities          | Возможность общего доступа для клиента. Возможные значения: `disabled`, `externalUserSharingOnly`, `externalUserAndGuestSharing`, `existingExternalUserSharingOnly`.                                                |
| sharingDomainRestrictionMode                       | sharingDomainRestrictionMode | Указывает режим внешнего совместного доступа для доменов. Возможные значения: `none`, `allowList`, `blockList`.                                                                                                        |
| siteCreationDefaultManagedPath                     | Строка                       | Значение управляемого пути сайта группы. Это путь, по которому будут создаваться новые сайты групп.                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | Квота хранилища по умолчанию для нового сайта после создания. Измеряется в мегабайтах (МБ).                                                                                                                            |
| tenantDefaultTimezone                              | Строка                       | Часовой пояс клиента по умолчанию для вновь созданных сайтов.                                                                                                                                                      |




## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный [](../resources/tenantadmin-settings.md) объект параметров в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_tenant_settings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/sharepoint/settings
Content-Type: application/json
Content-length: 1323

{
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [".mp3"],
    "imageTaggingOption": "enhanced",
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000
}
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
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [
        ".mp3"
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
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000,
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
```
