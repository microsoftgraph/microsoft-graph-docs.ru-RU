---
title: Общие сведения о метках Microsoft Purview Information Protection
description: Метки Microsoft Purview Information Protection помогают организациям классифицировать, помечайте и защищайте данные на основе меток конфиденциальности Центра безопасности и соответствия требованиям Office 365.
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: e2f93def1a27e3a19866319650122ba6d4fca09b
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884234"
---
# <a name="information-protection-overview"></a>Обзор Information Protection

Microsoft Purview Information Protection помогает организациям классифицировать, помечайте и защищайте данные на основе [конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels). 

Организации используют метки для оказания помощи:

* Пользователи, которые понимают важность обрабатываемой информации.
* Администраторы соответствия требованиям при обнаружении местонахождения конфиденциальной информации. 
* Администраторы безопасности при развертывании политик доступа к данным и защиты от потери данных на основе более подробных сведений о метках.

## <a name="why-integrate-microsoft-purview-information-protection"></a>Зачем интегрировать Microsoft Purview Information Protection? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Интеграция с универсальной платформой маркировки, которая обслуживает миллионы пользователей и устройств

Более миллиона организаций с десятками миллионов пользователей используют Microsoft Purview Information Protection для классификации, маркировки и защиты данных.  Помимо Microsoft 365, различные службы защиты от потери данных (DLP), платформы бизнес-аналитики и решения SaaS (программное обеспечение как услуга) имеют метки [Microsoft Purview Information Protection](https://www.microsoft.com/security/technology/information-protection) , чтобы обеспечить более широкие возможности классификации данных. 

### <a name="label-information-in-line-of-business-applications"></a>Сведения о метках в бизнес-приложениях

Корпоративные разработчики используют Microsoft Purview Information Protection для пометки и защиты конфиденциальной информации клиента при экспорте из бизнес-приложений, чтобы обеспечить безопасность сведений о клиентах. Подключение приложений к экосистеме Microsoft Purview Information Protection позволяет приложениям применять, обновлять и удалять метки конфиденциальности в собственных [](/Office365/SecurityCompliance/sensitivity-labels) данных приложения без дополнительных затрат на интеграцию полного пакета SDK.

## <a name="what-can-i-do-with-microsoft-purview-information-protection-label-apis-in-microsoft-graph"></a>Что можно сделать с помощью API меток Microsoft Purview Information Protection в Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Обнаружение меток, доступных пользователю или организации

С помощью Microsoft Graph вы можете получить доступ к [метках](/graph/api/resources/informationprotectionlabel) конфиденциальности, доступным пользователю или организации. Метки применяются приложениями и службами к неактивным или неактивным данным, помогая пользователям и подчиненным приложениям и службам понять конфиденциальность обрабатываемой информации.

### <a name="understand-how-to-apply-labels"></a>Общие сведения о применении меток

Предоставляя сведения о существующей и требуемой метке конфиденциальности, REST API может интеллектуально информировать приложение о действиях, [](/graph/api/resources/informationprotectionaction) которые необходимо предпринять для правильного применения метки. К ним относятся такие действия, как приложение [метаданных](/graph/api/resources/metadataaction) , создание [водяного](/graph/api/resources/addwatermarkaction) знака, [защита](/graph/api/resources/protectbytemplateaction) и т. д.

### <a name="interpret-labels-applied-to-data"></a>Интерпретация меток, примененных к данным

Приложения, использующие информацию, к [](/graph/api/resources/metadataaction) которой уже применены метаданные метки конфиденциальности, могут использовать API **extractLabel** для разрешения метаданных метки в метку конфиденциальности Microsoft Purview [Information Protection.](/graph/api/resources/informationprotectionlabel) Используйте метку, чтобы определить действия, которые должны выполняться приложением при обработке или использовании помеченных данных. 

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API Microsoft Purview Information Protection в бета-версии Microsoft Graph](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и попробуйте использовать примеры запросов меток Information Protection в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **Microsoft Purview Information Protection**.
