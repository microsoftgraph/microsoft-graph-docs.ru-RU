---
title: Отчеты о работе со Skype для бизнеса
description: Можно получить подробные сведения об активности внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
ms.openlocfilehash: 3681c733ae641dfd421171c864a737ea083eec41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078156"
---
# <a name="skype-for-business-activity-reports"></a>Отчеты о работе со Skype для бизнеса

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Можно получить подробные сведения об активности внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Получите сведения о действиях пользователей в Skype для бизнеса. |
| [Получение количества действий](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Узнайте, как меняется количество организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
