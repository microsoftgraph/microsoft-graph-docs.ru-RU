---
title: Microsoft Information Protection метки
description: Microsoft Information Protection помогает организациям классифицировать, маркировать и защищать данные на основе Office 365 меток безопасности и соответствия требованиям.
author: tommoser
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: dafa396b5c0d7a27400ddee5c6bb2965dd4abb1d83ccb5f9deef0f71283e1a02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237420"
---
# <a name="information-protection-overview"></a>Обзор защиты информации

Microsoft Information Protection помогает организациям классифицировать, маркировать и защищать данные на основе [конфиденциальности.](/Office365/SecurityCompliance/sensitivity-labels) 

Организации используют метки для оказания помощи:

* Пользователи понимают важность обрабатываемой информации.
* Администраторы соответствия требованиям при обнаружении того, где живет конфиденциальную информацию. 
* Администраторы безопасности при развертывании политик защиты от потери данных и доступа к данным на основе более богатых сведений об меток.

## <a name="why-integrate-microsoft-information-protection"></a>Зачем интегрировать Microsoft Information Protection? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Интеграция с платформой повсеместной маркировки, обслуживающей миллионы пользователей и устройств

Более миллиона организаций с десятками миллионов пользователей используют Microsoft Information Protection для классификации, метки и защиты данных.  Помимо Microsoft 365, различные службы по предотвращению потери данных( DLP), платформы бизнес-аналитики и решения для [](https://www.microsoft.com/security/technology/information-protection) программного обеспечения как-службы (SaaS) приняли Microsoft Information Protection метки, чтобы обеспечить более богатый опыт классификации данных. 

### <a name="label-information-in-line-of-business-applications"></a>Сведения о метки в бизнес-приложениях

Enterprise разработчики используют Microsoft Information Protection для маркировки и защиты конфиденциальной информации о клиентах при экспорте из бизнес-приложений для обеспечения безопасности сведений о клиентах. Подключение приложений к экосистеме Microsoft Information Protection позволяет приложениям применять, обновлять и [](/Office365/SecurityCompliance/sensitivity-labels) удалять метки конфиденциальности в собственных данных приложений без накладных расходов на интеграцию полного SDK.

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>Что можно сделать с API Microsoft Information Protection меток в Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Обнаружение меток, доступных пользователю или организации

С помощью microsoft Graph вы [](/graph/api/informationprotectionlabel?view=graph-rest-beta) можете получить доступ к метки конфиденциальности, доступные пользователю или организации. Метки применяются приложениями и службами к данным в режиме покоя или в движении, помогая пользователям и приложениям и службам ниже по течению понимать чувствительность обработки данных.

### <a name="understand-how-to-apply-labels"></a>Понимание применения меток

Предоставляя сведения о существующей и необходимой мете конфиденциальности, API REST [](/graph/api/resources/informationprotectionaction?view=graph-rest-beta) может разумно информировать ваше приложение о действиях, которые необходимо принять для правильного применения метки. Это включает такие действия, как приложение [метаданных,](/graph/api/resources/metadataaction?view=graph-rest-beta) генерация [водяных](/graph/api/resources/addwatermarkaction?view=graph-rest-beta) знаков, [защита](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta)и другие.

### <a name="interpret-labels-applied-to-data"></a>Интерпретация меток, применяемых к данным

Приложения, потребляющие информацию, [](/graph/api/resources/metadataaction?view=graph-rest-beta) уже применяемую метаданные метки чувствительности, могут использовать API **extractLabel** для решения метаданных меток на метку Microsoft Information Protection [чувствительности.](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta) Используйте метку, чтобы определить действия, которые должно принимать приложение при обработке или потреблении помеченных данных. 

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Microsoft Information Protection API в бета Graph Microsoft](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и попробуйте пример запросов по маркировке информационной защиты [в Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer) Выберите **Показать другие примеры** в столбце слева. Используйте меню, чтобы включить **Microsoft Information Protection**.
