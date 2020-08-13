---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 2dfeaa8ba656adac608de31028772f8b5665f4f0
ms.sourcegitcommit: 2e6fb1c0fef8cb3af1a72c115aa54902c71c99f5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658230"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="august-2020-new-and-generally-available"></a>Август 2020 г.: новые и общедоступные возможности

### <a name="change-notifications"></a>Уведомления об изменениях
[Отслеживание изменений](delta-query-overview.md) поддерживаемых ресурсов в национальном облаке Microsoft Graph для государственных организаций США.


## <a name="august-2020-new-in-preview-only"></a>Август 2020 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Поддержка единого входа на основе паролей в ресурсах приложения [субъекта-службы](/graph/api/resources/serviceprincipal?view=graph-rest-beta) и указание таких [параметров](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta) в свойстве **passwordSingleSignOnSettings**. Сведения о едином входе на основе паролей в Azure AD см. в статье [Настройка единого входа на основе пароля](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте свойство **includeResourceData** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta) для [настройки уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md). Не используйте свойство **includeProperties**.
- Получение [уведомлений об изменениях, доставляемых через концентратор событий](change-notifications-delivery.md).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [условий соглашения об использовании](/graph/api/resources/agreement?view=graph-rest-beta) для поддержки срока действия и периодичности соглашения с обязательным принятием пользователем соглашения на отдельных устройствах или повторным принятием соглашения с установленной периодичностью. 
- Используйте свойство **file** для перехода к [настраиваемому соглашению](/graph/api/resources/agreementfile?view=graph-rest-beta) условий. Не используйте свойство **files**.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение [отчетов об использовании приложений Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta), в частности сведений о пользователе, количества пользователей и количества используемых платформ.

