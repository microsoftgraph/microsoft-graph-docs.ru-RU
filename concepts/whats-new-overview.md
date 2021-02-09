---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6779d735c1c445ce3910fa649b3273405fc7d6da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159390"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.


## <a name="february-2021-new-in-preview-only"></a>Февраль 2021 г.: новые возможности только в предварительной версии

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Назначение данных географического расположения [пакету доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) ресурсу в [запросе на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Получение списка всех [сред ресурсов пакета доступа](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true), представляющих географические расположения, в которых хранятся ресурсы SharePoint Online.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение дополнительных свойств из [детальных отчетов об использовании сайтов SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId и unmanagedDevicePolicy.

### <a name="use-sdks"></a>Использование пакетов SDK
Попробуйте предварительный выпуск [пакета SDK Microsoft Graph Java версии 3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! Дополнительные сведения см. в соответствующей [записи блога](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/).

## <a name="january-2021-new-in-preview-only"></a>Январь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Организация трансляций как ресурсов [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). См. [пример](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Получение потока содержимого в виде [отчета об участниках](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [записи](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) или альтернативной записи трансляции.
- Получение статуса [присутствия](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) пользователя, которого [нет на месте](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true), а также любого сообщения, заданного в качестве этого статуса.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Обновление пароля домена Active Directory](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) для успешного [локального сетевого подключения](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Запуск проверок работоспособности локального сетевого подключения](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) теперь может выявлять 5 дополнительных типов ошибок в ресурсе [проверки работоспособности локального подключения](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Дополнительные сведения о типах ошибок см. в [журнале изменений](https://developer.microsoft.com/graph/changelog) за январь 2021 г.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Подписка на уведомления об изменениях облачной печати](universal-print-webhook-notifications.md) — при запуске задания печати и когда принтер готов скачать задание печати.
- Получение более полного диапазона [возможных значений](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values) для состояния [принтера](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true).
- Использование делегированных разрешений в приложениях от имени вошедшего пользователя:
  - `PrinterShare.ReadBasic.All` для чтения основных сведений об общих принтерах, кроме сведений об управлении доступом.
  - `PrintConnector.Read.All` для чтения соединителей печати.
  - `PrintConnector.ReadWrite.All` для чтения и записи соединителей печати.
  - `PrintJob.Create` для создания заданий печати и отправки содержимого в задания печати.
  - `PrintSettings.Read.All` для чтения параметров печати на уровне клиента.
  - `PrintSettings.ReadWrite.All` для чтения или записи параметров печати на уровне клиента.
  - `Reports.Read.All` для чтения сводки об использовании печати для определенного пользователя или принтера.

### <a name="education"></a>Образование
Использование [параметров заданий](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true) на уровне класса, чтобы включить или отключить анимацию для празднования сдачи задания.

### <a name="groups"></a>Группы
Получение состояния обработки динамической группы на основе правил с помощью свойства **membershipRuleProcessingStatus**. Это удобно, когда изменяется атрибут пользователя, участие пользователя в [группе Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) на основе правил подвергается повторной оценке в соответствии с правилами участия в группе, настроенными в организации. 

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Получение [права использования](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true) стороннего программного обеспечения, созданного на основе PowerApps, которым обладает пользователь или устройство, или права использования подписки, которым обладает устройство. Право использования содержит идентификаторы соответствующей службы или продукта и текущее состояние права использования, например "активно", "неактивно", "с предупреждением" или "приостановлено".

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Приложения могут использовать разрешения приложений, чтобы позволить администраторам управлять [способами проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) для пользователей.
- Поддержка [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя для входа или многофакторной проверки подлинности в Azure AD.
- Использование [политики Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true), чтобы определить параметры конфигурации, а также пользователей или группы, которым разрешено применять Microsoft Authenticator в качестве способа проверки подлинности. Использование политики Microsoft Authenticator вместо [политики входа по телефону без пароля с помощью Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), поддержка которой прекращена. 
- Поддержка [Windows Hello для бизнеса](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя при входе на устройствах с Windows без применения пароля.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
- [Получение отчета о количестве зарегистрированных пользователей или пользователей, которым доступны различные функции регистрации](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true), включая многофакторную проверку подлинности, самостоятельный сброс пароля или проверку подлинности без пароля.
- [Получение отчета о количестве пользователей, зарегистрированных для каждого способа проверки подлинности](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true), включая пароль, Windows Hello для бизнеса или вход без пароля с помощью телефона.

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
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
