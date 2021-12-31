---
title: Работа с API управления правами Azure AD
description: Управление доступом к ресурсам, включая группы, приложения и сайты, с помощью управления правами Azure AD
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f99496d7288531ee932a4022c67af2c3458e2d93
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651055"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления правами Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory управления правами Azure AD позволяет управлять доступом к группам, приложениям и веб-сайтам SharePoint для внутренних пользователей, а также пользователей за пределами организации.

Создав пакеты доступа с ролями, которые должны иметь пользователи в этих ресурсах, и определяя политики для того, кто может запрашивать пакет доступа и как долго у них может быть назначение пакета доступа, вы можете управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

Типы ресурсов управления правами включают:

- [accessPackage.](accesspackage.md)Определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам одним или более пользователями.
- [accessPackageAssignmentPolicy:](accesspackageassignmentpolicy.md)указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
- [accessPackageAssignmentRequest:](accesspackageassignmentrequest.md)создан пользователем, который хочет получить назначение пакета доступа.
- [accessPackageAssignment](accesspackageassignment.md): назначение пакета доступа определенному субъекту в течение определенного периода времени.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): указывает роль, определенную для ресурса, которую субъекту было назначено с помощью назначения пакета доступа.
- [accessPackageCatalog:](accesspackagecatalog.md)контейнер для пакетов доступа.
- [accessPackageResourceRequest:](accesspackageresourcerequest.md)запрос на добавление ресурса в каталог пакетов доступа.
- [accessPackageResourceEnvironment:](accesspackageresourceenvironment.md)ссылка на геолокацию ресурса. Применимо к сайтам Multi-Geo SharePoint Online.
- [connectedOrganization](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [entitlementManagementSettings:](entitlementmanagementsettings.md)параметры для управления правами Azure AD для всех клиентов.
- [утверждение:](approval.md)представляет решения, связанные с запросом пакета доступа.

Кроме того, назначения ролей для определенных ролей для управления правами можно управлять с помощью определений ролей управления [правами.](unifiedroledefinition.md)

Учебник, в который показано, как использовать управление правами для создания пакета ресурсов, которые внутренние пользователи могут запрашивать самостоятельно, см. в инструкции [Create an access package using Microsoft Graph API.](/graph/tutorial-access-package-api)

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. Клиент, в котором используется управление правами, должен иметь допустимую Azure AD Premium P2 или подписку emS E5.

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [получение](../api/entitlementmanagementsettings-get.md); | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ознакомьтесь с свойствами объекта **entitlementManagementSettings.** |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |
| [Пакеты доступа к спискам](../api/entitlementmanagement-list-accesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage.** |
| [Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Создайте новый **объект accessPackage.** |
| [Получить accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage,** фильтруемых на входе пользователя. |
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Извлечение списка **объектов accessPackageResourceRoleScope** для пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа. |
| [Список несовместимыхAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка несовместимых объектов **accesspackage** для этого пакета доступа. |
| [Добавление accessPackage в несовместимыеAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Нет | Добавьте ссылку, чтобы указать другой **пакет доступа** несовместим с указанным пакетом доступа. |
| [Удаление accessPackage из несовместимыхAccessPackages](../api/accesspackage-delete-incompatibleaccesspackage.md) | Нет | Удалить ссылку, которая указывала на **несовместимость accesspackage.** |
| [Несовместимые группы списка](../api/accesspackage-list-incompatiblegroups.md) | Коллекция [group](group.md) | Извлечение списка несовместимых **групповых** объектов для этого пакета доступа. |
| [Добавление группы в несовместимые Группы](../api/accesspackage-post-incompatiblegroup.md) | Нет | Добавьте ссылку, чтобы указать, что членство **в группе** несовместимо с указанным пакетом доступа. |
| [Удаление группы из несовместимых групп](../api/accesspackage-delete-incompatiblegroup.md) | Нет | Удалите ссылку, которая указывала, что членство **в** группе несовместимо.|
| [Список accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка объектов  **accesspackage,** которые перечисляют этот пакет доступа как несовместимые. |
| [Список accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection | Извлечение списка **объектов accessPackageAssignmentPolicy.** |
| [Создание accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Создание нового **объекта accessPackageAssignmentPolicy.** |
| [Получить accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **accessPackageAssignmentPolicy.** |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта **accessPackageAssignmentPolicy.** |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление **accessPackageAssignmentPolicy**. |
| [Список accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md) | Извлечение списка **объектов accessPackageAssignmentRequest.** |
| [Создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создание нового **accessPackageAssignmentRequest**. |
| [Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest.** |
| [Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Нет | Удаление **accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Извлечение списка **объектов accessPackageAssignmentRequest,** фильтруемых на входе пользователя.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest,** который находится в отменяемом состоянии: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .|
| [Списки accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment.** |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.|
| [Список accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md) | [коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Извлечение списка **объектов accessPackageAssignmentResourceRole.** |
| [Получите accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | **Извлечение объекта accessPackageAssignmentResourceRole.** |
| [Список accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка **объектов accessPackageCatalogs.** |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый **объект accessPackageCatalog.** |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog.** |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog.** |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog**. |
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка **объектов accessPackageResource.** |
| [Роли ресурсов accessPackageCatalog в списке](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Извлечение списка **объектов accessPackageResourceRole.** |
| [Список accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Чтение свойств и связей **объектов accessPackageResourceRequest.** |
| [Создание accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создание нового **объекта accessPackageResourceRequest.** |
|[Список accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection|Извлечение списка [объектов accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Получите accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
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
|[Получить утверждение](../api/approval-get.md) | [утверждение](approval.md) | Извлечение свойств объекта **утверждения.** |
|[Утверждение спискаSteps](../api/approval-list-steps.md) | [коллекция approvalStep](approvalstep.md) | Список объектов **approvalStep,** связанных с объектом **утверждения.** |
|[Получить утверждениеStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Извлечение свойств объекта **approvalStep.** |
|[Обновление approvalStep](../api/approvalstep-update.md) | Нет | Применить утверждение или отказ в принятии решения по **объекту approvalStep.** |


## <a name="types"></a>Типы

- [requestorSettings,](requestorsettings.md) [approvalSettings,](approvalsettings.md) [questions](accesspackagequestion.md) and [assignmentReviewSettings](assignmentreviewsettings.md) - Используется в [accessPackageAssignmentPolicy,](accesspackageassignmentpolicy.md) чтобы указать, кто может запрашивать, кто утверждает и кто проверяет запросы на назначение пакета доступа по этой политике.
- [approvalStage](approvalstage.md) — используется в [approvSettings](approvalsettings.md) для указания основных, резервных копий и утверждений эскалации.
- [approvalStep](approvalstep.md) — используется в [утверждении для](approval.md) разграничить различные этапы утверждения.
- [userSet](userset.md) подтипы [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md)и [externalSponsors](externalsponsors.md) - Используется в [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md), [approvalStep](approvalstep.md) и [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) — используется в [accessPackageAssignment](accesspackageassignment.md) как пользователь субъекта, у которого есть назначение пакета доступа.
- [identitySource](identitysource.md) — используется в [connectedOrganization](connectedorganization.md), одном из [azureActiveDirectoryTenant,](azureactivedirectorytenant.md) [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation.](externaldomainfederation.md)

## <a name="see-also"></a>См. также

 - [Что такое управление правами Azure AD?](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
