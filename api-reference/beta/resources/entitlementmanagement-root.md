---
title: Работа с API управления правами Azure AD
description: Управление доступом к ресурсам, включая группы, приложения и сайты, с помощью управления правами Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: d2363e60a0eb99388d3da36264802f87bc12ee93
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131539"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления правами Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление правами Azure Active Directory (Azure AD) позволяет управлять доступом к группам, приложениям и сайтам SharePoint Online для внутренних пользователей, а также пользователей за пределами организации.

Создав пакеты доступа с ролями, которые должны быть доступны пользователям в этих ресурсах, и определив политики для пользователей, которые могут запрашивать пакет доступа и как долго у них может быть назначение пакета доступа, можно управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

К типам ресурсов управления правами относятся:

- [accessPackage](accesspackage.md): определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): указывает политику, с помощью которой субъекты могут запрашивать или получать пакет доступа через назначение пакета доступа.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): создается пользователем, который хочет получить назначение пакета доступа.
- [accessPackageAssignment](accesspackageassignment.md): назначение пакета доступа определенной теме на определенный период времени.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): указывает определенную роль ресурса, которой была назначена тема посредством назначения пакета доступа.
- [accessPackageCatalog](accesspackagecatalog.md): контейнер для пакетов доступа.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): запрос на добавление ресурса в каталог пакетов доступа.
- [accessPackageResourceEnvironment](accesspackageresourceenvironment.md): ссылка на географическое местонахождение ресурса. Применимо к сайтам SharePoint Online с несколькими географическими режимами.
- [connectedOrganization](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [entitlementManagementSettings](entitlementmanagementsettings.md): параметры на клиенте для управления правами Azure AD.

Руководство по использованию управления правами для создания пакета ресурсов, которые внутренние пользователи могут самостоятельно запрашивать, см. в руководстве по созданию пакета доступа с помощью [API Microsoft Graph.](/graph/tutorial-access-package-api)

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. У клиента, в котором используется управление правами, должна быть действительная приобретенная или пробная подписка на Azure AD Premium P2 или EMS E5.

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [получение](../api/entitlementmanagementsettings-get.md); | [entitlementManagementSettings](entitlementmanagementsettings.md) | Чтение свойств объекта **entitlementManagementSettings.** |
| [Update](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |
| [Список accessPackages](../api/accesspackage-list.md) | [Коллекция accessPackage](accesspackage.md) | Получить список объектов **accessPackage.** |
| [Создание accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Создание объекта **accessPackage.** |
| [Get accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Получить список объектов **accessPackageResourceRoleScope** для пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа. |
| [Список accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Получить список объектов **accessPackageAssignmentPolicy.** |
| [Создание accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Создание объекта **accessPackageAssignmentPolicy.** |
| [Get accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **accessPackageAssignmentPolicy.** |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта **accessPackageAssignmentPolicy.** |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление **accessPackageAssignmentPolicy.** |
| [Список accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Получить список объектов **accessPackageAssignmentRequest.** |
| [Создание accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создайте **новый accessPackageAssignmentRequest.** |
| [Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest.** |
| [Список accessPackageAssignments](../api/accesspackageassignment-list.md) | [Коллекция accessPackageAssignment](accesspackageassignment.md) | Получить список объектов **accessPackageAssignment.** |
| [Список accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [Коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Получить список объектов **accessPackageAssignmentResourceRole.** |
| [Get accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | **Извлечение объекта accessPackageAssignmentResourceRole.** |
| [Список accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [Коллекция accessPackageCatalog](accesspackagecatalog.md) | Получить список объектов **accessPackageCatalogs.** |
| [Создание accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создание объекта **accessPackageCatalog.** |
| [Get accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog.** |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog.** |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog.** |
| [Список ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Коллекция accessPackageResource](accesspackageresource.md) | Получить список объектов **accessPackageResource.** |
| [Список ролей ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Получить список объектов **accessPackageResourceRole.** |
| [Список accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [Коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Чтение свойств и связей объектов **accessPackageResourceRequest.** |
| [Создание accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создание объекта **accessPackageResourceRequest.** |
|[Список accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[Коллекция accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Получить список объектов [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Get accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Чтение свойств и связей объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
| [Список connectedOrganizations](../api/connectedorganization-list.md) | [Коллекция connectedOrganization](connectedorganization.md) | Получить список объектов **connectedOrganization.** |
| [Создание connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Создание объекта **connectedOrganization.** |
| [Get connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта **connectedOrganization.** |
| [Обновление connectedOrganization](../api/connectedorganization-update.md) |Нет | Обновление **connectedOrganization**. |
| [Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление **connectedOrganization**. |
|[Список internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получить список внутренних спонсоров **connectedOrganization.** |
|[Список externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получить список внешних спонсоров **connectedOrganization.** |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренних спонсоров **connectedOrganization.** |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу во внешних спонсоров **connectedOrganization.** |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удаление пользователя или группы из внутренних спонсоров **connectedOrganization.** |
|[Удаление externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удаление пользователя или группы из внешних спонсоров **connectedOrganization.** |

## <a name="types"></a>Типы

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md), [вопросы](accesspackagequestion.md) и [assignmentReviewSettings](assignmentreviewsettings.md) — используется в [accessPackageAssignmentPolicy,](accesspackageassignmentpolicy.md) чтобы указать, кто может запрашивать, кто утверждает и кто просматривает запросы на назначение пакета доступа для этой политики.
- [approvalStage](approvalstage.md) — используется в [approvalSettings](approvalsettings.md) для указания основных, резервных копий и утверждений эскалации.
- [userSet](userset.md) subtypes [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors,](internalsponsors.md)and [externalSponsors](externalsponsors.md) - Used in [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md) and [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) — используется в [accessPackageAssignment](accesspackageassignment.md) в качестве пользователя субъекта с назначением пакета доступа.
- [identitySource](identitysource.md) — используется в [connectedOrganization](connectedorganization.md), один из [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md).

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
