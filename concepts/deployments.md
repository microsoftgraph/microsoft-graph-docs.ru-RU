---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти национальные облачные версии являются физическими и логически изолированными от сети экземплярами корпоративных облачных служб Майкрософт, которые ограничены в пределах географических границ конкретных стран и обслуживаются местным персоналом.
ms.openlocfilehash: a32d8bde766718aa0f6f6080ed4b8ff4e3e7f520
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526308"
---
# <a name="national-cloud-deployments"></a>Национальные облачные развертывания

В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти национальные облачные версии являются физическими и логически изолированными от сети экземплярами корпоративных облачных служб Майкрософт, которые ограничены в пределах географических границ конкретных стран и обслуживаются местным персоналом.

Существующие национальные облака:

- Microsoft Cloud for US Government
- Microsoft Cloud для Германии
- Службы Azure и Office 365 под управлением компании 21Vianet в Китае

Каждая национальная облачная среда уникальна и отличается от глобальной среды Майкрософт. При разработке приложений для национальных облачных сред важно помнить о некоторых из этих ключевых отличий. Например, регистрация приложений, получение маркеров и вызов API Microsoft Graph могут отличаться.

В этой статье приводятся сведения о различных облачных развертываниях Microsoft Graph и возможностях, доступных разработчикам в различных средах.

## <a name="app-registration-and-token-service-root-endpoints"></a>Конечные точки регистрации приложений и корневых конечных точек службы маркеров

Перед вызовом API Microsoft Graph необходимо сначала зарегистрировать приложение и получить маркер. В следующей таблице перечислены базовые URL-адреса для конечных точек Azure Active Directory (Azure AD) для регистрации приложения и получения маркеров для каждого национального облака.

| Национальный облако | Конечная точка портала Azure AD| Конечная точка Azure AD|
|---------------------------|----------------|----------------|
|Azure AD для государственных организаций США |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD для Германии |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|Azure AD для Китая под управлением 21Vianet |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD (глобальная служба)|https://portal.azure.com |`https://login.microsoftonline.com`|

Дополнительные сведения о маркерах доступа Azure AD и Microsoft Graph приведены в разделе [получение маркеров проверки](./auth-overview.md)подлинности. Сведения о сценариях проверки подлинности Azure AD см. [](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios)

> **Примечание.** [Конечные точки авторизации и маркеров Azure AD версии 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) доступны только в глобальной службе и не могут использоваться с национальными облачными развертываниями.


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Корневые конечные точки службы Microsoft Graph и проводника Graph

В следующей таблице показаны корневые конечные точки службы для Microsoft Graph и [проводника Graph](https://developer.microsoft.com/graph/graph-explorer) для каждого национального облака.

| Национальное облако | Microsoft Graph | Песочница Graph |
|---------------------------|----------------|----------------|
| Microsoft Graph для государственных организаций (США), 4 | https://graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для государственных учреждений (США), на английском (DOD) | https://dod-graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для Германии | https://graph.microsoft.de | Не поддерживается. |
| Microsoft Graph для Китая под управлением 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Глобальная служба Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

>**Важно!** Если у вас уже есть приложение в государственных странах США и вы используете конечную точку `https://graph.microsoft.com`, рекомендуем переключиться на новую `https://graph.microsoft.us` конечную точку. Доступ к данным правительства США с помощью Всемирной конечной точки в настоящее время функционирует, но в ближайшем будущем будет отключен.

> **Примечание.** Приложения могут получать доступ к данным организации только через конечные точки национальных облачных служб. Это означает, что приложения могут получать доступ только к данным в клиентах, зарегистрированных в конкретном национальном облаке. Приложения, пытающиеся получить доступ к данным пользователей, связанным с личными учетными записями Майкрософт через `https://graph.microsoft.com`Microsoft Graph, должны использовать глобальную службу. Маркеры доступа, полученные для национального облачного развертывания, не являются взаимозаменяемыми с данными, приобретенными для глобальной службы или любого другого национального облака.

## <a name="supported-features"></a>Поддерживаемые функции

Следующие функции Microsoft Graph, как правило, доступны в `/v1.0` конечной точке во всех национальных облачных развертываниях, за исключением оговоренных случаев.

| Функции Microsoft Graph | Microsoft Cloud for US Government | Microsoft Cloud Китая под управлением 21Vianet | Microsoft Cloud для Германии |
|---------------------------|----------------|----------------|----------------|
| Пользователи | ✔ | ✔ | ✔ |
| Группы | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Почта Outlook | ✔ | ✔ | ✔ |
| Календарь Outlook | ✔ | ✔ | ✔ |
| личные контакты; | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔ | ✔ |
| Планировщик|✔ |✔ |✔ |
| Отчеты  |➖| ✔ |➖|
| Уведомления об изменениях (веб-перехватчики)  | ➖|✔* |✔* |
| Запрос на получение различий | ➖ | ➖| ➖ |
| Расширения схемы каталога |➖|➖|➖|
| Расширения открытого типа|➖|➖|➖|
  
Следующие дополнительные функции Microsoft Graph доступны в предварительной версии (в `/beta` конечной точке) во всех национальных облачных развертываниях, за исключением тех случаев, когда они отмечены:

* Контакты организации
* Приложения
* Субъекты-службы
* Уведомления об изменениях (веб-перехватчики)

(*) Ограниченная поддержка только для служб Exchange и OneDrive. Службы Azure AD не поддерживаются. 

 > **Важно!** Некоторые службы и функции, которые находятся в определенных регионах глобальной службы, могут быть недоступны во всех национальных облаках. Чтобы узнать, какие службы доступны, ознакомьтесь со статьей [продукты, доступные по регионам](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).


Дополнительные сведения о национальных облаках приведены в следующих разделах:
- [Национальные облака Майкрософт](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 для государственных организаций США](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Служба Office 365, предоставляемая компанией 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Germany](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Правительственные учреждения Azure](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure Китая 21Vianet](https://docs.microsoft.com/azure/china/)
- [Azure Германия](https://docs.microsoft.com/azure/germany/)
