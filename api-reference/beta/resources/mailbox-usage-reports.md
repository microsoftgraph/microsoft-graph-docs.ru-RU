---
title: Отчеты об использовании почтовых ящиков
description: Вы можете получить сведения о пользователях с почтовым ящиком и их уровнем активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463532"
---
# <a name="mailbox-usage-reports"></a>Отчеты об использовании почтовых ящиков

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о пользователях с почтовым ящиком и их уровнем активности, которые в основном основаны на отправленных и полученных сообщениях электронной почты. Вы также можете посмотреть, сколько места занимает каждый почтовый ящик и сколько почтовых ящиков скоро превысят квоту хранилища.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о почтовых ящиках](../api/reportroot-getmailboxusagedetail.md) | Stream          | [Маилбоксусажедетаил](../resources/mailboxusagedetail.md) | Получите сведения об использовании почтовых ящиков.         |
| [Получение количества почтовых ящиков](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [Маилбоксусажемаилбокскаунтс](../resources/mailboxusagemailboxcounts.md) | Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо. |
| [Получение количества почтовых ящиков по состоянию квоты](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [Маилбоксусажекуотастатусмаилбокскаунтс](../resources/mailboxusagequotastatusmailboxcounts.md) | Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты. |
| [Получение занятого объема хранилища](../api/reportroot-getmailboxusagestorage.md) | Stream          | [Маилбоксусажестораже](../resources/mailboxusagestorage.md) | Узнайте, сколько места занято в хранилище организации. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
