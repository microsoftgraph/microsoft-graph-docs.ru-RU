---
title: Начало работы с облачными подключениями
description: Узнайте, как можно использовать боты для реагирования на потребности клиентов и упрощение совместной работы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ae04e60079a789125dd6a818c19ec625eaac1443
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871669"
---
# <a name="get-started-with-cloud-communications"></a>Начало работы с облачными подключениями

API облачных коммуникаций в Microsoft Graph добавляют новое измерение, в соответствии с которыми ваши приложения и службы взаимодействуют с пользователями с помощью различных компонентов, связанных с взаимодействием, таких как звонки и собрания по сети. В этой статье описывается, как можно использовать боты для реагирования на потребности клиентов и для упрощения совместной работы.

## <a name="prerequisites"></a>Необходимые компоненты

Беоре вы приступите к работе, вам будет полезно ознакомиться со следующими статьями:

- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) и как служба помогает сотрудникам входить в систему и получать доступ к ресурсам.
- [Служба Azure Bot](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) и ее возможности.

## <a name="register-a-bot"></a>Регистрация Bot

Термины "приложение службы" и "bot" можно использовать в качестве взаимозаменяемых. Вы можете самостоятельно создать объект Bot через [портал Azure](https://azure.microsoft.com/features/azure-portal/) или зарегистрировать Bot, который не размещен в Azure. Более подробную информацию о процессе регистрации Bot можно узнать в статье [регистрация абонентского робота](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). 

Чтобы упростить работу в дальнейшем, полезно знать о различных [типах разрешений](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) в Azure AD. Приложениям с делегированными разрешениями необходимо войти в систему пользователя. Для разрешений на основе приложения пользователь, вошедшего в систему, часто может работать в качестве фоновой службы.

Если вы хотите [Добавить Bot в Microsoft Teams](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), вы можете узнать, как использовать [app Studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio) и определить необходимые метаданные.

## <a name="manage-the-state-of-the-bot"></a>Управление состоянием Bot

После регистрации Bot решите, следует ли размещать мультимедийные и видеоролики в [приложениях или на размещении в службах](cloud-communications-media.md). На высоком уровне это позволяет решить, нужен ли доступ к потоковому носителю без формата RAW.

После этого вы можете решить, подходит ли этот интерфейс для ленты в качестве [состояния или без сохранения](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)состояния.

### <a name="stateless-bots"></a>Боты без сохранения состояния

Любая виртуальная машина может обрабатывать любой экземпляр Bot, что означает, что если один компьютер отключается, другой может позаботиться об этом. Это делает решение устойчивым.

С другой стороны, общий кэш, такой как REDIS, должен быть доступен всем виртуальным машинам.

### <a name="stateful-bots"></a>Боты с ведением базы данных

Виртуальная машина может обрабатывать только один экземпляр Bot за раз. Так как все состояния находятся на одном компьютере, не существует дополнительной проверки памяти или REDIS кэша.

Недостаток состоит в том, что поскольку экземпляр ленты выполняется только на одном компьютере, он не является устойчивым.

>**Примечание:** Размещенные в службах медиа Боты могут быть состояниями или без них. Боты, размещаемые в приложении, должны иметь состояние для использования [пакета SDK для Bot](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).

## <a name="use-the-sdks"></a>Использование пакетов SDK

В C# доступны следующие пакеты SDK. Мы будем предоставлять поддержку других языков в будущем.

- Если вы используете Боты **без сохранения состояния** , установите [пакет SDK для компонента Graph Communications Core SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Если вы используете боты с **ведением состояния** , установите [пакет SDK для связи](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)с помощью Graph.

## <a name="examples"></a>Примеры

Узнайте, как реализовать различные сценарии с помощью боты с ведением базы данных, например [отвечать на входящий вызов](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) с использованием размещенных в приложении или размещенных в службах носителей.

Дополнительные примеры приведены в [репозитории образцов обмена мгновенными сообщениями](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).
