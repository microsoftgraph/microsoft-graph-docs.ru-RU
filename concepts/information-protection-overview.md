---
title: Обзор меток Microsoft Information Protection
description: Метки Microsoft Information Protection помогают организациям классифицировать, помечать и защищать данные на основе меток конфиденциальности центра безопасности и соответствия требованиям Office 365.
author: tommoser
localization_priority: Normal
ms.prod: microsoft.informationprotection
ms.openlocfilehash: cdbe4b3bdb7bdada33fa8c46c074280abcf6c174
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969831"
---
# <a name="information-protection-overview"></a>Общие сведения о защите информации

Microsoft Information Protection помогает организациям классифицировать, помечать и защищать данные в зависимости от их [конфиденциальности](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels). 

В организациях для удобства используются метки:

* Пользователи в понимании важности обрабатываемых данных.
* Соответствие администраторы при обнаружении конфиденциальной информации. 
* Администраторы безопасности при развертывании политик доступа к данным и защиты от потери данных на основе более обширных сведений о метках.

## <a name="why-integrate-microsoft-information-protection"></a>Зачем нужно интегрировать защиту информации Майкрософт? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Интеграция с общедоступной платформой для маркировки, обслуживание миллионов пользователей и устройств

Более миллиона организаций с десятками миллионов пользователей используют защиту информации Майкрософт для классификации, подписи и защиты данных.  В дополнение к Office 365, различные службы защиты от потери данных (DLP), платформы бизнес-аналитики и программного обеспечения (SaaS) применяют метки [Microsoft Information Protection](https://www.microsoft.com/security/technology/information-protection) для предоставления более подробных возможностей классификации данных. 

### <a name="label-information-in-line-of-business-applications"></a>Сведения о подписи в бизнес-приложениях

Корпоративные разработчики используют Microsoft Information Protection для обозначения и защиты конфиденциальных сведений о клиентах при экспорте из бизнес-приложений, чтобы обеспечить безопасность сведений о клиентах. Подключение приложений к экосистеме Microsoft Information Protection позволяет приложениям применять, обновлять и удалять [метки конфиденциальности](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels) в своих данных приложений без дополнительных издержек при интеграции полного пакета SDK.

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>Что можно делать с помощью API меток защиты информации Майкрософт в Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Обнаружение меток, доступных пользователю или Организации

С помощью Microsoft Graph вы можете получить доступ к [меткам конфиденциальности](/graph/api/informationprotectionlabel?view=graph-rest-beta) , доступным для пользователя или организации. Метки применяются приложениями и службами к данным в REST или в движении, помогая пользователям и подчиненным приложениям и службам определить чувствительность обрабатываемой ими информации.

### <a name="understand-how-to-apply-labels"></a>Сведения о том, как применять метки

Предоставляя сведения о существующей и требуемой метке конфиденциальности, API REST может сообщить приложению о [действиях](/graph/api/resources/informationprotectionaction?view=graph-rest-beta) , которые необходимо выполнить, чтобы правильно применить метку. Сюда входят такие действия, как приложение [метаданных](/graph/api/resources/metadataaction?view=graph-rest-beta) , создание [водяного знака](/graph/api/resources/addwatermarkaction?view=graph-rest-beta) , [Защита](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta)и многое другое.

### <a name="interpret-labels-applied-to-data"></a>Интерпретация меток, примененных к данным

Приложения, использующие сведения, которые уже имеют атрибут [метки чувствительности](/graph/api/resources/metadataaction?view=graph-rest-beta) , могут использовать API **екстрактлабел** для разрешения метаданных метки в [метку чувствительности](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta)к защите информации Майкрософт. Используйте метку, чтобы определить действия, которые должны выполняться приложением при обработке или использовании данных с подписью. 

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API Microsoft Information Protection в бета-версии Microsoft Graph](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и попытайтесь пометить примеровые запросы для защиты информации в [проводнике Graph](https://developer.microsoft.com/graph/graph-explorer). Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **защиту информации Майкрософт**.
