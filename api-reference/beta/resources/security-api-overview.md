---
title: Использование Microsoft Graph Security API
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7c45ed1f157dbd634eb27fc633deb41ee996f2b6
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855891"
---
# <a name="use-the-microsoft-graph-security-api"></a>Использование Microsoft Graph Security API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph Security API обеспечивает единый интерфейс и схему интеграции с решениями безопасности от корпорации Майкрософт и партнеров экосистемы. Это позволяет клиентам упростить операции, связанные с безопасностью, и лучше защититься от возрастающих киберугроз. Microsoft Graph Security API объединяет запросы для всех подключенных поставщиков безопасности и собирает ответы. Используйте Microsoft Graph Security API для создания приложений с указанными ниже возможностями.

- объединение и корреляция оповещений системы безопасности из нескольких источников;
- разблокировка контекстных данных для получения сведений при расследованиях;
- автоматизация задач безопасности, бизнес-процессов, рабочих процессов и создания отчетов;
- отправка индикаторов угроз в продукты Майкрософт для настроенных обнаружений;
- вызов действий в ответ на новые угрозы;
- обеспечение видимости данных безопасности, чтобы использовать профилактическое управление рисками.

Microsoft Graph Security API включает указанные ниже ключевые объекты.

## <a name="actions-preview"></a>Действия (предварительная версия)

