---
title: Microsoft Information Protection метки
description: 'Microsoft Information Protection помогает организациям классифицировать, маркировать и защищать данные на основе Office 365 меток безопасности и соответствия требованиям.'
author: tommoser
ms.localizationpriority: medium
ms.prod: security
---

# <a name="information-protection-overview"></a>Обзор защиты информации

Microsoft Information Protection помогает организациям классифицировать, маркировать и защищать данные на основе [конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels). 

Организации используют метки для оказания помощи:

* Пользователи понимают важность обрабатываемой информации.
* Администраторы соответствия требованиям при обнаружении мест, где живут конфиденциальные сведения. 
* Администраторы безопасности при развертывании политик защиты от потери данных и доступа к данным на основе более богатых сведений об меток.

## <a name="why-integrate-microsoft-information-protection"></a>Зачем интегрировать Microsoft Information Protection? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Интеграция с платформой повсеместной маркировки, обслуживающей миллионы пользователей и устройств

Более миллиона организаций с десятками миллионов пользователей используют Microsoft Information Protection для классификации, метки и защиты данных.  Помимо Microsoft 365, различные службы по предотвращению потери данных(DLP), платформы бизнес-аналитики и решения для программного обеспечения как-службы (SaaS) приняли Microsoft Information Protection [](https://www.microsoft.com/security/technology/information-protection) метки, чтобы обеспечить более богатый опыт классификации данных. 

### <a name="label-information-in-line-of-business-applications"></a>Сведения о метки в бизнес-приложениях

Enterprise разработчики используют Microsoft Information Protection для маркировки и защиты конфиденциальной информации о клиентах при экспорте из бизнес-приложений для обеспечения безопасности сведений о клиентах. Подключение приложений к экосистеме Microsoft Information Protection позволяет приложениям применять, обновлять и удалять метки конфиденциальности в собственных данных приложений без [](/Office365/SecurityCompliance/sensitivity-labels) накладных расходов на интеграцию полного SDK.

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>Что можно сделать с API Microsoft Information Protection меток в Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Обнаружение меток, доступных пользователю или организации

С помощью microsoft Graph вы можете получить доступ к метки конфиденциальности, доступные пользователю или организации.[](/graph/api/resources/informationprotectionlabel) Метки применяются приложениями и службами к данным в режиме покоя или в движении, помогая пользователям и приложениям и службам ниже по течению понимать чувствительность обработки данных.

### <a name="understand-how-to-apply-labels"></a>Понимание применения меток

Предоставляя сведения о существующей и необходимой мете конфиденциальности, API REST может разумно информировать ваше приложение о действиях, [](/graph/api/resources/informationprotectionaction) которые необходимо принять для правильного применения метки. Это включает такие действия, как [приложение метаданных](/graph/api/resources/metadataaction)[,](/graph/api/resources/addwatermarkaction) генерация водяных знаков, [защита](/graph/api/resources/protectbytemplateaction) и другие.

### <a name="interpret-labels-applied-to-data"></a>Интерпретация меток, применяемых к данным

Приложения, потребляющие информацию, уже применяемую метаданные метки чувствительности, могут использовать API **extractLabel** для решения метаданных меток на метку Microsoft Information Protection [чувствительности](/graph/api/resources/informationprotectionlabel).[](/graph/api/resources/metadataaction) Используйте метку, чтобы определить действия, которые должно принимать приложение при обработке или потреблении помеченных данных. 

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Microsoft Information Protection API в бета Graph Microsoft](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и попробуйте пример запросов по маркировке [информационной защиты в Graph Explorer](https://developer.microsoft.com/graph/graph-explorer). Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **Microsoft Information Protection**.
