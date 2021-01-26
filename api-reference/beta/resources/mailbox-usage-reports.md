---
title: Отчеты об использовании почтовых ящиков
description: Вы можете получить сведения о пользователях с почтовым ящиком и их уровне активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: c679e8b73e0e2a43ded3bffd66fe7c9d14a957d1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983568"
---
# <a name="mailbox-usage-reports"></a>Отчеты об использовании почтовых ящиков

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о пользователях с почтовым ящиком и их уровне активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о почтовых ящиках](../api/reportroot-getmailboxusagedetail.md) | Поток          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | Получите сведения об использовании почтовых ящиков.         |
| [Получение количества почтовых ящиков](../api/reportroot-getmailboxusagemailboxcounts.md) | Поток          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо. |
| [Получение количества почтовых ящиков по состоянию квоты](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Поток          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты. |
| [Получение занятого объема хранилища](../api/reportroot-getmailboxusagestorage.md) | Поток          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | Узнайте, сколько места занято в хранилище организации. |


