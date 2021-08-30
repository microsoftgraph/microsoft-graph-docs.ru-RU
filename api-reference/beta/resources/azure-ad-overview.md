---
title: Работа с ресурсами Azure Active Directory в Microsoft Graph
description: Microsoft Graph для Azure Active Directory (Azure AD) предоставляет REST API для управления организацией, ресурсами и активами.
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: identity-and-access
author: dkershaw10
ms.openlocfilehash: f9556ca4f908533b2934ec381368b0845917819e
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696325"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Работа с ресурсами Azure Active Directory в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph предоставляет доступ к ресурсам [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) для управления ролями администратора (каталога), приглашения внешних пользователей в организацию, и, если вы являетесь [поставщиком облачных решений](https://partner.microsoft.com/cloud-solution-provider), управления данными клиентов.  Microsoft Graph также предоставляет методы, которые могут использоваться приложениями, например для поиска информации о транзитивных группах и ролях пользователей.

> **Примечание**. Некоторые ресурсы Azure AD описаны в других разделах справочника по API. Дополнительную информацию см. в статьях [Пользователи](users.md) и [Группы](group.md).


## <a name="authorization"></a>Авторизация

Для вызова API Microsoft Graph для ресурсов Azure AD приложению необходимы соответствующие разрешения. Для многих API, предоставляемых для ресурсов Azure AD, требуется одно из [разрешений _Directory_](/graph/permissions-reference#directory-permissions). Разрешения Directory дают широкие права и всегда предоставляются администратором.

Чтобы приложение могло вызывать API AD Azure от имени пользователя (делегированные разрешения), этому пользователю должна быть назначена соответствующая [роль администратора](/azure/active-directory/active-directory-assign-admin-roles).

Дополнительные сведения о разрешениях, в том числе делегированных и для приложений, см. в [справочнике по разрешениям](/graph/permissions-reference).

## <a name="common-use-cases"></a>Основные варианты использования

В следующей таблице перечислены основные варианты использования ресурсов Azure AD.

| **Варианты использования**        | **Ресурсы REST** | **См. также** |
|:-----------------|:--------|:----------|
| **Объект и методы каталога** | | |
| `directoryObject` — это базовый класс, от которого наследуются многие ресурсы каталога, такие как пользователи и группы. Microsoft Graph предоставляет несколько методов, которые можно использовать для поиска сведений о пользователях, группах и других объектах каталога. Например, вы можете проверить транзитивное членство в списке групп, вернуть все группы и роли, транзитивным членом которых является объект каталога, или получить все ресурсы указанного типа (такие как пользователь или группа) из списка идентификаторов ролевых ресурсов. | [directoryObject](../resources/directoryobject.md) | Н/Д |
| **Управление ролями каталога (администратора), административными единицами, параметрами каталога и политикой** | | |
| Активация ролей каталога в клиенте Azure AD и управление участием пользователей в ролях каталога. Роли каталога также известны как роли администратора. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Назначение ролей администратора в Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles)|
| Управление административными единицами. Роли каталога делегируют полномочия на уровне клиента своим участниками. Администратор может создавать административные единицы и управлять ими, чтобы делегировать более детализированные административные полномочия пользователям. | [administrativeUnit](../resources/administrativeunit.md) | [Управление административными единицами в Azure AD](/azure/active-directory/active-directory-administrative-units-management) |
| Применение предопределенных параметров каталога к клиенту или экземплярам отдельных ресурсов. В настоящее время поддерживаются только параметры для групп Microsoft 365. Применение предопределенных параметров группы к клиенту или экземплярам отдельных ресурсов. Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, разрешение или запрещение пользователям-гостям быть владельцами групп, а также многие другие случаи. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Командлеты Azure Active Directory для настройки параметров группы](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Применение политики Azure AD к приложениям, субъектам-службам, группам или всей организации. Поддерживаются политики для сопоставления утверждений, выдачи маркеров, времени существования маркеров, обнаружения в домашней области и других функций.  | [Доступные политики](../resources/policy-overview.md) | Недоступно |
| **Защита привилегированного доступа к Azure AD** | | |
| Отслеживание и управление ограниченным по времени привилегированным доступом к каталогу и ресурсам Azure для администраторов и ИТ-специалистов с помощью службы Privileged Identity Management (PIM). | [Privileged Identity Management API](../resources/privilegedidentitymanagement-root.md) | [Что такое Azure AD Privileged Identity Management?](/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Отслеживание событий с риском для идентификации, например входа пользователей с устройств, зараженных вредоносными программами, или из незнакомых расположений. | [API службы защиты идентификации](../resources/identityprotection-root.md) | [Защита идентификации Azure Active Directory](/azure/active-directory/active-directory-identityprotection)<br/><br/>[События с риском Azure Active Directory](/azure/active-directory/active-directory-reporting-risk-events) |
| **Управление устройствами** | | |
| Управляйте устройствами, зарегистрированными в организации. Устройства (ноутбуки, настольные компьютеры, планшеты и мобильные телефоны) регистрируются на пользователей. Устройства обычно создаются в облаке с помощью службы регистрации устройств или Microsoft Intune. Они используются политиками условного доступа для многофакторной аутентификации. | [device](../resources/device.md) | [Знакомство с регистрацией устройств в Azure Active Directory](/azure/active-directory/active-directory-device-registration-overview) |
| **Управление приложениями** | | |
| Управление настройкой приложения в клиенте разработчика. | [application](../resources/application.md) | [Объекты приложения и субъекта-службы в Azure Active Directory](/azure/active-directory/develop/active-directory-application-objects) |
| Управление приложениями, установленными в клиенте. | [servicePrinicpal](../resources/serviceprincipal.md) | [Объекты приложения и субъекта-службы в Azure Active Directory](/azure/active-directory/develop/active-directory-application-objects) |
| Управление разрешениями с согласия пользователей и администраторов в приложениях, установленных в клиенте. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | Н/Д |
| Управление участием в ролях для пользователей, групп и субъектов-служб в приложениях, установленных в клиенте. | [appRoleAssignment](../resources/approleassignment.md) | Н/Д |
| **Управление клиентами партнеров** | | |
| Получайте сведения об отношениях партнерства с клиентами. <br/><br/>**Примечание.** Это относится только к клиентам партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений Майкрософт](https://partnercenter.microsoft.com/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.| [contract](../resources/contract.md) | [Вызов Microsoft Graph из приложения Cloud Solution Provider](/graph/auth-cloudsolutionprovider) |
| Управление доменами, связанными с клиентом. Действия с доменами позволяют регистраторам автоматизировать установление связей доменов для таких служб, как Microsoft 365. | [domain](../resources/domain.md); | [Добавление имени личного домена в Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Управление клиентами** | | |
| Получайте информацию об организации, например адрес, контакты для уведомлений и связи по техническим вопросам, планы обслуживания, на которые она подписана, и связанные с ней домены. | [organization](../resources/organization.md) | Недоступно |
| Получайте информацию о службах, на которые подписана компания. | [subscribedSku](../resources/subscribedsku.md) | Недоступно |
| Приглашайте внешних пользователей в организацию. | [invitation](../resources/invitation.md) | [Что такое служба совместной работы Azure AD B2B?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| Управляйте фирменной символикой для интерфейса входа организации. | [organizationalbranding](../resources/organizationalbrandingproperties.md) | [Добавление фирменной символики на страницу входа в Azure Active Directory вашей организации](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)|
| **Проверки доступа** | | |
| Проверяйте правильность участия в группах и права доступа к приложению с помощью проверок доступа. | [API проверки доступа](../resources/accessreviews-root.md) |[Проверки доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
| **Запросы согласия** | | |
| Управление рабочим процессом запроса согласия для пользователей, пытающихся получить доступ к приложениям, для которых требуется авторизация администратора.  | [API запросов согласия](../resources/consentrequests-root.md) |[Настройка рабочего процесса согласия администратора](/azure/active-directory/manage-apps/configure-admin-consent-workflow) |

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).
