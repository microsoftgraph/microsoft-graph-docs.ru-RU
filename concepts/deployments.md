---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти версии национальный облаке, физической и логической изолированной экземпляры Microsoft enterprise облачных служб, которые находятся в границах географическое границы конкретных стран и обслуживается локальной персонала.
ms.openlocfilehash: a5f5c5d0ae8611957cb9087de53f5ddd87d1f25d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571298"
---
# <a name="national-cloud-deployments"></a>Национальные облачные развертывания

В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти версии национальный облаке, физической и логической изолированной экземпляры Microsoft enterprise облачных служб, которые находятся в границах географическое границы конкретных стран и обслуживается локальной персонала.

Существующие национальные облака:

- Microsoft Cloud for US Government
- Microsoft Cloud для Германии
- Службы Azure и Office 365 под управлением компании 21Vianet в Китае

Каждый национальный облачной среде — это уникальное и отличается от глобальной среды Microsoft. Важно иметь в виду некоторые из этих ключевых различий при разработке приложений для Национальный облачных средах; Например, для регистрации приложений, приобретение маркеры и вызов Microsoft Graph API может отличаться.

В этой статье сведения о различных развертываниях национальный облако Microsoft Graph и возможностей, доступных разработчикам в каждой.

## <a name="app-registration-and-token-service-root-endpoints"></a>Приложение регистрации и маркер корневой конечных точек службы

Прежде чем вызывать API-интерфейсы Microsoft Graph, следует регистрировать приложение и получить маркер. В следующей таблице приведены базовый URL-адресов для конечных точек Azure Active Directory (Azure AD) и зарегистрировать приложение маркеры для каждой страны облака.

| Национальный облако | Портала конечной Azure AD| Конечная точка Azure AD|
|---------------------------|----------------|----------------|
|Azure AD для государственных организаций США |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD для Германии |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|Azure AD для Китая под управлением 21Vianet |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD (глобальная служба)|https://portal.azure.com |`https://login.microsoftonline.com`|

Чтобы узнать больше о Azure AD доступа, маркеры и Microsoft Graph, обратитесь к разделу [получить проверкой подлинности на основе маркеров](./auth-overview.md). Сценарии проверки подлинности Azure AD в разделе [основы проверки подлинности Azure AD](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).

> **Примечание.** [Конечные точки авторизации и маркеров Azure AD версии 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) доступны только в глобальной службе и не могут использоваться с национальными облачными развертываниями.


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph и графическое представление проводника корневого конечных точек службы

В следующей таблице показаны корневой конечных точек службы Microsoft Graph и [Explorer график](https://developer.microsoft.com/graph/graph-explorer) для каждой страны облака.

| Национальное облако | Microsoft Graph | Песочница Graph |
|---------------------------|----------------|----------------|
| Microsoft Graph для государственных организаций США | https://graph.microsoft.us | Не поддерживается. |
| Microsoft Graph для Германии | https://graph.microsoft.de | Не поддерживается. |
| Microsoft Graph для Китая под управлением 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Глобальная служба Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **Примечание.** Приложения могут получать доступ к данным организации только через конечные точки национальных облачных служб. Это означает, что приложения можно только доступа к данным в клиенты, зарегистрированные в конкретных национальный облака. Приложения, которые пытается получить данные получателя, связанные с личных учетных записей Майкрософт с помощью Microsoft Graph, следует использовать глобальной службы `https://graph.microsoft.com`. Маркеры доступа, полученные для развертывания национальный облака не являются взаимозаменяемыми с учетными записями приобретено для глобальной службы или других национальный облака.

## <a name="supported-features"></a>Поддерживаемые функции

Microsoft Graph доступны следующие функции обычно на `/v1.0` конечной точки для всех развертываний национальный облаке, за исключением отмеченных.

| Компоненты Microsoft Graph | Microsoft Cloud for US Government | Обслуживается 21Vianet Китая облаке Майкрософт | Microsoft Cloud для Германии |
|---------------------------|----------------|----------------|----------------|
| Пользователи | ✔ | ✔ | ✔ |
| Группы | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Почта | ✔ | ✔ | ✔ |
| Календарь Outlook | ✔ | ✔ | ✔ |
| Личные контакты | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔* | ✔ |
| Запрос на получение различий | ✔ | ✔ | ✔ |
| Веб-перехватчики  | ✔ | ✔ | ✔ |
| Отчеты  |➖| ✔ |➖|
| Планировщик (Майкрософт)|➖|➖|➖|
|Расширения схемы каталога |➖|➖|➖|
| Расширения открытого типа|➖|➖|➖|
  
Доступны следующие дополнительные возможности Microsoft Graph в предварительной версии (на `/beta` конечной точки) на всех развертываний национальный облаке, за исключением отмеченных:

* Контакты организации
* Приложения
* Субъекты-службы

(*) Ограниченная поддержка API в этом облака.

 > **Важно:** Некоторых служб и компонентов, которые находятся в отдельных областей глобальной службы не становятся доступны во всех национальный облака. Чтобы узнать, какие службы доступны, обратитесь [продуктов, доступных по регионам](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).


Чтобы узнать больше о национальный облака в следующих разделах:
- [Национальный Microsoft облака](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 для государственных учреждений США.](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Office 365, которой с 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Германия](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure государственных организаций](https://azure.microsoft.com/global-infrastructure/government/)
- [21Vianet в Китае Azure](https://docs.microsoft.com/azure/china/)
- [Azure Германия](https://docs.microsoft.com/azure/germany/)