### <a name="teamwork"></a>Командная работа
Получение [контента, размещенного в сообщении чата](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta), например изображений или фрагментов кода. См. [пример](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&branch=master#example-2-get-hosted-content-bytes-for-an-image), чтобы получить количество байтов содержимого для изображения.

## <a name="july-2020-new-and-generally-available"></a>Июль 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
GA функции, которая позволяет организаторам предлагать альтернативное время собраний, а приглашенным [предлагать новое время для собрания](outlook-calendar-meeting-proposals.md), когда они [предварительно принимают](/graph/api/event-tentativelyaccept?view=graph-rest-1.0) или[отклоняют](/graph/api/event-decline?view=graph-rest-1.0) событие.

### <a name="change-notifications"></a>Уведомления об изменениях
Удалено ошибочно реализованное свойство **sequenceNumber** из ресурса [changeNotification](/graph/api/resources/changenotification).

### <a name="groups"></a>Группы
Общая доступность следующих свойств объекта [group](/graph/api/resources/group?view=graph-rest-v1.0): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** и **theme**.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Удаление пользователя в качестве зарегистрированного владельца или пользователя [устройства](/graph/api/resources/device).
- Отслеживайте изменения в новых, обновленных или удаленных локальных представлениях приложений (представленных ресурсами[servicePrincipals](/graph/api/resources/serviceprincipal)) и делегированных разрешениях (представленных ресурсами [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) без полного чтения всей коллекции ресурсов.
- GA [политики обеспечения безопасности по умолчанию](/graph/api/resources/identitysecuritydefaultsenforcementpolicy), которая защищает организации от распространенных атак.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- GA [политик условного доступа](/graph/api/resources/conditionalAccessPolicy), которые являются настраиваемыми правилами, определяющими сценарии доступа.
- GA [именованных расположений](/graph/api/resources/namedLocation), представляющих собой настраиваемые правила, которые определяют сетевые расположения, используемые в политике условного доступа.

### <a name="schema-extensions"></a>Расширения схемы
Функция [расширений схемы](/graph/api/resources/schemaextension) теперь общедоступна в [Microsoft Cloud for US Government](/graph/deployments).

### <a name="teamwork"></a>Командная работа
Используйте делегированные разрешения `TeamsAppInstallation.ReadForTeam` или`TeamsAppInstallation.ReadWriteForTeam`, или разрешения приложений `TeamsAppInstallation.ReadForTeam.All` или `TeamsAppInstallation.ReadWriteForTeam.All`, чтобы [составить список приложений, установленных в группе](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Июль 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Использование операции [update](/graph/api/onlinemeeting-update?view=graph-rest-beta), чтобы обновить свойство **startDateTime**, **endDateTime**, **participants** или **subject** для [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Подписка на уведомления об изменениях о доступности пользователя в Microsoft Teams, представленной ресурсом [presence](/graph/api/resources/presence?view=graph-rest-beta).

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- [Получение](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) записей звонков по ТСОП.
- [Получение](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) записей звонков прямой маршрутизации.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Появление [дел обнаружения электронных данных](/graph/api/resources/ediscoverycase?view=graph-rest-beta), которые могут содержать хранителей, удержания, коллекции, наборы для проверки и операции экспорта, доступные для использования в качестве доказательств в судебных делах.
Приложения теперь могут [запрашивать](/graph/api/resources/reviewsetquery?view=graph-rest-beta) и вызывать [данные наборов для проверки](/graph/api/resources/reviewset?view=graph-rest-beta), собранные для использования в судебных разбирательствах, расследованиях и нормативных запросах. Это добавление входит в состав [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide) Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Использование разрешения приложений `Printer.ReadWrite.All` и [шифрования Internet Printing Protocol (IPP)](https://tools.ietf.org/html/rfc8010) для [обновления принтера](/graph/api/printer-update?view=graph-rest-beta).
- Использование разрешений приложений `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All` или `PrintJob.ReadWrite.All` для [получения задания печати](/graph/api/printjob-get?view=graph-rest-beta) или [перечисления заданий печати для принтера](/graph/api/printer-list-jobs?view=graph-rest-beta).
- При [получении задания печати](/graph/api/printjob-get?view=graph-rest-beta) используйте `$expand` для получения [задач печати](/graph/api/resources/printtask?view=graph-rest-beta), выполняемых или выполненных в рамках задания. Задачи печати, [определения задач](/graph/api/resources/printtaskdefinition?view=graph-rest-beta) и [триггеры задач](/graph/api/resources/printtasktrigger?view=graph-rest-beta) используются при [печати по запросу](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Перенаправление задания печати](/graph/api/printjob-redirect?view=graph-rest-beta) на другой принтер в рамках печати по запросу.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июль](changelog.md#july-2020) в бета-версии.

### <a name="groups"></a>Группы
Используйте свойство **isAssignableToRole** [группы](/graph/api/resources/group?view=graph-rest-beta) Microsoft 365 и настройте его при создании группы, чтобы указать, можно ли назначить группу для роли Azure AD. Эта [помогает управлять назначениями ролей в Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept). Например, вместо назначения отдельным пользователям роли Azure AD привилегированный администратор ролей или глобальный администратор может создать группу Microsoft 365 и назначить ее этой роли, чтобы при присоединении пользователей к _группе_ им неявно назначалась нужная роль.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Получите маркер доступа](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta) для авторизации службы контроля использования Azure AD для предоставления пользователям доступа к приложению.
- [Получите](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta) или[обновите](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta)настройки управления правами, которые контролируют доступ к группам, приложениям и сайтам SharePoint Online для пользователей внутри или вне вашей организации. 

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Включение уровней риска пользователя (`low`, `medium`, `high`, `none`) при рассмотрении применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- [Использование смены пароля в качестве предоставления управления](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control), чтобы пройти политику условного доступа.
- Использование [поставщика Open ID Connect](/graph/api/resources/openidconnectprovider?view=graph-rest-beta) (ODIC) в качестве поставщика удостоверений в клиенте Azure AD и клиенте Azure AD B2C. Его свойство **claimsMapping** позволяет Azure AD [сопоставлять утверждения](/graph/api/resources/claimsmapping?view=graph-rest-beta) от поставщика OIDC с утверждениями, которые распознает и использует Azure AD.

### <a name="people-and-workplace-intelligence--insights"></a>Люди и рабочая аналитика | Аналитические сведения
Используйте более [детальное управление конфиденциальностью](insights-customize-item-insights-privacy.md) в отношении доступности и отображения[элементов аналитики](/graph/api/resources/iteminsights?view=graph-rest-beta) в Microsoft 365. Эти данные представляют собой отношения между пользователем и документами в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Люди и рабочая аналитика | Настройка карточки профиля
Администраторы могут [настроить свойства, представленные в карточке профиля для своих организаций](add-properties-profilecard.md), используя API-интерфейс для [свойств карточки профиля](/graph/api/resources/profilecardproperty?view=graph-rest-beta).

### <a name="sites-and-lists"></a>Сайты и списки
Доступ к таксономии [банка терминов](/graph/api/resources/termstore-store?view=graph-rest-beta) SharePoint — иерархии, состоящей из ресурсов [group](/graph/api/resources/termstore-group?view=graph-rest-beta), [set](/graph/api/resources/termstore-set?view=graph-rest-beta) и [term](/graph/api/resources/termstore-term?view=graph-rest-beta), а также ресурсов [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta) для связей между терминами.

### <a name="workbooks-and-charts"></a>Книги и диаграммы
[Получение состояния и любого результата](/graph/api/workbookoperation-get?view=graph-rest-beta) длительной [операции](/graph/api/resources/workbookoperation?view=graph-rest-beta) в [книге](/graph/api/resources/workbook?view=graph-rest-beta).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

