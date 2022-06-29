---
title: Начало работы с API облачных коммуникаций
description: Используйте API облачных коммуникаций в Microsoft Graph для создания ботов для клиентов. Узнайте, как зарегистрировать бот, а затем управлять его состоянием.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: e2b380108d06abc987fdf92564a1ecf17289d9c5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442157"
---
# <a name="get-started-with-the-cloud-communications-api"></a>Начало работы с API облачных коммуникаций

API облачных коммуникаций в Microsoft Graph можно использовать для создания ботов в ответ на потребности клиентов и упрощения совместной работы. В этой статье описывается, как зарегистрировать бот, а затем управлять его состоянием.

## <a name="prerequisites"></a>Предварительные требования

Прежде чем приступить к работе, полезно ознакомиться со следующими сведениями:

- [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) и как служба помогает сотрудникам входить в систему и получать доступ к ресурсам.
- Azure [Служба Bot](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0&preserve-view=true) и его возможности.

## <a name="register-a-bot"></a>Регистрация бота

Термины "приложение-служба" и "бот" можно использовать взаимозаменяемо. Вы можете создать бот с помощью [портал Azure или зарегистрировать](https://azure.microsoft.com/features/azure-portal/) бот, который не размещен в Azure. Дополнительные сведения о процессе регистрации бота см. в разделе ["Регистрация вызывающего бота"](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). 

Чтобы упростить работу позже, полезно понимать различные типы разрешений [в Azure AD](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions). Приложениям с делегированными разрешениями требуется пользователь, выполнив вход. Разрешения на основе приложений не требуют пользователя, выполнившего вход, и часто могут выполняться как фоновая служба.

После регистрации бота, если вы хотите добавить бота в [Microsoft Teams](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), убедитесь, что вы понимаете, как использовать [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) и определить необходимые метаданные.

## <a name="manage-the-state-of-the-bot"></a>Управление состоянием бота

После регистрации бота решите, следует ли разместить аудио- и видеофайл в приложении [или службе](cloud-communications-media.md). На высоком уровне это связано с принятием решения о том, хотите ли вы получить доступ к прямой трансляции необработанного носителя.

Затем вы можете решить, лучше ли для бота быть с отслеживанием [состояния или без отслеживания состояния](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Боты без отслеживания состояния

Любая виртуальная машина может обрабатывать любой экземпляр бота. Это означает, что при сжатии одной машины другой может обработать его. Это обеспечивает отказоустойчивое решение.

С другой стороны, общий кэш, например REDIS, должен быть доступен для всех виртуальных машин.

### <a name="stateful-bots"></a>Боты с отслеживанием состояния

Виртуальная машина может обрабатывать только один экземпляр бота за раз. Так как все состояния находятся на одном компьютере, нет дополнительных проверок памяти или проверок кэша REDIS.

Недостаток заключается в том, что, поскольку экземпляр бота находится только на одном компьютере, он не так устойчив.

> [!NOTE]
> Размещенные в службе боты мультимедиа могут иметь отслеживание состояния или без отслеживания состояния. Чтобы использовать пакет [SDK bot Media](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media), размещенные в приложении, необходимо обеспечить отслеживание состояния.

## <a name="use-the-sdks"></a>Использование пакетов SDK

Следующие пакеты SDK доступны в C#. В будущем мы будем поддерживать другие языки.

- Если вы используете боты без **отслеживания** состояния, установите пакет [SDK Graph Communications Core](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Если вы используете боты с **отслеживанием** состояния, установите пакет [SDK для вызовов Graph Communications](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).

## <a name="examples"></a>Примеры

Узнайте, как реализовать различные сценарии с помощью ботов с отслеживанием состояния[](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls), таких как ответ на входящий вызов с помощью размещенного в приложении или размещенного в службе носителя.

Дополнительные примеры см. в [репозитории примеров Communications](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).

## <a name="privacy-and-compliance"></a>Конфиденциальность и соответствие требованиям

В запросах к API конфиденциальные данные не должны отправляться в заголовках или тексте запроса, созданных на стороне клиента (например, идентификаторы сценариев, идентификаторы запросов или другие идентификаторы корреляции). Эти идентификаторы будут регистрироваться на стороне сервера для диагностики.

## <a name="see-also"></a>См. также

- [Общие сведения об API облачных коммуникаций](cloud-communications-concept-overview.md)