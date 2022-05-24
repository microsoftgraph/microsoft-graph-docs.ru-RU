---
title: Тип ресурса settings
description: Представляет параметры уровня клиента для SharePoint и OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: acc37088c339abeaf0e6405e00ef45a344803e9c
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653684"
---
# <a name="settings-resource-type"></a>Тип ресурса settings
Пространство имен: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры уровня клиента для SharePoint и OneDrive.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание
|:---|:---|:---
|[Получение параметров](../api/tenantadmin-settings-get.md)|[microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | Получение параметров уровня клиента для SharePoint и OneDrive.|
|[Обновление параметров](../api/tenantadmin-settings-update.md) | [microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | Обновите один или несколько параметров уровня клиента для SharePoint и OneDrive.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | Коллекция идентификаторов GUID              | Коллекция идентификаторов GUID доверенного домена для приложение синхронизации OneDrive приложения.                                                                                                                                                  |
| availableManagedPathsForSiteCreation               | Коллекция String            | Коллекция управляемых путей, доступных для создания сайта. Только для чтения.                                                                                                                                            |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | Количество дней для сохранения удаленного OneDrive.                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | Коллекция String            | Коллекция расширений файлов, не загруженных приложение синхронизации OneDrive приложения.                                                                                                                                           |
| imageTaggingOption                                 | [tenantAdmin.imageTaggingChoice](../resources/tenantadmin-settings.md#imagetaggingchoice-values)           | Указывает параметр маркировки изображений для клиента. Возможные значения: `disabled`, `basic`, `enhanced`.                                                                                                       |
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
| sharingAllowedDomainList                           | Коллекция String            | Коллекция доменов электронной почты, которым разрешен общий доступ за пределами организации.                                                                                                                              |
| sharingBlockedDomainList                           | Коллекция String            | Коллекция доменов электронной почты, которые заблокированы для общего доступа за пределами организации.                                                                                                                              |
| sharingCapability                                  | [tenantAdmin.sharingCapabilities](#sharingcapabilities-values)          | Возможность общего доступа для клиента. Возможные значения: `disabled`, `externalUserSharingOnly`, `externalUserAndGuestSharing`, `existingExternalUserSharingOnly`.                                                |
| sharingDomainRestrictionMode                       | [tenantAdmin.sharingDomainRestrictionMode](#sharingdomainrestrictionmode-values) | Указывает режим внешнего совместного доступа для доменов. Возможные значения: `none`, `allowList`, `blockList`.                                                                                                        |
| siteCreationDefaultManagedPath                     | Строка                       | Значение управляемого пути сайта группы. Это путь, по которому будут создаваться новые сайты групп.                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | Квота хранилища по умолчанию для нового сайта после создания. Измеряется в мегабайтах (МБ).                                                                                                                            |
| tenantDefaultTimezone                              | Строка                       | Часовой пояс клиента по умолчанию для вновь созданных сайтов.                                                                                                                                                      |

### <a name="imagetaggingchoice-values"></a>Значения imageTaggingChoice
| Member                          | Описание                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| отключено                        | Параметр маркировки изображений для клиента отключен.                                                                  |
| Основные                           | Позволяет пользователям в клиенте добавлять базовые теги к изображениям, чтобы сделать их доступными через поиск.                    |
| Расширенные                        | Позволяет пользователям помечать изображения пользовательскими тегами и расширенными функциями.                                                    |
| unknownFutureValue              | Значение sentinel для развиваемого перечисления. Не следует использовать.                                                                     |

### <a name="sharingcapabilities-values"></a>Значения sharingCapabilities
| Member                          | Описание                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| отключено                        | Пользователи могут предоставлять общий доступ только пользователям в организации. Внешний общий доступ не разрешен.                                 |
| externalUserSharingOnly         | Пользователи могут предоставлять общий доступ новым и существующим гостям. Гости должны войти в систему или предоставить код проверки.                     |
| externalUserAndGuestSharing     | Пользователи могут предоставлять общий доступ любому пользователю по ссылкам, которые не требуют входа.                                                |
| existingExternalUserSharingOnly | Пользователи могут делиться с существующими гостями (которые уже есть в каталоге организации).                            |
| unknownFutureValue              | Значение sentinel для развиваемого перечисления. Не следует использовать.                                                                     |

### <a name="sharingdomainrestrictionmode-values"></a>Значения sharingDomainRestrictionMode
| Member                          | Описание                                                                                                           |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| Нет                            | Ограничения не применяются.                                                                                                |
| allowList                       | Пользователи смогут предоставлять доступ внешним участникам совместной работы только из списка разрешенных доменов электронной почты.           |
| blockList                       | Пользователи смогут делиться со всеми внешними участниками совместной работы, кроме тех, которые есть в списке заблокированных доменов электронной почты. |
| unknownFutureValue              | Значение sentinel для развиваемого перечисления. Не следует использовать.                                                                     |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tenantAdmin.settings",
  "openType": "false"
}
-->
``` json
{
    "allowedDomainGuidsForSyncApp": ["string (identifier)"],
    "availableManagedPathsForSiteCreation": ["string"],
    "deletedUserPersonalSiteRetentionPeriodInDays": "Int32",
    "excludedFileExtensionsForSyncApp": ["string"],
    "id": "string (identifier)",
    "imageTaggingOption": "string",
    "isCommentingOnSitePagesEnabled": "boolean",
    "isFileActivityNotificationEnabled": "boolean",
    "isLoopEnabled": "boolean",
    "isMacSyncAppEnabled": "boolean",
    "isResharingByExternalUsersEnabled": "boolean",
    "isSharePointMobileNotificationEnabled": "boolean",
    "isSharePointNewsfeedEnabled": "boolean",
    "isSiteCreationEnabled": "boolean",
    "isSiteCreationUIEnabled": "boolean",
    "isSitePagesCreationEnabled": "boolean",
    "isSitesStorageLimitAutomatic": "boolean",
    "isSyncButtonHiddenOnPersonalSite": "boolean",
    "isUnmanagedSyncAppForTenantRestricted": "boolean",
    "personalSiteDefaultStorageLimitInMB": "Int64",
    "sharingAllowedDomainList" : ["string"],
    "sharingBlockedDomainList" : ["string"],
    "sharingCapability": "string",
    "sharingDomainRestrictionMode": "string",
    "siteCreationDefaultManagedPath": "string",
    "siteCreationDefaultStorageLimitInMB": "Int32",
    "tenantDefaultTimezone": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "namespace": "microsoft.graph.tenantAdmin"
}
-->
