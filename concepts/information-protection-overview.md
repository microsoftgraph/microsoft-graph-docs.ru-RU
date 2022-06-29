---
title: Защита информации Microsoft Purview меток
description: Используйте Защита информации Microsoft Purview для классификации, маркировки и защиты данных на основе меток конфиденциальности. Узнайте, как использовать API меток в Microsoft Graph.
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: 3d1018b76e72d8fde7384d516aa12848768c63bc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444931"
---
# <a name="microsoft-purview-information-protection-labeling-overview"></a>Защита информации Microsoft Purview меток

Защита информации Microsoft Purview помогает организациям классифицировать, помечайте и защищайте данные на основе [меток конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels).

Организации используют метки, чтобы помочь:

* Пользователи, которые понимают важность обрабатываемой информации.
* Администраторы соответствия требованиям при обнаружении местонахождения конфиденциальной информации.
* Администраторы безопасности при развертывании политик доступа к данным и защиты от потери данных на основе более подробных сведений о метках.

## <a name="why-integrate-with-microsoft-purview-information-protection"></a>Зачем выполнять интеграцию с Защита информации Microsoft Purview?

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Интеграция с универсальной платформой маркировки, которая обслуживает миллионы пользователей и устройств

Более миллиона организаций с десятками миллионов пользователей используют Защита информации Microsoft Purview для классификации, маркировки и защиты данных.  Помимо Microsoft 365, различные службы защиты от потери данных (DLP), платформы бизнес-аналитики и решения "программное обеспечение как услуга" (SaaS) уже применяли метки Защита информации Microsoft Purview, чтобы обеспечить более широкие возможности классификации данных.[](https://www.microsoft.com/security/technology/information-protection) 

### <a name="label-information-in-line-of-business-applications"></a>Сведения о метках в бизнес-приложениях

Корпоративные разработчики используют Защита информации Microsoft Purview, чтобы пометить и защитить конфиденциальную информацию клиента при экспорте из бизнес-приложений, чтобы обеспечить безопасность сведений о клиентах. Подключение приложений к экосистеме Защита информации Microsoft Purview позволяет приложениям применять, обновлять и удалять метки конфиденциальности в данных приложения без дополнительных затрат на интеграцию полного пакета SDK.[](/Office365/SecurityCompliance/sensitivity-labels)

## <a name="what-can-i-do-with-microsoft-purview-information-protection-label-apis-in-microsoft-graph"></a>Что можно сделать с Защита информации Microsoft Purview меток в Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Обнаружение меток, доступных пользователю или организации

С помощью Microsoft Graph вы можете получить доступ к [метках](/graph/api/resources/informationprotectionlabel) конфиденциальности, доступным пользователю или организации. Метки применяются приложениями и службами к неактивным или неактивным данным, помогая пользователям и подчиненным приложениям и службам понять конфиденциальность обрабатываемой информации.

### <a name="understand-how-to-apply-labels"></a>Общие сведения о применении меток

Предоставляя сведения о существующей и требуемой метке конфиденциальности, REST API может интеллектуально информировать приложение о действиях, [](/graph/api/resources/informationprotectionaction) которые необходимо предпринять для правильного применения метки. К ним относятся такие действия, как приложение [метаданных](/graph/api/resources/metadataaction) , создание [водяного](/graph/api/resources/addwatermarkaction) знака, [защита](/graph/api/resources/protectbytemplateaction) и т. д.

### <a name="interpret-labels-applied-to-data"></a>Интерпретация меток, примененных к данным

Приложения, использующие информацию, к [](/graph/api/resources/metadataaction) которой уже применены метаданные метки конфиденциальности, могут использовать API **extractLabel** для разрешения метаданных метки в метку Защита информации Microsoft Purview [конфиденциальности](/graph/api/resources/informationprotectionlabel). Используйте метку, чтобы определить действия, которые должны выполняться приложением при обработке или использовании помеченных данных. 

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Защита информации Microsoft Purview API в бета-версии Microsoft Graph](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Дальнейшие действия

- Выберите и попробуйте Information Protection пометить примеры запросов в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). Выберите **Показать другие примеры** в столбце слева. Используйте меню, **чтобы включить Защита информации Microsoft Purview**.
