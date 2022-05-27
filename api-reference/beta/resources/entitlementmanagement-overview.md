---
title: Работа с API Azure AD управления правами
description: Управление доступом к ресурсам, включая группы, приложения и сайты, Azure AD управления правами
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 520d786906963250024121144865cfcf15e07560
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694737"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API Azure AD управления правами

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) позволяет управлять доступом к группам, приложениям и сайтам SharePoint Online для внутренних пользователей, а также пользователей за пределами организации.

Создавая пакеты доступа с ролями, которые должны иметь пользователи в этих ресурсах, и определяя политики для пользователей, которые могут запрашивать пакет доступа и как долго они могут иметь назначение пакету доступа, вы можете управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

К типам ресурсов управления правами относятся:

- [accessPackage](accesspackage.md): определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md): указывает политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа через назначение пакета доступа.
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md): создается пользователем, который хочет получить назначение пакета доступа.
- [accessPackageAssignment](accesspackageassignment.md): назначение пакета доступа определенной теме на определенный период времени.
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md): указывает роль конкретного ресурса, которой субъект был назначен с помощью назначения пакета доступа.
- [accessPackageCatalog](accesspackagecatalog.md): контейнер для пакетов доступа.
- [accessPackageResource](accesspackageresource.md): ссылка на ресурс, связанный с каталогом пакетов для доступа.
- [accessPackageResourceRequest](accesspackageresourcerequest.md): запрос на добавление ресурса в каталог пакетов для доступа.
- [accessPackageResourceEnvironment](accesspackageresourceenvironment.md): ссылка на географическое положение ресурса. Применимо к сайтам с поддержкой нескольких регионов SharePoint Online.
- [connectedOrganization](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [entitlementManagementSettings](entitlementmanagementsettings.md): параметры на уровне клиента для Azure AD управления правами.
- [утверждение](approval.md): представляет решения, связанные с запросом пакета доступа.

Кроме того, назначениями ролей для ролей управления правами можно управлять с помощью определений ролей [управления правами](unifiedroledefinition.md).

Учебник, в котором показано, как использовать управление [правами](/graph/tutorial-access-package-api) для создания пакета ресурсов, которые внутренние пользователи могут самостоятельно запрашивать, см. в статье "Создание пакета доступа с помощью API Graph Майкрософт".

Обратите внимание, что функция управления правами, включая API, включена в Azure AD Premium P2. Клиент, в котором используется управление правами, должен иметь допустимую приобретенную или пробную Azure AD Premium P2 или подписку EMS E5. Дополнительные сведения о требованиях к лицензиям для функции управления правами см. в разделе ["Требования к лицензии на управление правами"](/azure/active-directory/governance/entitlement-management-overview#license-requirements).

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением правами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [Получение](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Чтение свойств объекта **entitlementManagementSettings** . |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings** . |
| [Перечисление accessPackage](../api/entitlementmanagement-list-accesspackages.md) | [Коллекция accessPackage](accesspackage.md) | Получение списка объектов **accessPackage** . |
| [Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Создайте объект **accessPackage** . |
| [Получение accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accessPackage** . |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage** . |
| [Удаление accessPackage](../api/accesspackage-delete.md) | | Удаление **accessPackage**. |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [Коллекция accessPackage](accesspackage.md) | Получение списка объектов **accessPackage** , отфильтрованных по пользователю, выполнившего вход. |
| [Перечисление accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Получение списка объектов **accessPackageResourceRoleScope** для пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте объект **accessPackageResourceRoleScope** для пакета доступа. |
| [Перечисление несовместимых пакетовAccessPackage](../api/accesspackage-list-incompatibleaccesspackages.md) | [Коллекция accessPackage](accesspackage.md) | Получение списка несовместимых объектов **accesspackage** для этого пакета доступа. |
| [Добавление accessPackage в incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Нет | Добавьте ссылку, чтобы указать, что **другой пакет доступа** несовместим с указанным пакетом доступа. |
| [Удаление accessPackage из несовместимых пакетовAccessPackage](../api/accesspackage-delete-incompatibleaccesspackage.md) | Нет | Удалите ссылку, указывающее на **несовместимость accesspackage** . |
| [Список несовместимых групп](../api/accesspackage-list-incompatiblegroups.md) | Коллекция [group](group.md) | Получение списка несовместимых объектов **группы** для этого пакета доступа. |
| [Добавление группы в несовместимые группы](../api/accesspackage-post-incompatiblegroup.md) | Нет | Добавьте ссылку, чтобы указать, что членство **в группе** несовместимо с указанным пакетом доступа. |
| [Удаление группы из несовместимых групп](../api/accesspackage-delete-incompatiblegroup.md) | Нет | Удалите ссылку, **указывающее** , что членство в группе несовместимо.|
| [Перечисление accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [Коллекция accessPackage](accesspackage.md) | Получение списка объектов  **accesspackage** , в которых этот пакет доступа содержит список несовместимых. |
| [Перечисление accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Получение списка объектов **accessPackageAssignmentPolicy** . |
| [Создание accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Создайте объект **accessPackageAssignmentPolicy** . |
| [Получение accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **accessPackageAssignmentPolicy** . |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта **accessPackageAssignmentPolicy** . |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление **accessPackageAssignmentPolicy**. |
| [Перечисление accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Получение списка объектов **accessPackageAssignmentRequest** . |
| [Создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создайте **новый accessPackageAssignmentRequest**. |
| [Получение accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **accessPackageAssignmentRequest** . |
| [Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |Нет | Удаление **объекта accessPackageAssignmentRequest**. |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[Коллекция accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Получение списка объектов **accessPackageAssignmentRequest** , отфильтрованных по пользователю, выполнившего вход.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[Коллекция accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest**, который находится в состоянии отмены: `accepted`, `pendingApproval`, , `pendingApprovalEscalated``pendingNotBefore`.|
| [Перечисление объектов accessPackageAssignment](../api/entitlementmanagement-list-accesspackageassignments.md) | [Коллекция accessPackageAssignment](accesspackageassignment.md) | Получение списка объектов **accessPackageAssignment** . |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** , отфильтрованных по пользователю, выполнившего вход.|
| [Повторная обработка](../api/accesspackageassignment-reprocess.md) | Нет | Автоматически переоценка и принудительное применение назначений пользователя для определенного пакета доступа.|
| [коллекция additionalAccess](../api/accesspackageassignment-additionalaccess.md) [accessPackageAssignment](../resources/accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** для пользователей, имеющих назначения несовместимым пакетам доступа.|
| [Перечисление accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md) | [Коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Получение списка объектов **accessPackageAssignmentResourceRole** . |
| [Получение accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Получение объекта **accessPackageAssignmentResourceRole** . |
| [Перечисление accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [Коллекция accessPackageCatalog](accesspackagecatalog.md) | Получение списка объектов **accessPackageCatalogs** . |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте объект **accessPackageCatalog** . |
| [Получение accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта **accessPackageCatalog** . |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **accessPackageCatalog** . |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление **accessPackageCatalog**. |
| [Перечисление ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Коллекция accessPackageResource](accesspackageresource.md) | Получение списка объектов **accessPackageResource** . |
| [Перечисление ролей ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Получение списка объектов **accessPackageResourceRole** . |
| [Перечисление accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [Коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Чтение свойств и связей объектов **accessPackageResourceRequest** . |
| [Создание accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создайте объект **accessPackageResourceRequest** . |
|[Перечисление accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[Коллекция accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Получение списка объектов [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) .|
|[Получение accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Чтение свойств и связей объекта [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) .|
| [Перечисление объектов connectedOrganization](../api/entitlementmanagement-list-connectedorganizations.md) | [коллекция connectedOrganization](connectedorganization.md) | Получение списка объектов **connectedOrganization** . |
| [Создание connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | Создайте объект **connectedOrganization** . |
| [Получение connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Чтение свойств и связей объекта **connectedOrganization** . |
| [Обновление connectedOrganization](../api/connectedorganization-update.md) |Нет | Обновление **connectedOrganization**. |
| [Удаление connectedOrganization](../api/connectedorganization-delete.md) |Нет | Удаление **connectedOrganization**. |
|[Перечисление объектов internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внутренних спонсоров **connectedOrganization** . |
|[Перечисление объектов externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внешних спонсоров **connectedOrganization** . |
|[Добавление internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавьте пользователя или группу во внутренних спонсоров **connectedOrganization** . |
|[Добавление externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавьте пользователя или группу во внешних спонсоров **connectedOrganization** . |
|[Удаление internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удалите пользователя или группу из внутренних спонсоров **connectedOrganization** . |
|[Получение утверждения](../api/approval-get.md) | [утверждение](approval.md) | Получение свойств объекта **утверждения** . |
|[Список approvalSteps](../api/approval-list-steps.md) | [Коллекция approvalStep](approvalstep.md) | Вывод списка **объектов approvalStep** , связанных с **объектом утверждения** . |
|[Получение approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Получение свойств объекта **approvalStep** . |
|[Обновление approvalStep](../api/approvalstep-update.md) | Нет | Примените утверждение или отклонение решения для **объекта approvalStep** . |


## <a name="types"></a>Типы

- [requestorSettings](requestorsettings.md), [approvalSettings](approvalsettings.md), [вопросы](accesspackagequestion.md) и [assignmentReviewSettings](assignmentreviewsettings.md) — используется в [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) , чтобы указать, кто может запрашивать, кто утверждает и кто проверяет запросы на назначение пакетов для этой политики.
- [approvalStage —](approvalstage.md) используется в [approvalSettings](approvalsettings.md) для указания основных утверждающих лиц, утверждающих резервное копирование и эскалацию.
- [approvalStep —](approvalstep.md) используется в [утверждении для](approval.md) различения различных шагов утверждения.
- [userSet](userset.md) subtypes [singleUser](singleuser.md), [groupMembers](groupmembers.md), [connectedOrganizationMembers](connectedorganizationmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md), and [externalSponsors](externalsponsors.md) - Used in [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md), [approvalStep](approvalstep.md) and [assignmentReviewSettings](assignmentreviewsettings.md).
- [accessPackageSubject](accesspackagesubject.md) — используется в [accessPackageAssignment](accesspackageassignment.md) в качестве пользователя субъекта с назначением пакета доступа.
- [identitySource](identitysource.md) — используется в [connectedOrganization](connectedorganization.md), одном из [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [crossCloudAzureActiveDirectoryTenant](crosscloudazureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md).

## <a name="see-also"></a>См. также

 - [Что такое Azure AD управления правами?](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
