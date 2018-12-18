---
title: Работа с ресурсами Azure Active Directory в Microsoft Graph
description: Microsoft Graph для Azure Active Directory (Azure AD) предоставляет API-интерфейсы REST для управления организацией, ресурсы и средства.
ms.openlocfilehash: 85f44df36057220e4ea26eb8d9342e9fd1df5bb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305385"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Работа с ресурсами Azure Active Directory в Microsoft Graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Microsoft Graph предоставляет доступ к [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) ресурсы для поддержки сценариев, как управление ролями администратора (каталог) приглашать внешних пользователей к организации и, если вы являетесь [Облаке решения поставщика (CSP)](https://partner.microsoft.com/cloud-solution-provider) Управление данными клиента. Microsoft Graph также предоставляет методы приложения могут использовать, например, для получения сведений о транзитивное группы и роли членство. 

> **Примечание**. Некоторые ресурсы Azure AD описаны в других разделах справочника по API. Дополнительную информацию см. в статьях [Пользователи](users.md) и [Группы](group.md).


## <a name="authorization"></a>Авторизация
 
Для вызова API Microsoft Graph для ресурсов Azure AD приложению необходимы соответствующие разрешения. Для многих API, предоставляемых для ресурсов Azure AD, требуется одно из [разрешений _Directory_](/graph/permissions-reference#directory-permissions). Разрешения Directory дают широкие права и всегда предоставляются администратором. 

Чтобы приложение могло вызывать API AD Azure от имени пользователя (делегированные разрешения), этому пользователю должна быть назначена соответствующая [роль администратора](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles).

Дополнительные сведения о разрешениях, в том числе делегированных и для приложений, см. в [справочнике по разрешениям](/graph/permissions-reference). 

## <a name="common-use-cases"></a>Основные варианты использования 

В следующей таблице перечислены основные варианты использования ресурсов Azure AD.

| **Варианты использования**        | **Ресурсы REST** | **См. также** |
|:-----------------|:--------|:----------|
| **Объект и методы каталога** | | |
| `directoryObject` — это базовый класс, от которого наследуются многие ресурсы каталога, такие как пользователи и группы. Microsoft Graph предоставляет несколько методов, которые можно использовать для поиска сведений о пользователях, группах и других объектах каталога. Например, вы можете проверить транзитивное членство в списке групп, вернуть все группы и роли, транзитивным членом которых является объект каталога, или получить все ресурсы указанного типа (такие как пользователь или группа) из списка идентификаторов ролевых ресурсов. | [directoryObject](../resources/directoryobject.md) | Недоступно |
| **Управление ролями каталогов (администратор), административные единицы, параметры каталога и политики** | | |
| Активируйте роли каталога в клиенте Azure AD и управляйте членством пользователей в ролях каталога. Роли каталога также известны как роли администратора. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Назначение ролей администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Управление административные единиц измерения. Каталог роли делегировать полномочия клиента всей их члены. Администратор можно создавать и управлять административные единицы делегировать более модульного заданной областью административные полномочия для пользователей. | [administrativeUnit](../resources/administrativeunit.md) | [Управление административные единицы в Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Примените настройки предварительно заданных каталога через клиента или с экземплярами отдельных ресурсов. В настоящее время поддерживаются только параметры групп Office 365. Поведения элемента управления параметры каталога, такие как списки заблокированных word для отображения имен групп, гостя, могут ли пользователи группы владельцев и многое другое. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Командлеты Azure Active Directory для настройки параметров группы](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Применение политики Azure AD для приложений, субъектов-служб, групп или во всей организации. В настоящее время поддерживаются политики для срока жизни маркера и обнаружения домашней области.  | [политики](../resources/policy.md) | Н/Д |
| **Безопасный привилегированный доступ к Azure AD** | | |
| Управление и мониторинг привязкой время привилегированный доступ к каталогу и Azure ресурсы для администраторов и ИТ-специалистов с помощью управления правами удостоверения (PIM). | [Управление удостоверениями привилегированной API](../resources/privilegedidentitymanagement-root.md) | [Что такое Azure AD привилегированной управления удостоверениями](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| События рисков identity монитор как вход из зараженный вредоносных программ устройства или незнакомы расположений пользователей. | [API-Интерфейс службы защиты удостоверения](../resources/identityprotection-root.md) | [Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[События рисков Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events) |
| **Управление устройствами** | | |
| Управляйте устройствами, зарегистрированными в организации. Устройства (ноутбуки, настольные компьютеры, планшеты и мобильные телефоны) регистрируются на пользователей. Устройства обычно создаются в облаке с помощью службы регистрации устройств или Microsoft Intune. Они используются политиками условного доступа для многофакторной аутентификации. | [device](../resources/device.md) | [Приступая к работе с регистрацию устройств Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[Что такое InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Регистрация устройств для управления в Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Управление приложениями** | | |
| Управлять конфигурацией приложения в клиенте разработчика. | [application](../resources/application.md) | [Приложение и объекты службы Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Управлять приложениями, установленные в клиент. | [servicePrinicpal](../resources/serviceprincipal.md) | [Приложение и объекты службы Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Управление разрешениями согласие с пользователями и администраторами на приложения, установленные в клиент. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | Н/Д |
| Управление пользователей, группы и участие в группах основную роль службы на приложения, установленные в клиент. | [appRoleAssignment](../resources/approleassignment.md) | Н/Д |
| **Управление клиентами партнеров** | | |
| Получайте сведения об отношениях партнерства с клиентами. <br/><br/>**Примечание.** Это относится только к клиентам партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений Майкрософт](https://partnercenter.microsoft.com/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.| [contract](../resources/contract.md) | [Вызов Microsoft Graph из приложения Cloud Solution Provider](/graph/auth-cloudsolutionprovider) |
| Управляйте доменами, связанными с клиентом. С его помощью регистраторы могут автоматизировать связь домена для таких служб, как Office 365. | [domain](../resources/domain.md) | [Добавление имени личного домена в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Управление клиентами** | | |
| Получайте информацию об организации, например адрес, контакты для уведомлений и связи по техническим вопросам, планы обслуживания, на которые она подписана, и связанные с ней домены. | [organization](../resources/organization.md) | Недоступно |
| Получайте информацию о службах, на которые подписана компания. | [subscribedSku](../resources/subscribedsku.md) | Недоступно |
| Приглашайте внешних пользователей в организацию. | [invitation](../resources/invitation.md) | [Что такое служба совместной работы Azure AD B2B?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Проверка доступа** | | |
| Убедитесь, в группах и прав доступа приложения поддерживаются с помощью access обзоры | [Access дается обзор API](../resources/accessreviews-root.md) |[Дается обзор доступа Microsoft Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>Дальнейшие действия
Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше: 

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Explorer](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

