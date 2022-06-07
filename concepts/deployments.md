---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах.
author: arpitha-dhanapathi
ms.localizationpriority: medium
ms.openlocfilehash: 06f3b34d8a1f41116f2e8e719ff81939f4999ecd
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924081"
---
# <a name="national-cloud-deployments"></a>Национальные облачные развертывания

В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти версии национального облака — это физические и логически изолированные от сети экземпляры корпоративных облачных служб Майкрософт, которые ограничены географическими границами определенных стран и обслуживаются локальным персоналом.

Существующие национальные облака:

* Microsoft Cloud for US Government
* Microsoft Cloud для Германии
* Azure и Microsoft 365, предоставляемые 21Vianet в Китае

Каждая из национальных облачных сред уникальна и отличается от глобальной среды Майкрософт. При разработке приложений для национальных облачных сред важно учитывать некоторые из этих ключевых различий. Например, регистрация приложений, получение маркеров и вызов API Microsoft Graph могут отличаться.

В этой статье содержатся сведения о различных национальных облачных развертываниях Microsoft Graph и возможностях, доступных разработчикам в каждом из них.

> **Примечание.** [Microsoft Graph Data Connect](./data-connect-concept-overview.md) не поддерживает развертывание в национальных облаках.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Регистрация приложений и корневые конечные точки службы маркеров

Перед вызовом API Microsoft Graph необходимо сначала зарегистрировать приложение и получить маркер. В следующей таблице перечислены базовые URL-адреса конечных точек Azure Active Directory (Azure AD) для регистрации приложения и получения маркеров для каждого национального облака.

| Национальное облако | Конечная точка портала Azure AD | Конечная точка Azure AD |
| -------------- | ------------------------ | ----------------- |
| Azure AD (глобальная служба) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD для государственных организаций США | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD для Германии | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Azure AD для Китая под управлением 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Дополнительные сведения о маркерах доступа и Microsoft Graph см. в [статьях об основах проверки подлинности](./auth/auth-concepts.md). Сведения о сценариях проверки подлинности Azure AD см. в статье "Основные сведения о проверке [подлинности Azure AD"](/azure/active-directory/develop/authentication-scenarios).

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Корневые конечные точки службы Microsoft Graph и песочниц Graph

В следующей таблице показаны корневые конечные точки службы для Microsoft Graph и [graph Explorer](https://developer.microsoft.com/graph/graph-explorer) для каждого национального облака.

| Национальное облако | Microsoft Graph | Песочница Graph |
| -------------- | --------------- | -------------- |
| Глобальная служба Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph для государственных организаций США L4 | https://graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для государственных организаций США L5 (DOD) | https://dod-graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для Германии | https://graph.microsoft.de | Не поддерживается. |
| Microsoft Graph для Китая под управлением 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Для приложения в государственных организаций США:
>
> * Если вы работаете в среде Microsoft 365 GCC, продолжайте использовать конечные точки по всему миру: `https://graph.microsoft.com` и `https://portal.azure.com`.
> * Если вы работаете в среде Microsoft 365 GCC High, используйте и `https://portal.azure.us` `https://graph.microsoft.us`.
> * Если вы работаете в среде Microsoft 365 DoD, используйте и `https://portal.azure.us` `https://dod-graph.microsoft.us`.

> [!NOTE]
> Приложения могут получать доступ к данным организации только через конечные точки национального облака. Это означает, что приложения могут получать доступ к данным только в клиентах, зарегистрированных в определенном национальном облаке. Приложения, которые пытаются получить доступ к данным потребителя, связанным с личными учетными записями Майкрософт, через Microsoft Graph, должны использовать глобальную службу `https://graph.microsoft.com`. Маркеры доступа, полученные для развертывания в национальных облаках, не являются взаимозаменяемыми с маркерами, полученными для глобальной службы или любого другого национального облака.

## <a name="supported-features"></a>Поддерживаемые функции

Следующие функции Microsoft Graph `/v1.0` общедоступны для конечной точки во всех национальных облачных развертываниях, за исключением указанных случаев.

| Функции Microsoft Graph | Microsoft Cloud for US Government | Microsoft Cloud China под управлением 21Vianet | Microsoft Cloud для Германии |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Проверки доступа | ✔ | ✔ | ➖ |
| Приложения | ✔ | ➖ | ➖ |
| Уведомления об изменениях (веб-перехватчики) | ✔ | ✔ | ✔\* |
| Разностный запрос | ✔ | ✔ | ➖ |
| Расширения схемы каталога | ✔ | ✔ | ➖ |
| Excel | ✔ | ➖ | ✔ |
| Группы | ✔ | ✔ | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Расширения открытого типа | ✔ | ➖ | ➖ |
| Контакты организации | ✔ | ➖ | ➖ |
| Календарь Outlook | ✔ | ✔ | ✔ |
| Почта Outlook | ✔ | ✔ | ✔ |
| личные контакты; | ✔ | ✔ | ✔ |
| управление привилегированными пользователями (PIM); | ✔ | ✔ | ➖ |
| Планировщик | ✔ | ✔ | ✔ |
| Отчеты | ➖ | ➖ | ➖ |
| Поиск (Поиск (Майкрософт) | ✔ | ➖ | ➖ |
| Безопасность | ✔ | ✔ | ✔ |
| Работоспособность и взаимодействие служб | ✔ | ✔ | ✔ |
| Субъекты-службы | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Пользователи | ✔ | ✔ | ✔ |

Следующие функции Microsoft Graph доступны в предварительной версии ( `/beta` в конечной точке) в Microsoft Cloud для Китая и Microsoft Cloud в Германии (конечные точки версии 1.0 для этих функций доступны только в Microsoft Cloud для государственных организаций США):

* Контакты организации
* Приложения
* Субъекты-службы

(\*) Ограниченная поддержка только служб Exchange и OneDrive. Службы Azure AD не поддерживаются.

> [!IMPORTANT]
> Некоторые службы и компоненты, которые находятся в определенных регионах глобальной службы, могут быть доступны не во всех национальных облаках. Чтобы узнать, какие службы доступны, ознакомьтесь с [продуктами, доступными по регионам](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).

Дополнительные сведения о национальных облаках см. в следующих разделах:

* [Национальные облака Майкрософт](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 для государственных организаций США](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 под управлением 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure для государственных организаций](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure для Китая (21Vianet)](/azure/china/)
* [Azure для Германии](/azure/germany/)

Изучите примеры проверки подлинности и работы с Azure и Microsoft 365 в национальных облачных развертываниях:

* [Работа с Azure с помощью Microsoft Graph для государственных организаций США](https://github.com/SteveWinward/Azure-Samples/blob/master/AAD/SampleAadToken_AzureForGovernment.ps1)
* [Подключение к средам Office 365 для государственных организаций США (GCC, GCC High и GCC DoD) с помощью Microsoft Graph PowerShell](https://github.com/microsoft/Federal-Business-Applications/tree/main/demos/powershell-gov-samples#microsoft-graph-powershell)

