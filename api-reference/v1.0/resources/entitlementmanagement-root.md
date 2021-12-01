---
title: Работа с API управления правами Azure AD
description: Управление доступом к ресурсам, включая группы, приложения и сайты, с помощью управления правами Azure AD
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f296c4c29f150100b585e8c86651e42d841a8820
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242878"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления правами Azure AD

Пространство имен: microsoft.graph

Azure Active Directory управления правами Azure AD позволяет управлять доступом к группам, приложениям и веб-сайтам SharePoint для внутренних пользователей, а также пользователей за пределами организации.

Создав пакеты доступа с ролями, которые должны иметь пользователи в этих ресурсах, и определяя политики для того, кто может запрашивать пакет доступа и как долго у них может быть назначение пакета доступа, вы можете управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

Типы ресурсов управления правами включают:

- [accessPackage.](accesspackage.md)Определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам одним или более пользователями.
- accessPackageAssignmentPolicy: указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
- [accessPackageAssignmentRequest:](accesspackageassignmentrequest.md)создан пользователем, который хочет получить назначение пакета доступа.
- [accessPackageAssignment](accesspackageassignment.md): назначение пакета доступа определенному субъекту в течение определенного периода времени.
- [accessPackageCatalog:](accesspackagecatalog.md)контейнер для пакетов доступа.
- [connectedOrganization](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [entitlementManagementSettings:](entitlementmanagementsettings.md)параметры для управления правами Azure AD для всех клиентов.
- [утверждение:](approval.md)представляет решения, связанные с запросом пакета доступа.

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. Клиент, в котором используется управление правами, должен иметь допустимую Azure AD Premium P2 или подписку emS E5.

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

## <a name="methods"></a>Методы

| Метод   | Тип возвращаемых данных |Описание|
|:---------------|:--------|:----------|
| [получение](../api/entitlementmanagementsettings-get.md); | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ознакомьтесь с свойствами объекта **entitlementManagementSettings.** |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |
| [Пакеты доступа к спискам](../api/entitlementmanagement-list-accesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage.** |
| [Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Создайте новый **объект accessPackage.** |
| [Получить accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage,** фильтруемых на входе пользователя. |
| [Список accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md) | [accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md) | Извлечение списка **объектов accessPackageAssignmentRequest.** |
| [Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest.** |
| [Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Нет | Удаление **accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Извлечение списка **объектов accessPackageAssignmentRequest,** фильтруемых на входе пользователя.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest,** который находится в отменяемом состоянии: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .|
| [Списки accessPackageAssignments](../api/entitlementmanagement-list-assignments.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment.** |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.|
| [Список accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка **объектов accessPackageCatalogs.** |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый **объект accessPackageCatalog.** |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog.** |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog.** |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog**. |
| [Списки подключенныхОрганизацией](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) collection | Извлечение списка **объектов connectedOrganization.** |
| [Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Создание нового **объекта connectedOrganization.** |
| [ПодключениеОрганизация](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта **connectedOrganization.** |
| [Обновление connectedOrganization](../api/connectedorganization-update.md) |Нет | Обновление **подключеннойорганизации.** |
| [Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление **подключеннойорганизации.** |
|[Список internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внутренних спонсоров **connectedOrganization.** |
|[Список externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внешних спонсоров **connectedOrganization.** |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренние спонсоры **connectedOrganization.** |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу к внешним спонсорам **connectedOrganization.** |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удалите пользователя или группу из внутренних спонсоров **connectedOrganization.** |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удалите пользователя или группу из внешних спонсоров **connectedOrganization.** |

## <a name="see-also"></a>См. также

- [Что такое управление правами Azure AD?](/azure/active-directory/governance/entitlement-management-overview)
- [subjectSet](subjectset.md) подтипы [singleUser,](singleuser.md) [groupMembers,](groupmembers.md) [connectedOrganizationMembers,](connectedorganizationmembers.md) [requestorManager,](requestormanager.md) [internalSponsors](internalsponsors.md)и [externalSponsors](externalsponsors.md).
- [accessPackageSubject](accesspackagesubject.md) — используется в [accessPackageAssignment](accesspackageassignment.md) как пользователь субъекта, у которого есть назначение пакета доступа.
- [identitySource](identitysource.md) — используется в [connectedOrganization](connectedorganization.md), одном из [azureActiveDirectoryTenant,](azureactivedirectorytenant.md) [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation.](externaldomainfederation.md)


