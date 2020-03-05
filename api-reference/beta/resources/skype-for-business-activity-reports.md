---
title: Отчеты о работе со Skype для бизнеса
description: Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: a66780b54239ab6bb87e8c910734a0c1a4ca32fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520494"
---
# <a name="skype-for-business-activity-reports"></a>Отчеты о работе со Skype для бизнеса

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [скипефорбусинессактивитюсердетаил](../resources/skypeforbusinessactivityuserdetail.md) | Получите сведения о действиях пользователей в Skype для бизнеса. |
| [Получение количества действий](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [скипефорбусинессактивитикаунтс](../resources/skypeforbusinessactivitycounts.md) | Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [скипефорбусинессактивитюсеркаунтс](../resources/skypeforbusinessactivityusercounts.md) | Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
