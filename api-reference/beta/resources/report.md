---
title: Работа с отчетами об использовании Microsoft 365 в Microsoft Graph
description: Microsoft Graph позволяет получить доступ к отчетам об использовании Microsoft 365 и узнать, как сотрудники компании используют службы Microsoft 365. Например, можно выяснить, кто слишком активно использует службы и практически выбрал квоты, а кому лицензия Microsoft 365, возможно, и вовсе не нужна.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ed1f58f3243a0abc433b2407f61d04077469f896
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133694"
---
# <a name="working-with-microsoft-365-usage-reports-in-microsoft-graph"></a>Работа с отчетами об использовании Microsoft 365 в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет получить доступ к отчетам об использовании Microsoft 365 и узнать, как сотрудники компании используют службы Microsoft 365. Например, можно выяснить, кто слишком активно использует службы и практически выбрал квоты, а кому лицензия Microsoft 365, возможно, и вовсе не нужна. 

Сведения о параметрах, регулирующих идентификацию и деидентификацию информации в данных отчетов об использовании Microsoft 365, см. в статье [Отчеты по Microsoft 365 в Центре администрирования](/microsoft-365/admin/activity-reports/activity-reports).

## <a name="authorization"></a>Авторизация

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Укажите разрешения, необходимые для доступа к отчетам, на портале Azure Active Directory (Azure AD). Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для отчетов](/graph/permissions-reference#reports-permissions).

## <a name="cloud-deployments"></a>Облачные развертывания

В следующей таблице показана доступность для каждого API во всех облачных развертываниях.

| Интерфейсы API                                                         | Глобальная служба Microsoft Graph | **Microsoft Cloud for US Government** | **Microsoft Cloud China под управлением 21Vianet** | **Microsoft Cloud для Германии** |
| ------------------------------------------------------------ | ------------------------------ | ------------------------------------- | ---------------------------------------------- | --------------------------- |
| [Активации Microsoft 365](/graph/api/resources/office-365-activations-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Активные пользователи Microsoft 365](/graph/api/resources/office-365-active-users-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Использование приложений Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Использование браузера Microsoft 365](/graph/api/resources/microsoft-365-browser-usage-report?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Действия в группах Microsoft 365](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Использование устройств Microsoft Teams](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Использование команды Microsoft Teams](/graph/api/resources/microsoft-teams-team-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Действия пользователей Microsoft Teams](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ➖                                              | ➖                           |
| [Действия в Outlook](/graph/api/resources/email-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Использование приложения Outlook](/graph/api/resources/email-app-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Использование почтового ящика Outlook](/graph/api/resources/mailbox-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Действия в OneDrive](/graph/api/resources/onedrive-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Использование OneDrive](/graph/api/resources/onedrive-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Действия в SharePoint](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Использование сайтов SharePoint](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ✔                                     | ✔                                              | ➖                           |
| [Действия в Skype для бизнеса](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Использование устройств со Skype для бизнеса](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Действия организаторов в Skype для бизнеса](/graph/api/resources/skype-for-business-organizer-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Действия участников в Skype для бизнеса](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Одноранговые действия в Skype для бизнеса](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ✔                                              | ➖                           |
| [Действия в Yammer](/graph/api/resources/yammer-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Использование устройств в Yammer](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Действия в группах Yammer](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-beta&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).


