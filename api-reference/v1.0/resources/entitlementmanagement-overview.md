---
title: Работа с API управления правами Azure AD
description: Управление доступом к ресурсам, включая группы, приложения и сайты, с помощью управления правами Azure AD
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 2b46abf3c7c7b8b74fcccc3647a4e33cae2efbc4
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607283"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления правами Azure AD

Пространство имен: microsoft.graph

Azure Active Directory управления правами Azure AD может помочь управлять доступом к группам, приложениям и веб-сайтам SharePoint для внутренних пользователей, а также пользователей за пределами организации.

Создав пакеты доступа с ролями, которые должны иметь пользователи в этих ресурсах, и определяя политики для того, кто может запрашивать пакет доступа и как долго у них может быть назначение пакета доступа, вы можете управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

Типы ресурсов управления правами включают:

- [accessPackage](accesspackage.md). Определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам одним или более пользователями.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): создан пользователем, который хочет получить назначение пакета доступа.
- [accessPackageAssignment](accesspackageassignment.md): назначение пакета доступа определенному субъекту в течение определенного периода времени.
- [accessPackageCatalog](accesspackagecatalog.md): контейнер для пакетов доступа.
- [connectedOrganization](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [entitlementManagementSettings](entitlementmanagementsettings.md): параметры для управления правами Azure AD для всех клиентов.
- [утверждение](approval.md): представляет решения, связанные с запросом пакета доступа.

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. Клиент, в котором используется управление правами, должен иметь допустимую Azure AD Premium P2 или подписку emS E5. Дополнительные сведения о требованиях к лицензиям для функции управления правами см. в дополнительных сведениях о требованиях к лицензиям на [управление правами](/azure/active-directory/governance/entitlement-management-overview#license-requirements).

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

| Метод   | Тип возвращаемых данных |Описание|
|:---------------|:--------|:----------|
| [Получение](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ознакомьтесь с свойствами объекта **entitlementManagementSettings** . |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings** . |
| [Пакеты доступа к спискам](../api/entitlementmanagement-list-accesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage** . |
| [Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Создайте новый **объект accessPackage** . |
| [Получить accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage** . |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage** . |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage** , фильтруемых на входе пользователя. |
| [Список accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md) | [accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md) | Извлечение списка **объектов accessPackageAssignmentRequest** . |
| [Создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создает новый **объект accessPackageAssignmentRequest** . |
| [Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest** . |
| [Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Нет | Удаление **accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Извлечение списка **объектов accessPackageAssignmentRequest** , фильтруемых на входе пользователя.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest**, который находится в отменяемом состоянии: `accepted`, `pendingApproval`, , `pendingNotBefore``pendingApprovalEscalated`.|
| [Списки accessPackageAssignments](../api/entitlementmanagement-list-assignments.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment** . |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment** , фильтруемых на входе пользователя.|
| [Список accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка **объектов accessPackageCatalogs** . |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый **объект accessPackageCatalog** . |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog** . |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog** . |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog**. |
|[Список accessPackageAssignmentPolicies](../api/entitlementmanagement-list-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Получите список объектов [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) и их свойств.|
|[Создание accessPackageAssignmentPolicy](../api/entitlementmanagement-post-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Создание нового [объекта accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Получить accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Обновление свойств объекта [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md)|Нет|Удаляет объект [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
| [Списки подключенныхОрганизацией](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) collection | Извлечение списка **объектов connectedOrganization** . |
| [Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Создание нового **объекта connectedOrganization** . |
| [ПодключениеОрганизация](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта **connectedOrganization** . |
| [Обновление connectedOrganization](../api/connectedorganization-update.md) |Нет | Обновление **подключеннойорганизации**. |
| [Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление **подключеннойорганизации**. |
|[Список internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внутренних спонсоров **connectedOrganization** . |
|[Список externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Извлечение списка внешних спонсоров **connectedOrganization** . |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренние спонсоры **connectedOrganization** . |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу к внешним спонсорам **connectedOrganization** . |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удалите пользователя или группу из внутренних спонсоров **connectedOrganization** . |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удалите пользователя или группу из внешних спонсоров **connectedOrganization** . |
|[Получить утверждение](../api/approval-get.md) | [утверждение](approval.md) | Извлечение свойств объекта **утверждения** . |
|[filterByCurrentUser](../api/approval-filterbycurrentuser.md)| [коллекция утверждений](approval.md)| **Извлечение объектов** утверждения для утверждения.|
|[Список утвержденийStages](../api/approval-list-stages.md) | [коллекция approvalStage](approvalstage.md) | Список объектов **approvalStage** , связанных с объектом **утверждения** . |
|[Получить утверждениеStage](../api/approvalstage-get.md) | [approvalStage](approvalstage.md) | Извлечение свойств объекта **approvalStage** . |
|[Обновление approvalStage](../api/approvalstage-update.md) | Нет | Применить утверждение или отказ в принятии решения по **объекту approvalStage** . |

## <a name="see-also"></a>См. также

- [Что такое управление правами Azure AD?](/azure/active-directory/governance/entitlement-management-overview)
- [subjectSet](subjectset.md) подтипы [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) и [externalSponsors](externalsponsors.md).
- [accessPackageSubject](accesspackagesubject.md) — используется в [accessPackageAssignment](accesspackageassignment.md) как пользователь субъекта, у которого есть назначение пакета доступа.
- [identitySource](identitysource.md) — используется в [connectedOrganization](connectedorganization.md), одном из [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md).


