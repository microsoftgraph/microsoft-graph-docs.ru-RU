---
title: Работа с API управления правами Azure AD
description: Управление доступом к ресурсам, включая группы, приложения и сайты, с помощью управления правами Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 7dc9ec20ef316cd0c6e5e305d780099f61901e6f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761327"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления правами Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление правами Azure Active Directory (Azure AD) позволяет управлять доступом к группам, приложениям и сайтам SharePoint Online для внутренних пользователей, а также пользователей за пределами организации.

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

Учебник, в который показано, как использовать управление правами для создания пакета ресурсов, которые внутренние пользователи могут запрашивать для самообслуживки, см. в статью Создание пакета доступа с помощью [API Microsoft Graph.](/graph/tutorial-access-package-api)

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. Клиент, в котором используется управление правами, должен иметь допустимую приобретенную или пробную подписку Azure AD Premium P2 или EMS E5.

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [получение](../api/entitlementmanagementsettings-get.md); | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ознакомьтесь с свойствами объекта **entitlementManagementSettings.** |
| [Update](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |
| [Пакеты доступа к спискам](../api/accesspackage-list.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accessPackage.** |
| [Создание accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Создайте новый **объект accessPackage.** |
| [Получить accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Извлечение списка **объектов accessPackageResourceRoleScope** для пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа. |
| [Список accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection | Извлечение списка **объектов accessPackageAssignmentPolicy.** |
| [Создание accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Создание нового **объекта accessPackageAssignmentPolicy.** |
| [Получить accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **accessPackageAssignmentPolicy.** |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта **accessPackageAssignmentPolicy.** |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление **accessPackageAssignmentPolicy**. |
| [Список accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md) | Извлечение списка **объектов accessPackageAssignmentRequest.** |
| [Создание accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создание нового **accessPackageAssignmentRequest**. |
| [Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest.** |
| [Списки accessPackageAssignments](../api/accesspackageassignment-list.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment.** |
| [Список accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Извлечение списка **объектов accessPackageAssignmentResourceRole.** |
| [Получите accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | **Извлечение объекта accessPackageAssignmentResourceRole.** |
| [Список accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка **объектов accessPackageCatalogs.** |
| [Создание accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый **объект accessPackageCatalog.** |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog.** |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog.** |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog**. |
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка **объектов accessPackageResource.** |
| [Роли ресурсов accessPackageCatalog в списке](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Извлечение списка **объектов accessPackageResourceRole.** |
| [Список accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Чтение свойств и связей **объектов accessPackageResourceRequest.** |
| [Создание accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создание нового **объекта accessPackageResourceRequest.** |
|[Список accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection|Извлечение списка [объектов accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Получите accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
| [Списки подключенныхОрганизацией](../api/connectedorganization-list.md) | [connectedOrganization](connectedorganization.md) collection | Извлечение списка **объектов connectedOrganization.** |
| [Создание connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Создание нового **объекта connectedOrganization.** |
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