Принимайте незамедлительные действия по защите от угроз с помощью объекта [securityAction](securityaction.md) Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Попробуйте выполнить действия по обеспечению безопасности с помощью [Microsoft Defender для конечной точки](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.

  > **Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.

## <a name="alerts"></a>Оповещения

Оповещения — это потенциальные проблемы безопасности в клиенте пользователя, выявленные решениями по обеспечению безопасности корпорации Майкрософт или партнеров и помеченные для действия или уведомления. С помощью объекта [alerts](alert.md) Microsoft Graph Security можно объединить и оптимизировать управление проблемами безопасности во всех интегрированных решениях. Это также позволит приложениям коррелировать оповещения и контекст для улучшения защиты от угроз и отклика на них. Благодаря функции обновления оповещений можно синхронизировать состояние определенных оповещений в разных продуктах и службах обеспечения безопасности, интегрированных с Microsoft Graph Security API, с помощью обновления объекта [alerts](alert.md).

При использовании Microsoft Graph Security API доступны оповещения от указанных ниже поставщиков. Поддержка для оповещений GET, оповещений PATCH и подписки (с помощью веб-перехватчиков) представлена в приведенной ниже таблице.

| Поставщик безопасности | <p align="center">Оповещение GET</p>| <p align="center">Оповещение PATCH</p>| <p align="center">Подписка на оповещения</p>|
|:------------------|:---------|:-----------|:------------------|
|[Центр безопасности Azure](/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Защита идентификации Azure Active Directory](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) (ранее Microsoft Cloud App Security) | <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender для конечной точки](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) (ранее Microsoft Defender ATP) **| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender для удостоверений](/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) (ранее Azure Advanced Threat Protection) ***| <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [По умолчанию](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>Пользовательское оповещение</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center">Не поддерживается в Azure Sentinel. </p> | <p align="center">&#x2713;</p> |
> **Примечание.** К экосистеме безопасности Microsoft Graph постоянно подключаются новые поставщики. Чтобы запросить новых поставщиков или дополнительную поддержку у существующих поставщиков, [уведомите о проблеме в репозитории GitHub для Microsoft Graph Security](https://github.com/microsoftgraph/security-api-solutions/issues/new).

\* Проблема с файлом: статус оповещения обновляется в интегрированных в API безопасности Microsoft Graph приложениях, но не отображается в интерфейсе управления провайдера.

\*\* Microsoft Defender для конечной точки требует дополнительных [ролей пользователя](/windows/security/threat-protection/microsoft-defender-atp/user-roles) помимо ролей, необходимых для Microsoft Graph Security API. Только пользователи, которым назначены роли как в Microsoft Defender для конечной точки, так и в Microsoft Graph Security API, могут получить доступ к данным Microsoft Defender для конечной точки. Поскольку это ограничение не распространяется на проверку подлинности только для приложений, рекомендуется использовать маркер проверки подлинности только для приложений.

\*\*\* Оповещения Microsoft Defender для удостоверений доступны в рамках интеграции с Microsoft Defender for Cloud Apps. Это означает, что вы будете получать оповещения Microsoft Defender для удостоверений только в том случае, если вы присоединились к комплексному решению SecOps и подключили Microsoft Defender для удостоверений к Microsoft Defender for Cloud Apps. Узнайте больше о том, [как интегрировать Microsoft Defender для удостоверений и Microsoft Defender for Cloud Apps](/azure-advanced-threat-protection/atp-mcas-integration).

## <a name="attack-simulation-and-training-preview"></a>Симуляция атак и обучение (предварительная версия)

[Симуляция атак и обучение](/microsoft-365/security/office-365-security/attack-simulation-training) входит в состав [Microsoft Defender для Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). Эта служба позволяет пользователям в клиенте испытать на себе реалистичную учебную фишинговую атаку и извлечь уроки. Симуляция социотехники и обучение пользователей помогают снизить риск взлома с применением таких методов атаки. API симуляции атак и обучения позволяет администраторам клиентов просматривать запущенные упражнения и тренинги по [симуляции](simulation.md) и получать [отчеты](report-m365defender-reports-overview.md) об аналитике поведения пользователей в Интернете в условиях симуляции фишинга.

## <a name="ediscovery-preview"></a>Обнаружение электронных данных (предварительная версия)

[Обнаружение электронных данных в Microsoft Purview (премиум)](/microsoft-365/compliance/overview-ediscovery-20) обеспечивает комплексный рабочий процесс для сохранения, сбора, анализа, проверки и экспорта содержимого, используемого во внутренних и внешних исследованиях вашей организации.

## <a name="information-protection"></a>Защита информации

**Метки**. Метки защиты информации предоставляют сведения о правильном применении метки конфиденциальности к информации. API метки защиты информации описывает настройку меток конфиденциальности, применяемых к пользователю или клиенту.

**Оценка угроз**. API оценки угроз Microsoft Graph позволяет организациям оценить угрозу, возникшую для любого пользователя в клиенте. Благодаря этому пользователи могут сообщать в корпорацию Майкрософт о полученной нежелательной или подозрительной почте, фишинговых URL-адресах и вредоносных вложениях. Корпорация Майкрософт проверяет соответствующий пример и используемые политики организации перед оформлением результата, чтобы администраторы клиентов могли понять решение о проверке угроз и скорректировать свою политику организации. Они также могут использовать его для создания отчетов о допустимых сообщениях электронной почты, чтобы предотвратить их блокировку.

> **Примечание.** Вместо этого рекомендуется использовать API [отправки информации об угрозах](https://github.com/microsoftgraph/microsoft-graph-docs/pull/16242/files#threat-submission).

## <a name="secure-score"></a>Оценка безопасности

[Оценка безопасности (Майкрософт)](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) — это решение аналитики безопасности, обеспечивающее обзор вашего набора решений безопасности и способов его улучшения. С помощью одной оценки можно лучше понять, что сделано для снижения риска в решениях Майкрософт. Также можно сравнить свою оценку с другими организациями и просмотреть ее изменение со временем. Объекты [secureScore](securescores.md) и [secureScoreControlProfile](securescorecontrolprofiles.md) системы безопасности Microsoft Graph помогают обеспечить баланс между требованиями по безопасности и производительности в организации, позволяя совмещать соответствующие функции безопасности. Вы также можете спрогнозировать значение оцени после внедрения функций безопасности.

## <a name="threat-intelligence-indicators-preview"></a>Индикаторы аналитики угроз (предварительная версия)

Индикаторы угроз, также называемые индикаторами компрометации (IoCs), представляют данные об известных угрозах, таких как вредоносные файлы, URL-адреса, домены и IP-адреса. Пользователи могут создавать индикаторы путем сбора внутренней аналитики угроз или получения индикаторов от сообществ по анализу угроз, лицензированных веб-каналов и других источников. Затем эти индикаторы используются в различных средствах безопасности для защиты от соответствующих угроз.

Объект [tiIndicators](tiindicator.md) Microsoft Graph Security позволяет пользователям направлять свои индикаторы в решения по обеспечению безопасности Майкрософт для включения блокировки и оповещений о вредоносных действиях или их разрешения, что приостанавливает действия для индикаторов, считающихся неважными для организации. При отправке индикаторов указывается как решение корпорации Майкрософт, использующее индикатор, так и выполняемое с индикатором действие.

Можно интегрировать объект [tiIndicator](tiindicator.md) в свое приложение или использовать одну из указанных ниже интегрированных платформ аналитики угроз (TIP):

- [Palo Alto Networks MineMeld Threat Intelligence Sharing](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [Платформа аналитики угроз MISP с открытым кодом](http://www.misp-project.org/), доступная в [примере аналитики угроз](https://aka.ms/tipmispsample)

Индикаторы угроз, отправляемые с помощью Microsoft Graph Security API, в настоящее время доступны в следующих продуктах:

- [Azure Sentinel](/azure/sentinel/overview): позволяет сопоставлять индикаторы угроз с данными журнала, чтобы получать оповещения о вредоносных действиях.
- [Microsoft Defender для конечной точки](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection) — позволяет создавать оповещения и/или блокировать индикаторы угроз, связанные с вредоносными действиями. Вы можете также разрешить индикатору игнорировать автоматические исследования. Подробнее о поддерживаемых типах индикаторов и ограничениях относительно количества индикаторов для каждого клиента см. в статье [Управление индикаторами](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators).

Поддержка в других службах безопасности Майкрософт появится в ближайшее время.

## <a name="threat-submission"></a>Отправка информации об угрозах

API отправки информации об угрозах Microsoft Graph позволяет организациям отправлять сведения об угрозе, возникшей для любого пользователя в клиенте. Благодаря этому пользователи могут сообщать в корпорацию Майкрософт о полученной нежелательной или подозрительной почте, фишинговых URL-адресах и вредоносных вложениях. Корпорация Майкрософт проверяет отправляемый объект в соответствии с действующими политиками организации и отправляет его специалистам по оценке. Результат таких действий поможет администраторам клиента понять решение касательно сканирования угроз и скорректировать политику организации. Администраторы могут также, учитывая результаты, сообщить о допустимых сообщениях электронной почты, чтобы предотвратить их блокировку.

> **Примечание.** Рекомендуется использовать этот API вместо нерекомендуемого API оценки угроз для Information Protection. API отправки информации об угрозах обеспечивает унифицированные возможности отправки сведений об угрозах безопасности, а также единую поддержку результатов, поддержку запросов касательно отправляемых пользователями данных, поддержку списков блокировок и разрешений для клиента, поддержку проверки администратором и поддержку режима только для приложений.

## <a name="common-use-cases"></a>Основные варианты использования

Ниже приводятся некоторые из наиболее популярных запросов для работы с Microsoft Graph Security API.

| **Варианты использования**   | **Ресурсы REST** | **Попробовать в песочнице Graph** |
|:---------------|:--------|:----------|
| **Действия (предварительная версия)**|||
| Получение действия по обеспечению безопасности | [Получение действия по обеспечению безопасности](../api/securityaction-get.md)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление действий по обеспечению безопасности| [Перечисление действий по обеспечению безопасности](../api/securityactions-list.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание действий по обеспечению безопасности|[Создание действий по обеспечению безопасности](../api/securityactions-post.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Отмена действия по обеспечению безопасности|[Отмена действий по обеспечению безопасности](../api/securityaction-cancelsecurityaction.md)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **Оповещения**|||
| Перечисление оповещений | [Перечисление оповещений](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [Обновление оповещения](../api/alert-update.md) </br> [Обновление нескольких оповещений](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **Симуляция атак и обучение (предварительный просмотр)**|||
|Перечисление симуляций|[Перечисление симуляций](../api/attacksimulationroot-list-simulations.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Получение обзорного отчета по симуляции|[Получение обзорного отчета по симуляции](../api/simulationreportoverview-get.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/overview&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Отчет по списку пользователей, участвующих в симуляции|[Отчет по списку пользователей, участвующих в симуляции](../api/usersimulationdetails-list.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/simulationUsers](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/simulationUsers&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Обнаружение электронных данных**|||
|Перечисление случаев обнаружения электронных данных|[Перечисление eDiscoveryCases](../api/security-casesroot-list-ediscoverycases.md)|[https://graph.microsoft.com/beta/security/cases/eDiscoveryCases](https://developer.microsoft.com/graph/graph-explorer?request=security%2Fcases%2FeDiscoverycases&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление операций со случаями обнаружения электронных данных|[Перечисление caseOperations](../api/security-ediscoverycase-list-operations.md)|[https://graph.microsoft.com/beta/security/cases/eDiscoverycases/{id}/operations](https://developer.microsoft.com/graph/graph-explorer?request=security%2Fcases%2FeDiscoverycases%2F%7Bid%7D%2Foperations&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Оценки безопасности**|||
|Список оценок безопасности|[Перечисление объектов secureScores](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Профили составляющих оценки безопасности**|||
|Список профилей составляющих оценки безопасности|[Перечисление объектов secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Обновление профилей составляющих оценки безопасности|[Обновление secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Указания по аналитике угроз (предварительная версия)**|||
|Получение индикатора аналитики угроз|[Получение объекта tiIndicator](../api/tiindicator-get.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление индикаторов аналитики угроз | [Перечисление объектов tiIndicator](../api/tiindicators-list.md) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание индикатора аналитики угроз|[Создание объекта tiIndicator](../api/tiindicators-post.md)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Отправка индикаторов аналитики угроз|[Отправка объектов tiIndicator](../api/tiindicator-submittiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|Обновление индикаторов аналитики угроз|[Обновление объекта tiIndicator](../api/tiindicator-update.md) </br>[Обновление нескольких объектов tiIndicator](../api/tiindicator-updatetiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Удаление индикаторов аналитики угроз|[Удаление объекта tiIndicator](../api/tiindicator-delete.md) </br>[Удаление нескольких объектов tiIndicator](../api/tiindicator-deletetiindicators.md) </br>[Удаление объекта tiIndicator с помощью externalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)| DELETE </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Отправка информации об угрозах**|||
|Получение информации об угрозах, связанных с электронной почтой|[Get emailThreat](../api/security-emailthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Список отправленных сведений об угрозах, связанных с электронной почтой | [List emailThreats](../api/security-emailthreatsubmission-list.md) | [https://graph.microsoft.com/beta/threatSubmission/emailThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/emailThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание отправляемой информации об угрозах, связанных с электронной почтой|[Create emailThreat](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/emailThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Проверка отправленной информации об угрозах, связанных с электронной почтой|[Review emailThreat](../api/security-emailthreatsubmission-review.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/{id}/review](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission//emailThreats/{id}/review&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Получение информации об угрозах, связанных с файлами|[Get fileThreat](../api/security-filethreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/fileThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/urlThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Список отправленных сведений об угрозах, связанных с файлами | [List fileThreats](../api/security-filethreatsubmission-list.md) | [https://graph.microsoft.com/beta/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/fileThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание отправляемой информации об угрозах, связанных с файлами|[Create fileThreat](../api/security-filethreatsubmission-post-fileThreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/fileThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/fileThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Получение информации об угрозах, связанных с URL-адресами|[Get urlThreat](../api/security-urlthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/urlThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/urlThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Список отправленных сведений об угрозах, связанных с URL-адресами | [List urlThreats](../api/security-urlthreatsubmission-list.md) | [https://graph.microsoft.com/beta/security/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/urlThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание отправляемой информации об угрозах, связанных с URL-адресами|[Create urlThreat](../api/security-urlthreatsubmission-post-urlthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/urlThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Получение политики касательно отправляемой информации об угрозах, связанных с электронной почтой|[Get emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Список политик касательно отправляемой информации об угрозах, связанных с электронной почтой | [List emailThreatSubmissionPolicies](../api/security-emailthreatsubmissionpolicy-list.md) | [https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание политики касательно отправляемой информации об угрозах, связанных с электронной почтой|[Create emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies](https://developer.microsoft.com/graph/graph-explorer?request=/security/threatSubmission/emailThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Обновление политики касательно отправляемой информации об угрозах, связанных с электронной почтой|[Update emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|
|Удаление политики касательно отправляемой информации об угрозах, связанных с электронной почтой|[Delete emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-delete.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com)|

Можно использовать [веб-перехватчиков](/graph/webhooks) Microsoft Graph, чтобы подписаться на получение уведомлений об обновлениях объектов Microsoft Graph Security API.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этих наборов API.

## <a name="next-steps"></a>Дальнейшие действия

Microsoft Graph Security API раскрывает новые способы взаимодействия с решениями для обеспечения безопасности, предоставляемыми корпорацией Майкрософт и партнерами. Чтобы приступить к работе, следуйте указанным ниже инструкциям.

- Подробно изучите [оповещения](alert.md), [tiIndicator](tiindicator.md) (предварительная версия), [securityAction](securityaction.md) (предварительная версия), [secureScore](securescores.md) и [secureScoreControlProfiles](securescorecontrolprofiles.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). В разделе **Примеры запросов** выберите элемент **Показать другие примеры** и установите категорию безопасности в положение **Вкл.**
- Попробуйте [подписаться на получение уведомлений](/graph/webhooks) об изменениях объекта.

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).

## <a name="see-also"></a>См. также

[Создавайте код и внесите вклад](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Пример для PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Другие примеры или добавление нового примера](https://aka.ms/graphsecurityapicode)

Ознакомьтесь с другими возможностями подключения с помощью Microsoft Graph Security API:

- [Соединители Microsoft Graph Security для Logic Apps, Flow и Power Apps](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security)
- [Примеры записных книжек Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://techcommunity.microsoft.com/t5/microsoft-graph-security-api/bd-p/SecurityGraphAPI)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)