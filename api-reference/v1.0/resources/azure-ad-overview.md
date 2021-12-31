---
title: Работа с ресурсами Azure Active Directory в Microsoft Graph
description: 'Microsoft Graph предоставляет доступ к ресурсам Azure Active Directory (Azure AD) для управления ролями администратора (каталога), приглашения внешних пользователей в организацию, и, если вы являетесь поставщиком облачных решений, управления данными клиентов.  Microsoft Graph также предоставляет методы, которые могут использоваться приложениями, например для поиска информации о транзитивных группах и ролях пользователей. '
ms.localizationpriority: high
author: dkershaw10
ms.prod: identity-and-access
doc_type: conceptualPageType
ms.openlocfilehash: fd58ab506d7fe0df4c1802e004c51a25de52bdbd
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650519"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Работа с ресурсами Azure Active Directory в Microsoft Graph

Microsoft Graph предоставляет доступ к ресурсам [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) для управления ролями администратора (каталога), приглашения внешних пользователей в организацию, и, если вы являетесь [поставщиком облачных решений](https://partner.microsoft.com/cloud-solution-provider), управления данными клиентов.  Microsoft Graph также предоставляет методы, которые могут использоваться приложениями, например для поиска информации о транзитивных группах и ролях пользователей.

> **Примечание**. Некоторые ресурсы Azure AD описаны в других разделах справочника по API. Дополнительную информацию см. в статьях [Пользователи](users.md) и [Группы](group.md).


## <a name="authorization"></a>Авторизация

Для вызова API Microsoft Graph для ресурсов Azure AD приложению необходимы соответствующие разрешения. Для многих API, предоставляемых для ресурсов Azure AD, требуется одно из [разрешений _Directory_](/graph/permissions-reference#directory-permissions). Разрешения Directory дают широкие права и всегда предоставляются администратором.

Чтобы приложение могло вызывать API AD Azure от имени пользователя (делегированные разрешения), этому пользователю должна быть назначена соответствующая [роль администратора](/azure/active-directory/active-directory-assign-admin-roles).

Дополнительные сведения о разрешениях, в том числе делегированных и для приложений, см. в [справочнике по разрешениям](/graph/permissions-reference).

## <a name="common-use-cases"></a>Основные варианты использования

В следующей таблице перечислены основные варианты использования ресурсов Azure AD.

| **Варианты использования**        | **Ресурсы REST** | **См. также** |
|:---------------|:--------|:----------|
| **Объект и методы каталога** | | |
| `directoryObject` — это базовый класс, от которого наследуются многие ресурсы каталога, такие как пользователи и группы. Microsoft Graph предоставляет несколько методов, которые можно использовать для поиска сведений о пользователях, группах и других объектах каталога. Например, вы можете проверить транзитивное членство в списке групп, вернуть все группы и роли, транзитивным членом которых является объект каталога, или получить все ресурсы указанного типа (такие как пользователь или группа) из списка идентификаторов ролевых ресурсов. | [directoryObject](../resources/directoryobject.md) | Недоступно |
| **Управление ролями каталога (администратора)** | | |
| Активируйте роли каталога в клиенте Azure AD и управляйте членством пользователей в ролях каталога. Роли каталога также известны как роли администратора. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | [Назначение ролей администратора в Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles) |
| Применение предопределенных параметров группы к клиенту или экземплярам отдельных ресурсов. Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, разрешение или запрещение пользователям-гостям быть владельцами групп, а также многие другие случаи. | [groupSetting](../resources/groupsetting.md) <br/>[groupSettingTemplate](../resources/groupsettingtemplate.md)| [Командлеты Azure Active Directory для настройки параметров группы](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| **Управление устройствами** | | |
| Управляйте устройствами, зарегистрированными в организации. Устройства (ноутбуки, настольные компьютеры, планшеты и мобильные телефоны) регистрируются на пользователей. Устройства обычно создаются в облаке с помощью службы регистрации устройств или Microsoft Intune. Они используются политиками условного доступа для многофакторной аутентификации. | [device](../resources/device.md) | [Знакомство с регистрацией устройств в Azure Active Directory](/azure/active-directory/active-directory-device-registration-overview).<br/><br/>[Что такое InTune?](/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Регистрация устройств для управления в Intune](/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Управление клиентами партнеров** | | |
| Получайте сведения об отношениях партнерства с клиентами.<br/><br/>**Примечание.** Это относится только к клиентам партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений Майкрософт](https://partnercenter.microsoft.com/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor. | [contract](../resources/contract.md) | [Вызов Microsoft Graph из приложения Cloud Solution Provider](/graph/auth-cloudsolutionprovider) |
| Управление доменами, связанными с клиентом. Действия с доменами позволяют регистраторам автоматизировать установление связей доменов для таких служб, как Microsoft 365. | [domain](../resources/domain.md); | [Добавление имени личного домена в Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Управление клиентами** | | |
| Получайте информацию об организации, например адрес, контакты для уведомлений и связи по техническим вопросам, планы обслуживания, на которые она подписана, и связанные с ней домены. | [organization](../resources/organization.md) | Недоступно |
| Получайте информацию о службах, на которые подписана компания. | [subscribedSku](../resources/subscribedsku.md) | Недоступно |
| Приглашайте внешних пользователей в организацию. | [invitation](../resources/invitation.md) | [Что такое служба совместной работы Azure AD B2B?](/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b) |
| Управляйте фирменной символикой для интерфейса входа организации. | [organizationalbranding](../resources/organizationalbranding.md) | [Добавление фирменной символики на страницу входа в Azure Active Directory вашей организации](/azure/active-directory/fundamentals/customize-branding)|
| **Запросы согласия** | | |
| Управление рабочим процессом запроса согласия для пользователей, пытающихся получить доступ к приложениям, для которых требуется авторизация администратора.  | [API запросов согласия](../resources/consentrequests-overview.md) |[Настройка рабочего процесса согласия администратора](/azure/active-directory/manage-apps/configure-admin-consent-workflow) |

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).
