---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах.
author: arpitha-dhanapathi
ms.openlocfilehash: f4e7a29043a55ddefc5a3f5b7fe5a53911d8ee40
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754280"
---
# <a name="national-cloud-deployments"></a>Национальные облачные развертывания

В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти национальные облачные версии — это физические и логически изолированные в сети экземпляры корпоративных облачных служб Майкрософт, которые ограничены географическими границами определенных стран и управляются локальным персоналом.

Существующие национальные облака:

* Microsoft Cloud for US Government
* Microsoft Cloud для Германии
* Azure и Microsoft 365 под управлением 21Vianet в Китае

Каждая из национальных облачных сред уникальна и отличается от глобальной среды Майкрософт. Важно помнить о некоторых из этих ключевых отличий при разработке приложений для национальных облачных сред; Например, регистрация приложений, получение маркеров и вызов API Microsoft Graph могут быть разными.

В этой статье содержится информация о различных национальных облачных развертываниях Microsoft Graph и возможностях, доступных разработчикам в каждом из них.

> **Примечание.** [Подключение к данным Microsoft Graph](./data-connect-concept-overview.md?view=graph-rest-1.0) не поддерживает какие-либо национальные облачные развертывания.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Регистрация приложений и корневые конечные точки службы маркеров

Перед вызовом API Microsoft Graph необходимо зарегистрировать приложение и получить маркер. В следующей таблице перечислены базовые URL-адреса конечных точек Azure Active Directory (Azure AD) для регистрации приложения и получения маркеров для каждого национального облака.

| Национальные облачные технологии | Конечная точка портала Azure AD | Конечная точка Azure AD |
| -------------- | ------------------------ | ----------------- |
| Azure AD (глобальная служба) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD для государственных организаций США | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD для Германии | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Azure AD для Китая под управлением 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Дополнительные информацию о маркерах доступа Azure AD и Microsoft Graph см. [в основах проверки подлинности.](./auth/auth-concepts.md) Для сценариев проверки подлинности Azure AD см. основные принципы проверки [подлинности Azure AD.](/azure/active-directory/develop/authentication-scenarios)

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Корневые конечные точки службы Microsoft Graph и graph Explorer

В следующей таблице показаны корневые конечные точки службы для Microsoft Graph и [обозревателя Graph](https://developer.microsoft.com/graph/graph-explorer) для каждого национального облака.

| Национальное облако | Microsoft Graph | Песочница Graph |
| -------------- | --------------- | -------------- |
| Глобальная служба Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph для правительства США L4 | https://graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для правительства США L5 (DOD) | https://dod-graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для Германии | https://graph.microsoft.de | Не поддерживается. |
| Microsoft Graph для Китая под управлением 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Для приложения в правительства США:
> 
> 
> * Если вы работаете в среде Microsoft 365 GCC, продолжайте использовать конечные точки по всему миру: `https://graph.microsoft.com` и `https://portal.azure.com` .
> * Если вы работаете в среде Microsoft 365 GCC High, используйте: `https://portal.azure.us` и `https://graph.microsoft.us` .
> * Если вы работаете в среде Microsoft 365 DoD, используйте `https://portal.azure.us` и `https://dod-graph.microsoft.us` .
> 
> 
> Доступ к данным правительства США с помощью всемирной конечной точки будет отключен в ближайшее время.

> [!NOTE]
> Приложения могут получать доступ к организационным данным только через конечные точки национального облака. Это означает, что приложения могут получать доступ только к данным в клиентах, зарегистрированных в определенном национальных облаках. Приложения, которые пытаются получить доступ к потребительским данным, связанным с личными учетными записями Майкрософт, через Microsoft Graph, должны использовать глобальную `https://graph.microsoft.com` службу. Маркеры доступа, полученные для развертывания в национальных облаках, не могут быть взаимозаменяемыми с маркерами, полученными для глобальной службы или любого другого национального облака.

## <a name="supported-features"></a>Поддерживаемые функции

Следующие функции Microsoft Graph, как правило, доступны на конечной точке во всех национальных облачных развертываниях, за исключением `/v1.0` отмеченных.

| Функции Microsoft Graph | Microsoft Cloud for US Government | Microsoft Cloud для Китая под управлением 21Vianet | Microsoft Cloud для Германии |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Пользователи | ✔ | ✔ | ✔ |
| Группы | ✔ | ✔ | ✔ |
| Excel | ✔ | ✔\* | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Почта Outlook | ✔ | ✔ | ✔ |
| Календарь Outlook | ✔ | ✔ | ✔ |
| личные контакты; | ✔ | ✔ | ✔ |
| Безопасность | ✔ | ✔ | ✔ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Планировщик | ✔ | ✔ | ✔ |
| Отчеты | ➖ | ✔ | ➖ |
| Контакты организации | ✔ | ➖ | ➖ |
| Приложения | ✔ | ➖ | ➖ |
| Субъекты-службы | ✔ | ➖ | ➖ |
| Уведомления об изменениях (веб-перехватчики) | ✔ | ✔ | ✔\* |
| Разностный запрос | ✔ | ✔ | ➖ |
| Расширения схемы каталога | ✔ | ✔ | ➖ |
| Расширения открытого типа | ✔ | ➖ | ➖ |
| Поиск (Поиск (Майкрософт) | ➖ | ➖ | ➖ |
 
Следующие функции Microsoft Graph доступны в предварительной версии (на конечной точке) в Microsoft Cloud для Китая и Microsoft Cloud в Германии (конечные точки V1.0 для этих функций доступны только в Microsoft Cloud для правительства `/beta` США):

* Контакты организации
* Приложения
* Субъекты-службы

( \* Ограниченная поддержка только служб Exchange и OneDrive. Службы Azure AD не поддерживаются.

> [!IMPORTANT]
> Некоторые службы и функции, которые находятся в определенных регионах глобальной службы, могут быть недоступны во всех национальных облаках. Чтобы узнать, какие службы доступны, см. [продукты, доступные по регионам.](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)

Дополнительные информацию о национальных облаках см. в следующих темах:

* [Национальные облака Майкрософт](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 для правительства США](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 под управлением 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure для государственных органов](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure для Китая 21Vianet](/azure/china/)
* [Azure для Германии](/azure/germany/)