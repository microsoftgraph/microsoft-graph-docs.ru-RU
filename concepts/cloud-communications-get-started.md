---
title: Начало работы с облачными коммуникациями
description: Узнайте, как использовать боты для удовлетворения потребностей клиентов и облегчения совместной работы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a977c2a81d40679eb3029bdfaf7560dd744fc9439e7a650e63d470198883ab0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246509"
---
# <a name="get-started-with-cloud-communications"></a>Начало работы с облачными коммуникациями

API облачных коммуникаций в Microsoft Graph новое измерение взаимодействия приложений и служб с пользователями с помощью различных функций, связанных с коммуникацией, таких как вызовы и собрания в Интернете. В этой статье описывается, как можно использовать боты для удовлетворения потребностей клиентов и облегчения совместной работы.

## <a name="prerequisites"></a>Необходимые условия

Перед началом работы полезно ознакомиться со следующими словами:

- [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) и как служба помогает сотрудникам войти и получить доступ к ресурсам.
- Служба [ботов Azure и](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) ее возможности.

## <a name="register-a-bot"></a>Регистрация бота

Термины "приложение-служба" и "бот" можно использовать взаимозаменяемо. Вы можете создать бот непосредственно на [портале Azure](https://azure.microsoft.com/features/azure-portal/) или зарегистрировать бота, который не имеется в Azure. Дополнительные сведения о процессе регистрации ботов см. в [материале Регистрация вызываемого бота.](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html) 

Чтобы упростить работу в дальнейшем, полезно понять различные типы разрешений [в](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) Azure AD. Приложения с делегированными разрешениями требуют от пользователя, вписаного в нее. Разрешения, основанные на приложениях, не требуются пользователю, который может часто работать в качестве фоновой службы.

После регистрации бота, если вы хотите добавить бот в [Microsoft Teams,](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)убедитесь, [](/microsoftteams/platform/get-started/get-started-app-studio) что вы понимаете, как использовать студию приложений и определить необходимые метаданные.

## <a name="manage-the-state-of-the-bot"></a>Управление состоянием бота

После регистрации бота определите, хотите ли вы, чтобы аудио- и видеосвязь была размещена в приложении или [размещена в службе.](cloud-communications-media.md) На высоком уровне для этого необходимо решить, хотите ли вы получить доступ к живому потоку необработанных средств массовой информации.

Далее вы можете решить, лучше ли для вашего бота быть [состоянием или без состояния](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Боты без состояния

Любая виртуальная машина может обрабатывать любой экземпляр бота, что означает, что если одна машина идет вниз, другой может заботиться о нем. Это позволяет сделать решение устойчивым.

С другой стороны, общий кэш, например REDIS, должен быть доступен для всех виртуальных машин.

### <a name="stateful-bots"></a>Состояние ботов

Виртуальная машина может обрабатывать только один экземпляр бота одновременно. Так как все состояния находятся на одной машине, дополнительные проверки памяти или проверки кэша REDIS не проводятся.

Недостатком является то, что, поскольку экземпляр бота находится только на одной машине, он не так устойчив.

>**Примечание:** Медиа-боты, на которые есть служба, могут иметь состояние или состояние без состояния. Для использования [SDK Bot Media SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)с использованием средств массовой информации, на которые есть приложения, необходимо применять состояние.

## <a name="use-the-sdks"></a>Использование пакетов SDK

Следующие SDKs доступны в C#. В будущем мы будем поддерживать другие языки.

- Если вы используете **боты** без состояния, [установите Graph SDK communications Core](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Если вы используете состояние **ботов,** установите Graph [связи вызова SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).

## <a name="examples"></a>Примеры

Узнайте, как реализовать различные сценарии с помощью [](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) штатных ботов, например отвечать на входящий вызов с помощью средств массовой информации с хост-службами или приложениями.

Дополнительные примеры см. в [репозитории образцов communications.](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)

## <a name="privacy-and-compliance"></a>Конфиденциальность и соответствие требованиям

В запросах на наши API конфиденциальные данные не следует отослать в заглавные и запросные ID-данные в заглавных заголовках или в теле запроса. Эти ID будут зарегистрированы на стороне сервера для диагностики.
