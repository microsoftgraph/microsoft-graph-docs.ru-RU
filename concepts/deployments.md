---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах.
author: arpitha-dhanapathi
ms.localizationpriority: medium
ms.openlocfilehash: 9ec835a37863ee2bb39fed65d2c4748d0f797bef
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137422"
---
# <a name="national-cloud-deployments"></a>Национальные облачные развертывания

В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти национальные облачные версии являются физическими и логически изолированными сетевыми экземплярами корпоративных облачных служб Майкрософт, которые ограничены географическими границами определенных стран и управляются местным персоналом.

Существующие национальные облака:

* Microsoft Cloud for US Government
* Microsoft Cloud для Германии
* Azure и Microsoft 365 21Vianet в Китае

Каждая национальная облачная среда уникальна и отличается от глобальной среды Майкрософт. Важно помнить о некоторых из этих ключевых различий при разработке приложений для национальных облачных сред; например, регистрация приложений, приобретение маркеров и вызов API microsoft Graph может быть другим.

В этой статье данная статья содержит сведения о различных развертываниях Graph microsoft и возможностях, доступных разработчикам в каждом из них.

> **Примечание.** [Подключение к данным Microsoft Graph](./data-connect-concept-overview.md) не поддерживает ни один из национальных облачных развертывание.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Корневые точки регистрации приложений и службы маркеров

Прежде чем вызывать API Graph Microsoft, сначала необходимо зарегистрировать приложение и приобрести маркер. В следующей таблице перечислены базовые URL-адреса для конечных точек Azure Active Directory Azure AD для регистрации приложения и приобретения маркеров для каждого национального облака.

| Национальное облако | Конечная точка портала Azure AD | Конечная точка Azure AD |
| -------------- | ------------------------ | ----------------- |
| Azure AD (глобальная служба) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD для государственных организаций США | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD для Германии | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Azure AD для Китая под управлением 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Дополнительные новости о маркерах доступа Azure AD и microsoft Graph см. в основных документах [проверки подлинности.](./auth/auth-concepts.md) В сценариях проверки подлинности Azure AD см. основные принципы проверки [подлинности Azure AD.](/azure/active-directory/develop/authentication-scenarios)

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Корневые точки службы Graph и Graph Explorer

В следующей таблице показаны корневые точки службы microsoft Graph [и Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) для каждого национального облака.

| Национальное облако | Microsoft Graph | Песочница Graph |
| -------------- | --------------- | -------------- |
| Глобальная служба Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph для правительства США L4 | https://graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для правительства США L5 (DoD) | https://dod-graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для Германии | https://graph.microsoft.de | Не поддерживается. |
| Microsoft Graph для Китая под управлением 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Для приложения в правительстве США:
>
>
> * Если вы работаете в Microsoft 365 GCC среде, продолжайте использовать конечные точки по всему миру: `https://graph.microsoft.com` и `https://portal.azure.com` .
> * Если вы работаете в среде Microsoft 365 GCC, используйте: `https://portal.azure.us` и `https://graph.microsoft.us` .
> * Если вы работаете в среде Microsoft 365 DoD, используйте `https://portal.azure.us` и `https://dod-graph.microsoft.us` .
>
>
> Доступ к данным правительства США с помощью конечной точки по всему миру будет отключен в ближайшем будущем.

> [!NOTE]
> Приложения могут получать доступ к организационным данным только через национальные конечные точки облака. Это означает, что приложения могут получать доступ к данным только в клиентах, зарегистрированных в определенном национальном облаке. Приложения, которые пытаются получить доступ к потребительским данным, связанным с личными учетными записями Майкрософт Graph Microsoft, должны использовать глобальную `https://graph.microsoft.com` службу. Маркеры доступа, приобретенные для развертывания национальных облаков, не являются взаимозаменяемыми с маркерами, приобретенными для глобальной службы или любого другого национального облака.

## <a name="supported-features"></a>Поддерживаемые функции

Следующие функции Microsoft Graph доступны в конечной точке во всех национальных облачных развертываниях, за исключением `/v1.0` отмеченных.

| Функции Graph Microsoft | Microsoft Cloud for US Government | Microsoft Cloud China управляется 21Vianet | Microsoft Cloud для Германии |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Приложения | ✔ | ➖ | ➖ |
| Уведомления об изменениях (веб-перехватчики) | ✔ | ✔ | ✔\* |
| Разностный запрос | ✔ | ✔ | ➖ |
| Расширения схемы каталога | ✔ | ✔ | ➖ |
| Excel | ✔ | ✔\* | ✔ |
| Группы | ✔ | ✔ | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Расширения открытого типа | ✔ | ➖ | ➖ |
| Контакты организации | ✔ | ➖ | ➖ |
| Календарь Outlook | ✔ | ✔ | ✔ |
| Почта Outlook | ✔ | ✔ | ✔ |
| личные контакты; | ✔ | ✔ | ✔ |
| Планировщик | ✔ | ✔ | ✔ |
| Отчеты | ➖ | ✔ | ➖ |
| Поиск (Поиск (Майкрософт)) | ➖ | ➖ | ➖ |
| Безопасность | ✔ | ✔ | ✔ |
| Работоспособность и взаимодействие служб | ✔ | ✔ | ✔ |
| Субъекты-службы | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Пользователи | ✔ | ✔ | ✔ |

Следующие функции Microsoft Graph доступны в предварительном просмотре (на конечной точке) в Microsoft Cloud China и Microsoft Cloud Germany (конечные точки V1.0 для этих функций доступны только в `/beta` Microsoft Cloud for US Government):

* Контакты организации
* Приложения
* Субъекты-службы

( \* Ограниченная поддержка только Exchange и OneDrive служб. Службы Azure AD не поддерживаются.

> [!IMPORTANT]
> Некоторые службы и функции, которые находятся в определенных регионах глобальной службы, могут быть недоступны во всех национальных облаках. Чтобы узнать, какие службы доступны, см. [в сайте продукты, доступные по регионам.](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)

Дополнительные информацию о национальных облаках см. в следующих разделах:

* [Microsoft National Clouds](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 для правительства США](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure Government](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure China 21Vianet](/azure/china/)
* [Azure для Германии](/azure/germany/)
