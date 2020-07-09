---
title: Работа с ресурсами Azure Active Directory в Microsoft Graph
description: Microsoft Graph для Azure Active Directory (Azure AD) предоставляет REST API для управления организацией, ресурсами и активами.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b2d6bff52e7defbf487b0cbe9016dd278591588b
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080872"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Работа с ресурсами Azure Active Directory в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph предоставляет доступ к ресурсам [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) для управления ролями администратора (каталога), приглашения внешних пользователей в организацию, и, если вы являетесь [поставщиком облачных решений](https://partner.microsoft.com/cloud-solution-provider), управления данными клиентов.  Microsoft Graph также предоставляет методы, которые могут использоваться приложениями, например для поиска информации о транзитивных группах и ролях пользователей.

> **Note**: Some Azure AD resources are documented in other sections of the API reference. For more information, see [Users](users.md) and [Groups](group.md).


## <a name="authorization"></a>Авторизация

To call the Microsoft Graph APIs on Azure AD resources, your app will need the appropriate permissions. Many of the APIs exposed on Azure AD resources require one of the [_Directory_ permissions](/graph/permissions-reference#directory-permissions). Directory permissions are highly privileged and always require administrator consent.

Чтобы приложение могло вызывать API AD Azure от имени пользователя (делегированные разрешения), этому пользователю должна быть назначена соответствующая [роль администратора](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles).

Дополнительные сведения о разрешениях, в том числе делегированных и для приложений, см. в [справочнике по разрешениям](/graph/permissions-reference).

## <a name="common-use-cases"></a>Основные варианты использования

В следующей таблице перечислены основные варианты использования ресурсов Azure AD.

| **Варианты использования**        | **Ресурсы REST** | **См. также** |
|:-----------------|:--------|:----------|
| **Объект и методы каталога** | | |
| `directoryObject` is the base class that many directory resources, like users and groups, inherit from. Microsoft Graph exposes several methods that you can use to discover information about users, groups, and other directory objects. For example, you can check for transitive membership in a list of groups, return all the groups and directory roles that a directory object is a transitive member of, or get all the resources of a specified type (like user or group) from a list of generic resource IDs. | [directoryObject](../resources/directoryobject.md) | Н/Д |
| **Управление ролями каталога (администратора), административными единицами, параметрами каталога и политикой** | | |
| Activate directory roles in an Azure AD tenant and manage user memberships in directory roles. Directory roles are also known as administrator roles. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Назначение ролей администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Управление административными единицами. Роли каталога делегируют полномочия на уровне клиента своим участниками. Администратор может создавать административные единицы и управлять ими, чтобы делегировать более детализированные административные полномочия пользователям. | [administrativeUnit](../resources/administrativeunit.md) | [Управление административными единицами в Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Применение предопределенных параметров каталога к клиенту или экземплярам отдельных ресурсов. В настоящее время поддерживаются только параметры для групп Microsoft 365. Применение предопределенных параметров группы к клиенту или экземплярам отдельных ресурсов. Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, разрешение или запрещение пользователям-гостям быть владельцами групп, а также многие другие случаи. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Командлеты Azure Active Directory для настройки параметров группы](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Применение политики Azure AD к приложениям, субъектам-службам, группам или всей организации. Поддерживаются политики для сопоставления утверждений, выдачи маркеров, времени существования маркеров, обнаружения в домашней области и других функций.  | [Доступные политики](../resources/policy-overview.md) | Недоступно |
| **Защита привилегированного доступа к Azure AD** | | |
| Отслеживание и управление ограниченным по времени привилегированным доступом к каталогу и ресурсам Azure для администраторов и ИТ-специалистов с помощью службы Privileged Identity Management (PIM). | [Privileged Identity Management API](../resources/privilegedidentitymanagement-root.md) | [Что такое Azure AD Privileged Identity Management?](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Отслеживание событий с риском для идентификации, например входа пользователей с устройств, зараженных вредоносными программами, или из незнакомых расположений. | [API службы защиты идентификации](../resources/identityprotection-root.md) | [Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[События с риском Azure Active Directory](/azure/active-directory/active-directory-reporting-risk-events) |
| **Управление устройствами** | | |
| Manage devices registered in the organization. Devices are registered to users and include items like laptops, desktops, tablets, and mobile phones. Devices are typically created in the cloud using the Device Registration Service or by Microsoft Intune. They're used by conditional access policies for multifactor authentication. | [device](../resources/device.md) | [Знакомство с регистрацией устройств в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[Что такое InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Регистрация устройств для управления в Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Управление приложениями** | | |
| Управление настройкой приложения в клиенте разработчика. | [application](../resources/application.md) | [Объекты приложения и субъекта-службы в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Управление приложениями, установленными в клиенте. | [servicePrinicpal](../resources/serviceprincipal.md) | [Объекты приложения и субъекта-службы в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Управление разрешениями с согласия пользователей и администраторов в приложениях, установленных в клиенте. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | Н/Д |
| Управление участием в ролях для пользователей, групп и субъектов-служб в приложениях, установленных в клиенте. | [appRoleAssignment](../resources/approleassignment.md) | Н/Д |
| **Управление клиентами партнеров** | | |
| Получайте сведения об отношениях партнерства с клиентами. <br/><br/>**Note:** This applies to partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of the [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.| [contract](../resources/contract.md) | [Вызов Microsoft Graph из приложения Cloud Solution Provider](/graph/auth-cloudsolutionprovider) |
| Manage domains associated with a tenant. Domain operations enable registrars to automate domain association for services such as Microsoft 365. | [domain](../resources/domain.md); | [Добавление имени личного домена в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Управление клиентами** | | |
| Получайте информацию об организации, например адрес, контакты для уведомлений и связи по техническим вопросам, планы обслуживания, на которые она подписана, и связанные с ней домены. | [organization](../resources/organization.md) | Недоступно |
| Получайте информацию о службах, на которые подписана компания. | [subscribedSku](../resources/subscribedsku.md) | Недоступно |
| Приглашайте внешних пользователей в организацию. | [invitation](../resources/invitation.md) | [Что такое служба совместной работы Azure AD B2B?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Проверки доступа** | | |
| Проверка правильности участия в группах и прав доступа к приложению с помощью проверок доступа | [API проверки доступа](../resources/accessreviews-root.md) |[Проверки доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
Directory resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph. To learn more:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Explorer](https://developer.microsoft.com/graph/graph-explorer).

Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

