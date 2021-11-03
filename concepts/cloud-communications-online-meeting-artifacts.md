---
title: Артефакты и разрешения собраний по сети
description: Узнайте о артефактах собраний в Интернете и о том, что необходимо для их получения.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: 59d5bca4e8484d7965eeef44e44c08b7c67b09fb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60685529"
---
# <a name="online-meeting-artifacts-and-permissions"></a>Артефакты и разрешения собраний по сети

Артефакты собраний в Интернете — это контент, производимый в течение продолжительности собрания или Microsoft Teams [в прямом эфире.](/microsoftteams/teams-live-events/what-are-teams-live-events) Вы можете использовать [операцию Get onlineMeeting,](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) чтобы получить следующие артефакты собрания:

- Отчет о посещаемости собрания в Интернете в виде ответа JSON. Отчеты о посещаемости имеют следующие характеристики:
  - Доступно для собраний, не Teams живых событий
  - Доступно только по завершению собрания
  - Только организатор собрания может получить доступ
- Записи Teams в виде ссылки на скачивание, срок действия которого истекает через 60 секунд. Записи имеют следующие характеристики:
  - Доступно только для Teams событий в прямом эфире
  - Доступно только после Teams события в прямом эфире
  - Доступ к Teams может получить только организатор живых событий
- Отчет участника о Teams в виде ссылки на скачивание, срок действия которого истекает через 60 секунд. Отчеты участников имеют следующие характеристики:
  - Доступно только для Teams событий в прямом эфире
  - Доступно только после Teams события в прямом эфире
  - Доступ к Teams может получить только организатор живых событий

## <a name="permissions"></a>Разрешения

Для управления артефактами собраний доступны следующие разрешения.

- Делегированная (работа или учетная запись школы) - OnlineMeetingArtifact.Read.All
- Приложение - OnlineMeetingArtifact.Read.All

Только _onlineMeetingArtifact.Read.All_ permissions are required to fetch online meeting artifacts. До **15 января 2022** г. для получения артефактов собраний в бета-версии можно использовать следующие разрешения:

- _OnlineMeeting.Read_
- _OnlineMeeting.ReadWrite_
- _OnlineMeeting.Read.All_
- _OnlineMeeting.ReadWrite.All_

После этой даты для получения артефактов собраний потребуются разрешения _OnlineMeetingArtifact.Read.All._ запросы, которые не имеют этих разрешений, будут отклонены.
